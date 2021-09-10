---
title: Microsoft 365 Exchange Online 資料刪除
description: 深入瞭解如何在 Exchange Online 中處理信箱和信箱內的信箱及專案的軟和硬性資料刪除。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 9dd365e075226d8fdbfd1a9f9e371df2668f814d
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58946953"
---
# <a name="exchange-online-data-deletion-in-microsoft-365"></a>Microsoft 365 中的 Exchange Online 資料刪除

在 Exchange Online 中，有兩種刪除專案：虛刪除和實刪除。 這適用于信箱中的信箱和專案。

## <a name="soft-deleted-and-hard-deleted-mailboxes"></a>虛刪除和實刪除的信箱

虛刪除的使用者信箱是已使用 Microsoft 365 系統管理中心或 Remove-Mailbox Cmdlet 刪除的信箱，但在30天內仍會保留在 Azure Active Directory 回收站中。 您可以使用下列任何方式，將信箱變成虛刪除：

- 會虛刪除使用者信箱的相關 Azure Active Directory 使用者帳戶， (使用者物件超出範圍或回收站容器) 。
- 使用者信箱的相關 Azure Active Directory 使用者帳戶已實刪除，但 Exchange Online 信箱處於訴訟暫止或 eDiscovery 暫止狀態。
- 使用者信箱的相關聯 Azure Active Directory 使用者帳戶已在過去30天內清除。這是最大保留長度 Exchange Online 會將信箱保留在虛刪除的狀態，永久地將其清除且無法復原。

實刪除的使用者信箱是已使用下列其中一種方式刪除的信箱：

- 使用者信箱已虛刪除超過30天，且相關聯的 Azure Active Directory 使用者已硬性刪除。 會永久刪除所有信箱內容，例如電子郵件、連絡人及檔案。
- 與使用者信箱相關聯的使用者帳戶已從 Azure Active Directory 中硬性刪除。 在 Exchange Online 中，使用者信箱現在已虛刪除，並保持30天的虛刪除狀態。 若30天的期限內，新的 Azure Active Directory 使用者會從原始收件者帳戶同步處理 **ExchangeGuid** 或 **ArchiveGuid** 的原始收件者帳戶，而該新帳戶已取得 Exchange Online 的授權，這會導致刪除原始使用者信箱的硬拷貝。 會永久刪除所有信箱內容，例如電子郵件、連絡人及檔案。
- 虛刪除信箱會使用 **Remove-Mailbox PermanentlyDelete** 來刪除。

上述刪除案例假設使用者信箱未處於保留狀態，例如訴訟暫止或 eDiscovery 暫止。 如果信箱上有任何類型的保留，則無法刪除信箱。 針對所有郵件使用者收件者類型，會忽略任何 [保留](https://support.office.com/article/manage-legal-investigations-in-office-365-2e5fbe9f-ee4d-4178-8ff8-4356bc1b168e?ui=en-US&rs=en-US&ad=US) 設定，而且不會影響實刪除或虛刪除。

## <a name="soft-deleted-and-hard-deleted-items"></a>虛刪除和實刪除的專案

當使用者刪除信箱專案 (例如電子郵件、連絡人、行事曆約會或工作) 時，該專案會移至 [可復原的專案] 資料夾，以及名為 "delete" 的子資料夾中。 這稱為虛刪除。 刪除的專案保留在「刪除」資料夾中的時間，取決於為該信箱設定的已刪除專案保留期間。 Exchange Online 信箱預設會將刪除的專案保留14天，但 Exchange Online 管理員可以變更此設定，使其最長可增加30天。  (如需增加 Exchange Online 信箱之已刪除專案保留期間的詳細步驟，請參閱[變更保留 Exchange Online 信箱的永久刪除專案的時間長度](/exchange/recipients-in-exchange-online/manage-user-mailboxes/change-deleted-item-retention)。 ) 使用者可以在刪除專案的保留時間到期之前，復原或清除刪除的專案。 若要這樣做，他們會使用 Microsoft Outlook 或 Outlook 網頁版中的 [復原刪除的郵件] 功能。

如果使用者使用 Outlook 或 Outlook 網頁版中的 [復原刪除的郵件] 功能來清除已刪除的專案，則這稱為實刪除。 在 Exchange Online 中，預設會在建立新信箱時啟用單一專案復原，因此，管理員仍可在刪除的專案保留期間到期之前，先[復原](/Exchange/recipients/user-mailboxes/recover-deleted-messages)已刪除的郵件。 此外，如果使用者或程式變更了郵件，則在啟用單一專案復原時，也會保留原始專案的副本。

## <a name="page-zeroing"></a>清空頁面

*清零* 是一種安全性機制，可在刪除的資料上寫入零或二進位模式，使刪除的資料更難於復原。 在 Exchange Online 中，信箱資料庫使用 *頁面* 作為其存放區，並執行稱為 *分頁零* 的覆寫處理常式。 頁面清零預設為啟用，且無法由客戶或 Microsoft 停用。 頁面清零作業會記錄在交易記錄檔中，以類似的方式，讓指定資料庫的所有副本都具有頁面零的功能。 在主動資料庫副本上清空頁面，會導致頁面在資料庫的被動副本上取得零。

頁面清零會寫入實刪除記錄的二進位模式。 頁面清零模式專用於可擴展的儲存體引擎 (ESE) 作業 (伺服器在 Exchange Online) 中使用的內部資料庫引擎名稱，而且與後臺資料庫維護作業的執行時間作業不同。  (後臺資料庫維護是一種持續校驗及掃描每個資料庫的程式。 其主要功能是對資料庫頁面進行校驗和，但也會處理清理空間，並清空未清零的記錄和頁面，因為儲存區損毀。 ) 

下表列出對應至特定執行階段作業的填滿圖樣。

| ESE 執行階段作業   | 填滿圖樣 |
|--------------------------|--------------|
| 取代                  | R            |
| 記錄/長數值刪除 | D            |
| 釋放的頁面空間         | H            |

下表列出對應至特定作業的填滿圖樣，這些作業是在 ESE 背景資料庫維護期間進行。

| ESE 背景資料庫維護作業 | 填滿圖樣 |
|-----------------------------------------------|--------------|
| 記錄刪除                                 | D            |
| 長數值刪除                             | L            |
| 部分使用頁面的已釋放頁面空間       | Z            |
| 未使用頁面的已釋放頁面空間               | U            |

### <a name="page-zeroing-process"></a>頁面清空處理常式

分頁清空的程式取決於刪除的案例。 下表討論資料庫刪除案例，以及分頁清空功能發生的時間。

| 資料庫刪除案例 | 清空資料庫資料 的 ESE 處理程序和時段 |
|:--------------------------|:------------------------------------------------|
| 專案會根據刪除專案的保留期間到期。 | 非同步執行緒會以二進位模式覆寫刪除的資料。 此動作會在記錄刪除的幾毫秒內發生。 如果儲存區處理常式當非同步清零工作仍未完成時， (或因版本儲存區) 成長而取消時，則會取消清空版本，因為後臺資料庫維護處理資料庫的該區段時，則會完成清零。 |
| 查看案例：從 Outlook/Outlook 網頁版資料夾檢視中的專案到期 (例如，交談 view)  | 資料清空會在背景資料庫維護處理該區段的資料庫時進行。 |
| 移動信箱/刪除信箱案例：刪除來源信箱 (到期的已刪除信箱)  | 資料清空會在背景資料庫維護處理該區段的資料庫時進行。 |

### <a name="mailbox-data-types-without-page-zeroing"></a>不含頁面清零的信箱資料類型

下列信箱資料類型未提供分頁清空的規定：

- **信箱資料庫交易記錄** -當交易記錄刪除為一般作業的一部分時，系統會在儲存已刪除記錄檔的檔案系統中，不會有任何程式會將其封鎖 (s) 。 檔案系統可能會很快 reutilize 新建立記錄的可用空間，但不能保證會發生這種情況。
- **內容索引目錄** 檔案-Exchange Online 使用搜尋 Foundation (也稱為 FAST) 的搜尋索引功能。 搜尋索引目錄是由數個檔案所組成，與信箱資料庫檔案儲存在相同的磁片區上。 從信箱資料庫實刪除郵件時，不會立即刪除搜尋類別目錄中關聯的內容。 當搜尋 Foundation 會將許多小型目錄檔案的陰影 (或主合併) 至一個較大的檔案，便會發生內容刪除。 完成主要合併後，便會將較小的類別目錄檔案刪除。 未儲存已刪除的目錄檔案的區塊沒有任何處理程式。

## <a name="continuous-replication"></a>連續複寫

連續複寫 (也稱為記錄傳送及重新顯示) 是 Exchange Online 中建立及維護每個信箱資料庫副本以提供高可用性、網站恢復能力及嚴重損壞修復的技術。 連續複寫使用 Exchange Server 資料庫崩潰復原支援，提供技術，以執行非同步更新的信箱資料庫的一或多個複本。 每個信箱伺服器都會記錄在使用中資料庫上進行的資料庫更新 (例如，使用者的電子郵件活動) 為一組連續 1 MB 交易記錄檔中的記錄記錄。 這組檔稱為記錄資料流程。 在連續複寫中，記錄資料流程也是用來非同步更新資料庫的一個或多個複本。 若要完成此項操作，您可以將記錄傳送至包含主動資料庫被動副本的位置，然後將它們重新顯示至被動資料庫副本。 如果使用資料庫的被動副本重新顯示所有的記錄，則這兩個資料庫是相同的，而在此程式中，對作用中資料庫所做的任何實體變更都會複寫到該資料庫的所有被動複本。

任何從信箱資料庫刪除、信箱專案或整個信箱，以及虛刪除或實刪除，都代表對使用中資料庫的實體變更。 頁面清零也會必然對使用中的資料庫進行實際變更。 這些變更會透過稱為連續複寫的處理常式寫入記錄檔，當這些記錄檔重新執行資料庫的被動副本時，就會對那些被動資料庫進行相同的實際變更。
