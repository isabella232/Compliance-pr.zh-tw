---
title: Exchange OnlineMicrosoft 365 中的資料恢復功能
description: 在本文中，將說明 Exchange Online 和 Microsoft 365 內資料恢復的各個方面。
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
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 8952d492c4427d5f4af64a853adaaf15303e8caf
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088632"
---
# <a name="exchange-online-data-resiliency-in-microsoft-365"></a>Exchange Online Microsoft 365 中的資料恢復功能

>[!IMPORTANT]
>當我們繼續以保留信箱內容的不同方式投資時，我們宣佈 Exchange 系統管理中心的退休 In-Place 保留 (EAC) 中 Exchange Online。 從2020年7月1日開始，您將無法建立新的 In-Place 保留。 不過，您仍然可以管理 EAC 中的 In-Place，或是使用 Exchange Online PowerShell 中的 **Set-MailboxSearch** Cmdlet 來管理。 不過，從2020年10月1日開始，您將無法管理 In-Place 保留。 您只能在 EAC 或使用 **Remove-MailboxSearch** Cmdlet 中移除它們。 仍支援使用 Exchange Server 和 Exchange 混合式部署的 In-Place 保留。 如需 Exchange Online 中封存 In-Place 封存的詳細資訊，請參閱[舊版 eDiscovery tools 的退休](/microsoft-365/compliance/legacy-ediscovery-retirement)。

原有範圍暫止 會保留所有的信箱內容，包括刪除的項目和修改項目的原始版本。 [就地 eDiscovery](/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)搜尋時會傳回這類信箱項目。 當您設定使用者信箱的 In-Place 時，對應的封存信箱中的內容 (若啟用) 也會保留，並在 eDiscovery 搜尋中傳回。

有兩種類型的損毀可能會影響 Exchange 資料庫：實體損毀，通常是由硬體 (所造成，也就是因其他因素而發生的儲存硬體) 問題和邏輯損毀。 一般來說，在 Exchange 資料庫內可能會發生兩種類型的邏輯損毀：

- **資料庫邏輯損毀** -資料庫頁面校驗和相符，但是頁面上的資料在邏輯上有錯誤。 當資料庫引擎 (可擴展的儲存體引擎 (ESE) ) 嘗試寫入資料庫頁面，但即使作業系統會傳回成功訊息時，資料永遠不會寫入磁片或寫入錯誤的位置，就會發生這種情況。 這稱為 *遺失的清除*。 ESE 包含許多功能和保護措施，其設計目的是為了避免資料庫的實體損毀及其他資料遺失案例。 為了避免遺失的刷新遺失資料，ESE 會在資料庫中包含遺失的清除偵測機制，以及 (單一分頁還原的功能) 修正此機制。
- **儲存邏輯損毀** -資料會以使用者未預期的方式新增、刪除或操控。 這兩種情況是由協力廠商應用程式所造成。 使用者將它視為損毀，通常會損毀。 Exchange 存放區會將產生邏輯損毀的交易視為一系列有效的 MAPI 作業。 Exchange Online 中的[In-Place 保留](/exchange/security-and-compliance/create-or-remove-in-place-holds)功能提供對儲存邏輯損毀 (的保護，因為它可防止使用者或應用程式) 永久刪除內容。 

Exchange Online 會在記錄檔檢查和記錄檔重新顯示期間，對複寫的記錄檔執行數種一致性檢查。 這些一致性檢查會防止系統複製實體損毀。 例如，在記錄檢查期間，會有實體完整性檢查可驗證記錄檔，並驗證記錄檔中記錄的檢查碼是否符合記憶體中產生的 checksum。 此外，會檢查記錄檔標頭，確定記錄檔中記錄的記錄檔簽名與記錄檔的記錄檔相符。 在記錄檔重播期間，記錄檔會進一步進行審查。 例如，資料庫標頭也包含與記錄檔的簽名進行比較的記錄簽章，以確保它們相符。 

針對 Exchange Online 中的信箱資料損毀，可透過使用 Exchange 原生資料保護，利用跨多部伺服器和多個資料中心的應用層級複寫來進行保護的修復原則，以及協助防止資料因損毀或其他原因而遺失的其他功能。 這些功能包括由 Microsoft 或 Exchange Online 應用程式本身所管理的原生功能，例如：

- [資料可用性群組](/exchange/back-up-email)
- 單一位修正 
- 線上資料庫掃描 
- 遺失的刷新偵測 
- 單一分頁還原 
- 信箱複寫服務 
- 記錄檔檢查 
- 在彈性檔案系統上部署 

如需先前所列的原生功能的詳細資訊，請選取超連結，並查看下列相關資訊，以及有關沒有超連結之專案的詳細資訊。 除了這些原生功能之外，Exchange Online 也包含客戶可管理的資料恢復功能，例如： 
- [預設會啟用單一專案復原 () ](/exchange/recipients-in-exchange-online/manage-user-mailboxes/recover-deleted-messages) 
- [就地保留與訴訟資料暫留](/exchange/security-and-compliance/in-place-and-litigation-holds) 
- [已刪除的郵件保留和 Soft-Deleted 信箱 (預設為啟用) ](/exchange/recipients-in-exchange-online/delete-or-restore-mailboxes) 

## <a name="database-availability-groups"></a>資料庫可用性群組 
Microsoft 365 中的每個信箱資料庫都裝載于[資料庫可用性群組中 (DAG) ](/exchange/back-up-email)並且複寫到相同地區內位於不同地理位置的資料中心。 最常見的設定是四個資料中心內的四個資料庫副本;不過，有些地區所用的資料中心， (資料庫會複寫至三個資料中心，而在澳大利亞和日本) 有兩個資料中心。 但在所有的情況下，每個信箱資料庫都有四個副本分散在多個資料中心，因此可確保信箱資料受到軟體、硬體甚至資料中心失敗的保護。 

這四個副本中，有三個是設定為高可用性。 第四個副本已設定為 [延遲資料庫副本](/Exchange/high-availability/manage-ha/activate-lagged-db-copies)。 延遲資料庫副本不適用於個別的信箱復原或訊息項目復原。 其目的是為了提供復原機制，以進行極少的系統嚴重損壞邏輯損毀的事件。 

延遲中的資料庫副本是以七天的記錄檔重新顯示延遲時間設定 Exchange Online。 此外，也會啟用 Exchange 重新顯示 Lag 管理員，以提供延遲副本的動態記錄檔，以允許延遲資料庫副本自行修復並記錄管理檔成長。 雖然延遲資料庫副本是用於 Exchange Online，但是請務必瞭解它們不是一個有保證的時間點備份。 延遲 Exchange Online 中的資料庫副本具有可用性閾值（通常是90%），因為磁片上有延遲副本因磁片故障而遺失的情況，延遲副本會變成高可用性的副本 (，因為這是因為自動向下) ，也就是延遲資料庫副本重新產生記錄檔重放佇列的期限。 

## <a name="transport-resilience"></a>傳輸恢復 
Exchange Online 包括兩個主要的傳輸恢復功能：卷影冗余及安全性 Net。 「陰影冗余」會在傳輸期間保留郵件的重複副本。 [安全性] Net 會在成功傳遞郵件後，保留郵件的重複副本。 

有了陰影冗余，每個 Exchange Online 傳輸伺服器都會在它認可成功接收郵件至傳送伺服器的每一封郵件上進行複本。 這會使傳輸管線中的所有郵件在傳輸期間都是多餘的。 如果 Exchange Online 判斷原始郵件在傳輸過程中遺失，將會重新傳遞郵件的重複副本。 

安全網路是與信箱伺服器上的傳輸服務相關聯的傳輸佇列。 此佇列儲存伺服器已成功處理的郵件副本。 當信箱資料庫或伺服器失敗需要啟用信箱資料庫的過期複本時，系統會自動將安全網路佇列中的郵件重新提交至信箱資料庫的新主動副本。 Net Net 也是多餘的，因此可避免傳輸成為單一失敗點。 它使用主要安全網和陰影安全網路的概念，其中如果主要的安全網在超過12小時內不可用，則重新提交要求會變成陰影重新提交要求，而且會從陰影的安全網路重新傳遞郵件。

由管理 DAGs 和信箱資料庫副本之 Microsoft Exchange 複寫服務的 Active Manager 元件自動啟動來自安全網的郵件 safety。 不需要手動動作便可重新提交來自安全網路的郵件。 

## <a name="single-bit-correction"></a>單一位修正 
ESE 包含一種機制，可偵測和解決單一位 CRC 錯誤 (也稱為單一位翻轉) ，這是硬體錯誤的結果 (，所以它們代表實體損毀) 。 當發生這些錯誤時，ESE 會自動修正這些錯誤，並記錄事件記錄檔中的事件。 

## <a name="online-database-scanning"></a>線上資料庫掃描 
線上資料庫掃描 (也稱為 *資料庫檢查求和*) 是 ESE 使用資料庫一致性檢查程式來讀取每個頁面及檢查分頁損毀的處理常式。 主要用途是偵測可能無法透過事務性作業偵測到的實際損毀和遺失的刷新。 資料庫掃描也會執行儲存後的損毀作業。 磁碟空間可能會因損毀而洩漏，而且線上資料庫掃描會找到並恢復遺失的空間。 系統所設計的預期是每7天完全掃描一次每個資料庫。 

## <a name="lost-flush-detection"></a>遺失的刷新偵測 
當磁片子系統/作業系統傳回完成的資料庫寫入作業實際上未寫入磁片，或是寫入錯誤的位置時，就會發生遺失清除。 遺失的刷新事件可能會導致資料庫邏輯損毀，因此，避免遺失的刷新導致資料遺失，ESE 會包含遺失的清除偵測機制。 當資料庫頁面寫入被動副本時，會對使用中副本上的遺失的刷新執行檢查。 如果偵測到遺失的清除，ESE 便可使用頁面修補程式修復處理常式。 

## <a name="single-page-restore"></a>單一分頁還原 
單一分頁還原（也稱為 *頁面修補*）是一種自動處理方式，在狀況良好的副本中，完好的副本會取代損壞的資料庫頁面。 損壞頁面的修復程式取決於資料庫副本為主動或被動。 當作用中的資料庫副本遇到損毀的頁面時，它可以從其複本中複製頁面（只要它所複製的頁面是最新的）。 您可以將頁面要求放入記錄檔（即信箱資料庫複寫的基礎），以完成此程式。 當複本到達頁面要求時，它會傳送頁面的副本到要求的資料庫副本，以進行回應。 單一分頁還原也提供非同步通訊機制，可讓作用中從複本要求頁面，即使複本目前已離線也是一樣。 

在被動資料庫副本（包括延遲資料庫副本）遭到損毀時，因為這些複本永遠落後于主動副本，所以將任何頁面從主動副本複製到被動複本時，總會是安全的。 被動資料庫副本的自然可用性非常高，所以在修補頁面時，記錄檔重新顯示已暫停，但記錄複製會繼續進行。 被動資料庫副本會從主動副本中檢索損毀的頁面複本，直到複製並檢查符合最大要求記錄檔要求的記錄檔為止，然後再修補損壞的頁面。 在修補頁面後，記錄檔重新顯示簡歷。 延遲資料庫副本的程式是相同的，唯一不同之處在于，延遲資料庫會先重新顯示取得能狀態所需的所有記錄檔。 

## <a name="mailbox-replication-service"></a>信箱複寫服務 
移動信箱是管理大規模電子郵件服務的重要部分。 時刻都有更新的技術與硬體和版本升級，使我們的工程師能夠完成這項工作，同時讓使用者能在) 整個程式中保持線上，使信箱對使用者 (保持線上狀態，並確保在信箱變得更大及更大的情況下，處理常式會適當地伸縮。 

Exchange 的信箱複寫服務 (MRS) 負責在資料庫之間移動信箱。 在移動期間，MRS 會對信箱內的所有專案執行一致性檢查。 如果發現一致性問題，MRS 將修正問題，或略過損毀的專案，進而移除信箱的損毀。 

因為 MRS 是 Exchange Online 的元件，所以我們可在其程式碼中進行變更，以解決未來所偵測到的新損毀形式。 例如，如果我們偵測到 MRS 無法修正的一致性問題，我們可以分析損毀、變更 MRS 程式碼，並修正不一致的 (如果我們瞭解如何) 。 

## <a name="log-file-checks"></a>記錄檔檢查 
Exchange 資料庫所產生的所有交易記錄檔都會經歷數種不同的一致性檢查格式。 在建立記錄檔時，首先會寫入一個位模式，然後執行一系列的記錄寫入作業。 此結構可讓 Exchange Online 執行一系列的檢查 (遺失的清除、CRC 和其他檢查，) 在寫入每個記錄檔時進行驗證，以及在複製時重新驗證。 

## <a name="deployment-on-resilient-file-system"></a>在彈性檔案系統上部署 
若要防止檔案系統層級的損毀，Exchange Online 部署于彈性檔案系統上 (ReFS) 磁碟分割以提供增強的復原功能。 ReFS 是 Windows Server 2012 和更新版本中的檔案系統，其設計使其能夠更具彈性，避免資料損毀，從而使資料的可用性和完整性達到最大。 具體而言，ReFS 會以更新中繼資料的方式取得改進，以提供更好的資料保護，並減少資料損毀案例。 它也會使用校驗和來驗證檔案資料和中繼資料的完整性，以確保容易找到並修復資料損毀。 

Exchange Online 會利用數個 ReFS 優點： 
- 資料完整性的彈性越多，意味著較少的資料損毀事件。 減少損毀事件的數量，意味著較少不必要的資料庫重新植入。 
- 在中繼資料上執行的檢查碼，可使偵測到破壞案例的速度更快且更明確，讓我們能夠修正客戶資料損毀，在資料量出現灰色失敗之前。
- 可搭配大型資料集（pb 和更大）搭配效能，而不會影響效能
- 支援 Exchange Online 所使用的其他功能，例如 BitLocker 加密。 

Exchange Online 也會受益于其他 ReFS 功能： 
- **完整性 (完整性資料流程)** ReFS 儲存資料的方式，可防止一般會導致資料遺失的常見錯誤。 Microsoft 365搜尋會使用完整性資料流程，協助早期磁片損毀偵測和檔案內容的校驗和。 此功能也可減少因「斷寫」所造成的損毀事件， (當寫入作業由於電源中斷等問題而無法完成時，請 ) 。 
- **可用性 (搶救)** ReFS 優先順序的資料可用性。 從過去的角度來看，檔案系統常常會受到資料損毀的破壞，需要系統離線才能進行修復。 雖然很少會發生損毀，但 ReFS 會執行搶救，這項功能會從即時磁片區上的命名空間中移除損毀的資料，並確保無法在非修復損毀的資料上受到不良的資料影響。 套用搶救功能並隔離資料損毀以 Exchange Online 資料庫磁片區，意味著我們可以將不受影響的資料庫置於損毀與修復動作之間的健康磁片。 此結構可增加一般會受到這類磁片損毀問題影響的資料庫可用性。 
