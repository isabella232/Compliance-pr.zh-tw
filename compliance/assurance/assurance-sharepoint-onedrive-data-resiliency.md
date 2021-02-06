---
title: 在 Microsoft 365 中 SharePoint 和 OneDrive 資料恢復功能
description: 本文提供 Microsoft 365 中 SharePoint 和 OneDrive 資料恢復功能的概覽。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 26281e076ea2500a0a4071233b88c2a1f23fe9c5
ms.sourcegitcommit: 21ed42335efd37774ff5d17d9586d5546147241a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/05/2021
ms.locfileid: "50120452"
---
# <a name="sharepoint-and-onedrive-data-resiliency-in-microsoft-365"></a>在 Microsoft 365 中 SharePoint 和 OneDrive 資料恢復功能

在 Microsoft 365 內，OneDrive 是以 SharePoint 檔案平臺為基礎。 在本文中，只會使用 SharePoint 來指代這兩種產品。 本文內容適用于 Microsoft 365，不適用於消費者服務。

有兩個主要資產組成 SharePoint 的核心內容存放區：

- **中繼資料**：每個檔案的中繼資料都儲存在 Azure SQL Database 中。 Azure SQL 提供完整的商務持續性情景，本文稍後會涵蓋 SharePoint 使用方式及詳細資料。
- **Blob 儲存**：上傳至 SharePoint 的使用者內容儲存在 Azure 儲存體中。 SharePoint 已在 Azure 存放區上建立自訂恢復計畫，以確保對使用者內容和真正主動/主動系統的近乎即時的重複。

若要確保資料恢復功能，請在進一步闡述一組完整的控制項。

## <a name="blob-storage-resilience"></a>Blob 儲存恢復

SharePoint 有一個自訂的解決方案，用來儲存 Azure Storage 中的客戶資料。 每個檔案都會同時寫入主要和次要資料中心區域。 如果寫入任一 Azure 區域失敗，檔案儲存將會失敗。 在將內容寫入 Azure Storage 之後，會以中繼資料個別儲存校驗和，並用於確定已送出的寫入與您在所有未來讀取期間傳送給 SharePoint 的原始檔案相同。 在所有工作流程中使用相同的技術，以防止傳播應該發生的任何損毀。 在每個地區內，Azure 本機冗余儲存體 (LRS) 提供高層次的可靠性。 如需詳細資訊，請參閱 [Azure Storage 冗余度](/azure/storage/common/storage-redundancy-lrs) 一文。

SharePoint 會使用 Append-Only 儲存區。 此程式可確保檔案在初始儲存後無法變更或損毀，但也可以使用產品版本的版本設定，即可檢索任何先前版本的檔內容。

任一資料中心的 SharePoint 環境都可以存取兩個 Azure 區域中的儲存體容器。 基於效能原因，相同本地資料中心內的儲存容器永遠都是可取的，但是在所需閾值內，未看到結果的讀取要求將會有相同的遠端資料中心要求的內容，以確保資料永遠可用。

## <a name="metadata-resilience"></a>中繼資料恢復

SharePoint 中繼資料在儲存使用者內容的位置和存取機碼儲存于 Azure Storage 中儲存的內容時也很重要。 這些資料庫是儲存在 Azure SQL 中，其具有大量的 [業務持續性計畫](/azure/sql-database/sql-database-business-continuity)。

SharePoint 使用 Azure SQL 所提供的複寫模型，並已建立專屬的自動化技術，以判斷是否需要容錯移轉，並視需要啟動作業。 如此一來，它會從 Azure SQL 的觀點降至「手動資料庫容錯移轉」類別。 Azure SQL database 可恢復性的最新指標可于 [這裡](/azure/azure-sql/database/business-continuity-high-availability-disaster-recover-hadr-overview#recover-a-database-to-the-existing-server)取得。

SharePoint 使用 Azure SQL 的備份系統來啟用時間點還原 (PITR) 最多14天。 PITR 會在[稍後的章節](#deletion-backup-and-point-in-time-restore)中涵蓋。

## <a name="automated-failover"></a>自動容錯移轉

SharePoint 會使用自訂的自動容錯移轉，將發生特定位置的事件時，對客戶體驗的影響降至最低。 在特定閾值以外，監控導向的自動化會偵測到單一或多個元件的失敗，因此會導致將所有使用者的活動自動重新導向到問題環境，並移至溫次要。 容錯移轉會導致中繼資料及計算儲存完全從新的資料中心內服務。 因為 blob 儲存區永遠執行完全使用/使用中，所以容錯移轉不需要進行任何變更。 計算階層優先于最接近的 blob 容器，但會隨時使用本機和遠端 blob 儲存位置，以確保可用性。

SharePoint 使用 Azure 前門服務，以提供 Microsoft 網路的內部路由。 此設定可讓獨立于 DNS 的容錯移轉重新導向，並減少本機電腦快取的影響。 大多數的容錯移轉作業對使用者而言都是透明的。 如果發生容錯移轉，客戶將不需要進行任何變更，以維護服務的存取權。

## <a name="versioning-and-files-restore"></a>版本設定與檔案還原

針對新建立的文件庫，SharePoint 在每個檔案上都預設為500版本，且您可以設定為保留更多版本（如有需要）。 使用者介面不允許設定小於100版本的值，但是可以使用 public APIs 將系統設定為儲存較少的版本。 出於可靠性的考慮，不建議使用小於100的任何值，而且可能會導致意外資料遺失的使用者活動。

如需版本設定的詳細資訊，請參閱 [SharePoint 中的版本](/microsoft-365/community/versioning-basics-best-practices)設定。

[檔案還原] 是指在過去30天內，將 SharePoint 任何文件庫中的「回到目前」時間的功能。 此程式可用於從勒索軟體復原、大量刪除、損毀或任何其他事件。 這項功能會使用檔版本，以便減少預設版本，以降低此還原的效能。

檔案還原功能會為 [OneDrive](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15) 和 [SharePoint](https://support.office.com/article/Restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)進行記錄。

## <a name="deletion-backup-and-point-in-time-restore"></a>刪除、備份和時間點還原

從 SharePoint 刪除的使用者內容會經歷下列刪除流程。

刪除的郵件會保留在回收站中的特定一段時間。 SharePoint，保留時間為93天。 當您從原始位置刪除專案時，它就會開始。 當您從網站回收站刪除專案時，它會進入 [網站集合的回收站](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)。 在其餘的93天內，它會持續保留，然後永久刪除。 下列連結提供如何使用回收站的詳細資訊：

- [還原回收站中的專案](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be)
- [從網站集合回收站還原已刪除的專案](https://support.office.com/article/Restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)。

此程式是預設刪除流程，而且不會納入帳戶保留原則或標籤。 如需詳細資訊，請參閱 [瞭解保留的 SharePoint 和 OneDrive](/microsoft-365/compliance/retention-policies-sharepoint)。

在93天的回收管線完成之後，就會獨立進行中繼資料及 Blob 儲存的刪除。 中繼資料將立即從資料庫中移除，除非從備份還原中繼資料，否則會使內容無法讀取。 SharePoint 維護14天的元資料備份。 這些備份會以接近即時的方式從本機取得，然後根據此出版物中的檔，以 [檔](/azure/sql-database/sql-database-automated-backups) 的方式，將其推入冗余 Azure 存放容器中的儲存體，其為5-10 分鐘排程。

當您刪除 Blob 儲存內容時，SharePoint 會利用 Azure Blob 儲存的虛刪除功能，以防止意外或惡意的刪除。 使用此功能，我們總共有14天的時間來還原內容，再永久刪除。

>[!Note]
>雖然 Microsoft 應用程式會將內容傳送至標準程式的回收站，但 SharePoint 會提供 APIs，讓您可以略過回收站及強制立即刪除。 請複查您的應用程式，以確保這種做法只會因規範原因而必要。

## <a name="integrity-checks"></a>完整性檢查

SharePoint 會使用各種方法來確保 blob 和中繼資料的完整性，在資料生命週期的各階段：

- **儲存在中繼資料中的檔案雜湊**：整個檔案的雜湊會以檔案中繼資料儲存，以確保在所有作業期間維護檔層級的資料完整性
- **Blob 雜湊儲存于中繼資料中**：每個 Blob 專案會儲存加密內容的雜湊，以防止基礎 Azure 儲存區損毀。
- **資料完整性工作**：每隔14天，會列出資料庫中的專案，並符合 Azure 儲存體中列出的 blob，針對每個網站進行完整性掃描。 工作會報告任何 blob 參照缺失的儲存體-blob，而且可以視需要透過 [Azure 儲存體虛刪除](/azure/storage/blobs/soft-delete-blob-overview) 功能取得這些 blob。
