---
title: Skype、OneDrive、SharePoint 和 Exchange 的加密
description: 摘要： Skype、OneDrive、SharePoint、Microsoft Teams 及 Exchange Online 加密的描述。
ms.author: krowley
author: kccross
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: None
search.appverid:
- MET150
ms.collection:
- Strat_O365_Enterprise
- M365-security-compliance
- Strat_O365_Enterprise
- SPO_Content
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 77371208a5bd6d67fb9239ceebb18319b9a9253c265d7233ed789d75ba2e1815
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54287182"
---
# <a name="encryption-for-skype-for-business-onedrive-for-business-sharepoint-online-microsoft-teams-and-exchange-online"></a>商務用 Skype、商務用 OneDrive、SharePoint 線上、Microsoft Teams 及 Exchange Online 的加密

Microsoft 365 是高安全性的環境，可提供多層的廣泛保護：實體資料中心安全性、網路安全性、存取安全性、應用程式安全性及資料安全性。

## <a name="skype-for-business"></a>商務用 Skype

商務用 Skype 客戶資料可能會以會議參與者上傳的檔案或簡報形式儲存在靜止的位置。 Web 會議伺服器會使用含256位金鑰的 AES 加密客戶資料。 加密的客戶資料會儲存在檔案共用上。 每個客戶資料都是以不同隨機產生的256位金鑰加密。 當會議中有一部分客戶資料共用時，Web 會議伺服器會指示會議用戶端透過 HTTPS 下載加密的客戶資料。 它會將對應的機碼傳送給用戶端，以便能夠解密客戶資料。 Web 會議伺服器也會驗證會議用戶端，讓用戶端能夠存取會議客戶資料。 加入 Web 會議時，每個會議用戶端會建立 SIP 對話，讓會議焦點元件在前端伺服器透過 TLS 執行。 會議焦點會將 Web 會議伺服器所產生的驗證 cookie 傳遞給會議用戶端。 然後，會議用戶端會連接到 Web 會議伺服器，以顯示驗證 cookie，以供伺服器驗證。

## <a name="sharepoint-online-and-onedrive-for-business"></a>SharePoint Online 和商務用 OneDrive

在 SharePoint Online 中的所有客戶檔案，都是以唯一的、每個副檔名為單一租使用者的金鑰保護。 這些機碼是由 SharePoint 線上服務建立及管理，或由客戶使用、建立及管理客戶金鑰。 上載檔案時，會在上傳要求的內容中 SharePoint 線上執行加密，然後再將其傳送至 Azure 儲存體。 下載檔案時，SharePoint 線上會根據唯一的檔識別碼從 Azure 儲存體檢索加密的客戶資料，並在將客戶資料傳送給使用者前解密客戶資料。 Azure 儲存區沒有能力解密，甚至可識別或瞭解客戶資料。 所有的加密和解密都會發生在強制租使用者隔離的相同系統中，也就是 Azure Active Directory 和 SharePoint 線上。

在線上 SharePoint 中 Microsoft 365 儲存資料的數種工作負載，包括 Microsoft Teams，它會儲存 SharePoint online 中的所有檔案，並商務用 OneDrive 使用 SharePoint 線上存放。 所有儲存在 SharePoint Online 中的客戶資料都是以一或多個 AES 256 位金鑰) 和分散于整個資料中心的方式進行加密 (，如下所示。  (此加密處理常式的每一個步驟都是驗證 FIPS 140-2 層級2。 如需有關 FIPS 140-2 規範的詳細資訊，請參閱 [fips 140-2 相容性](/previous-versions/sql/sql-server-2008-r2/bb326611(v=sql.105))。 ) 

- 每個檔案都會分割成一或多個區塊，視檔案大小而定。 每個區塊都會以其專屬唯一的 AES 256 位金鑰加密。
- 更新檔案時，會以相同的方式處理更新：此變更會分割成一或多個區塊，而且每個區塊都會以個別的唯一金鑰加密。
- 這些區塊–檔案、檔片段和更新變化–會以 blob 形式儲存在 Azure 存放區中，而這些儲存體會隨機分散在多個 Azure 儲存體帳戶。
- 這兩個客戶資料區塊的加密金鑰集也會加密。

    - 用來加密 blob 的金鑰會儲存在 SharePoint 線上內容資料庫中。
    - 內容資料庫是由資料庫存取控制和靜止加密所保護。 在[Azure SQL Database](/azure/sql-database/sql-database-technical-overview)中使用[透明資料加密](/sql/relational-databases/security/encryption/transparent-data-encryption-tde) (TDE) 執行加密。  (Azure SQL Database 是一個一般用途的關係資料庫 Microsoft Azure 服務，可支援諸如關聯式資料、JSON、空間和 XML 等結構。 ) 這些機密是在線上 SharePoint 的服務層級，而不是在租使用者層級。 這些機密 (有時候稱為主要金鑰) 儲存在個別的安全存放庫中，稱為機碼存放區。 TDE 為使用中的資料庫與資料庫備份和交易記錄，提供了靜止的安全性。
    - 當客戶提供選用的金鑰時，客戶金鑰會儲存在 Azure Key Vault 中，而且服務會使用金鑰來加密租使用者金鑰（用來加密網站機碼，然後用來加密檔層級金鑰）。 實質上，當客戶提供金鑰時，會引入新的主要階層。
- 用來重新裝配檔案的對應，會與加密金鑰一起儲存在內容資料庫中，並與解密所需的主金鑰分開。
- 每個 Azure 儲存體帳戶每一種存取類型都有自己的唯一認證 (讀取、寫入、列舉和刪除) 。 每個認證集都會保留在安全的金鑰存放區中，且會定期重新整理。 如以上所述，有三種不同類型的存放區，各有不同的功能：
    - 客戶資料會在 Azure 儲存體中儲存為加密的 blob。 每個客戶資料區塊的金鑰會加密，並分別儲存在內容資料庫中。 客戶資料本身不會持有如何解密的任何線索。
    - 內容資料庫為 SQL Server 資料庫。 它會保留找出並重新組裝 Azure 儲存區中的客戶資料 blob 以及加密這些 blob 所需的金鑰所需的對應。 不過，這些機碼集本身就是以上述方式加密 () 並保留在個別的金鑰存放區中。
    - 主要存放區與內容資料庫和 Azure 儲存區實際分開。 它會保留每個 Azure 儲存體容器的認證，以及保留在內容資料庫中的加密金鑰集的主要金鑰。

每個這三個儲存元件– Azure blob 存放區、內容資料庫及主要存放區–都是以實際方式個別。 任何一種元件中的資訊，都無法自行使用。 若未存取所有三種方式，將機碼取回到區塊中是不可能的，解密機碼使其可供使用、將機碼與對應區塊相關聯、解密每個區塊，或從其構成區塊重新構建檔。

BitLocker 憑證，用來保護資料中心內電腦上的實體磁片區，會儲存在安全的存放庫中 (伺服器陣列金鑰所保護的 SharePoint 線上機密存放區) 。

保護每個 blob 機碼的 TDE 機碼會儲存在兩個位置：

- 安全存放庫，它會容納 BitLocker 憑證，並受伺服器陣列金鑰保護;和
- 在 Azure SQL Database 所管理的安全存放庫中。

用於存取 Azure 儲存體容器的認證也會保留在 SharePoint 線上機密存放區中，並視需要委派給每個 SharePoint online 伺服器陣列。 這些認證是 Azure storage SAS 特徵碼，使用不同的認證來讀取或寫入資料，並套用原則，讓它們每60天自動到期。 不同的認證是用來讀取或寫入資料 (但不是) ，也不會授予 SharePoint 線上伺服器陣列的列舉許可權。

> [!NOTE]
> 針對 Office 365 美國政府客戶，資料 blob 儲存在 Azure 美國政府儲存體中。 此外，Office 365 美國政府的 SharePoint Online 機碼的存取權僅限於已特別遮罩 Office 365 員工。 Azure 美國政府運作人員無法存取用來加密資料 blob 的 SharePoint Online 機碼存放區。

如需 SharePoint 線上及商務用 OneDrive 中的資料加密的相關資訊，請參閱[商務用 OneDrive 和 SharePoint Online 中的資料加密](https://technet.microsoft.com/library/dn905447.aspx)。

### <a name="list-items-in-sharepoint-online"></a>在 SharePoint Online 中列出專案

清單專案是一些小型的客戶資料區塊，可在網站內隨意建立，例如使用者建立清單中的資料列、SharePoint online 博客中的個別文章，或 SharePoint 線上 wiki 頁面中的專案。 清單專案會儲存在內容資料庫中 (Azure SQL Database) 並以 TDE 加以保護）。

## <a name="encryption-of-data-in-transit"></a>傳輸中資料的加密

在OneDrive for Business 和 SharePoint Online 中，資料進出資料中心的方式有兩種。

- **用戶端與伺服器** 之間的通訊若要 SharePoint 線上及透過網際網路商務用 OneDrive 使用 TLS 連線。
- **資料中心之間的資料移動** -在資料中心之間移動資料的主要原因是用於地理位置複寫，以啟用嚴重損壞修復。 例如，SQL Server交易記錄和 Blob 儲存體差異會隨時此管道流動。 若己使用私人網路傳輸資料，則系統會進一步以業界領先的加密方式保護資料。

## <a name="exchange-online"></a>Exchange Online

Exchange Online 會針對所有信箱資料使用 BitLocker，BitLocker 設定會在 BitLocker 中說明[為加密](/microsoft-365/compliance/office-365-bitlocker-and-distributed-key-manager-for-encryption)。 服務層級加密會加密信箱層級的所有信箱資料。 

除了服務加密之外，Microsoft 365 支援客戶金鑰，這是以服務加密為基礎的。 客戶金鑰是 microsoft 管理的金鑰選項，可供 microsoft 的藍圖上的 Exchange Online 服務加密使用。 這種加密方法可提供 BitLocker 所提供的增強保護，因為它提供伺服器管理員的隔離和解密資料所需的加密金鑰，而且因為加密是以直接方式套用至資料 (BitLocker，因此會在邏輯磁片磁片區上套用加密，) 從 Exchange 伺服器複製的任何客戶資料仍保持加密。

Exchange Online 服務加密的範圍是存放在 Exchange Online 中的客戶資料。  (商務用 Skype 會在使用者的 Exchange Online 信箱內儲存幾乎所有使用者產生的內容，因此會繼承 Exchange Online 的服務加密功能。 ) 


## <a name="microsoft-teams"></a>Microsoft Teams

Teams 會使用 TLS 及 MTLS 來加密立即訊息。 不論流量是限制在內部網路或越過內部網路周邊，所有伺服器對伺服器的流量都需要 MTLS。

此表摘要 Teams 所使用的通訊協定。

|**流量類型**|**加密者**|
|:-----|:-----|
|伺服器對伺服器|MTLS|
|用戶端對伺服器 (ex。 立即訊息與顯示狀態) |TLS|
|媒體流程 (ex。 媒體) 的音訊和影片共用|TLS|
|媒體的音訊和影片共用|SRTP/TLS|
|信號|TLS|

#### <a name="media-encryption"></a>媒體加密

媒體流量都是使用安全 RTP (SRTP) 加密，它是即時傳輸通訊協定 (RTP) 的設定檔，為 RTP 流量提供機密性、驗證功能和重播攻擊防護。 SRTP 使用以安全亂數產生器所產生，並使用信號 TLS 通道進行交換的工作階段金鑰。 用戶端對用戶端媒體流量是透過用戶端對伺服器的連線信號進行協商，但是會在用戶端對用戶端直接前往用戶端時以 SRTP 加密。

Teams 會使用認證型權杖，以透過輪流安全地存取媒體轉送。 媒體轉送透過 TLS 安全通道交換權杖。

#### <a name="fips"></a>Fips

Teams 會使用 FIPS (聯邦資訊處理標準) 相容性演算法，以進行加密金鑰交換。 如需實施 FIPS 的詳細資訊，請參閱 [聯邦資訊處理標準 (FIPS) 發佈 140-2](/microsoft-365/compliance/offering-fips-140-2)。
