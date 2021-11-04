---
title: 加密和金鑰管理概觀
description: 深入瞭解 Microsoft 365 中的加密和金鑰管理
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: f5ba22f53b0f40983bd0f76d2a9ffc2061c2c30e
ms.sourcegitcommit: 444a58b28f8611323e16d28b4c63a0f68eaaafa6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780099"
---
# <a name="encryption-and-key-management-overview"></a>加密和金鑰管理概觀

## <a name="what-role-does-encryption-play-in-protecting-customer-content"></a>加密在保護客戶內容時會扮演什麼角色？

大部分的 Microsoft business 雲端服務是多租使用者，也就是說，客戶內容與其他客戶可以儲存在相同的實體硬體上。 為了保護客戶內容的機密性，Microsoft 線上服務會加密所有靜態資料，並使用一些最強大且最安全的加密通訊協定進行傳輸。

加密不是強存取控制的替代。 Microsoft 的存取控制原則零上的存取 (ZSA) 會保護客戶內容，避免 Microsoft 員工未經授權的存取。 加密是指在任何地方儲存客戶內容的機密性，並防止內容在 Microsoft online 服務系統之間或 Microsoft online 服務和客戶之間傳輸時，保護存取控制。

## <a name="how-do-microsoft-online-services-encrypt-data-at-rest"></a>Microsoft online services 如何加密靜態資料？

Microsoft online services 中的所有客戶內容都受到一或多個加密形式的保護。 Microsoft 伺服器使用 BitLocker 來加密包含磁片磁碟機的磁片磁碟機，該磁片磁片磁碟機包含的容量層級的客戶內容。 BitLocker 所提供的加密，可在其他程式或控制項中不再需要時，保護客戶內容 (例如，對硬體) 的存取控制或回收，可能會導致未經授權的實體存取包含客戶內容的磁片。

除了磁片區層級的加密之外，Microsoft 線上服務會在應用層使用服務加密，以加密客戶內容。 服務加密在增強式加密保護之上提供版權保護和管理功能。 它也可讓 Windows 的作業系統和這些作業系統儲存或處理的客戶資料之間分開。

## <a name="how-do-microsoft-online-services-encrypt-data-in-transit"></a>Microsoft online services 如何加密資料傳輸？

Microsoft online services 使用強大的傳輸通訊協定（例如 TLS），防止未經授權的協力廠商在透過網路移動時竊取客戶資料。 中轉中的資料範例包括正在傳遞的郵件訊息、線上會議中進行的交談，或是資料中心之間複寫的檔案。

在 Microsoft online services 中，每當使用者的裝置與 Microsoft 伺服器通訊，或 Microsoft 伺服器與另一部伺服器通訊時，就會將資料視為「傳輸」。

## <a name="how-do-microsoft-online-services-manage-the-keys-used-for-encryption"></a>Microsoft online services 如何管理加密所用的金鑰？

增強式加密的安全性，只是用來加密資料的金鑰。 Microsoft 會使用自己的安全性憑證來加密資料內傳輸的 TLS 連線。 針對靜態資料，使用完整大量加密金鑰加密 BitLocker 受保護的磁片區，該金鑰是使用大量的主金鑰進行加密，而該金鑰又會系結至伺服器中的受信任平臺模組 (TPM) 。 BitLocker 會使用 FIPS 相容的演算法，以確保加密金鑰永遠不會以明文儲存或傳送。

服務加密為客戶資料提供了另一層加密，讓客戶有兩種加密金鑰管理選項： Microsoft 管理金鑰或客戶金鑰。 使用 Microsoft 管理的金鑰時，Microsoft 線上服務會自動產生並安全地儲存用於服務加密的根機碼。

具有控制其自己之根加密金鑰需求的客戶可以搭配客戶金鑰使用服務加密。 使用客戶金鑰，客戶可以使用內部部署硬體服務模組 (HSM) 或 Azure Key Vault (AKV) 來產生自己的加密金鑰。 客戶根機碼儲存在 AKV 中，而這些機碼是用來加密客戶信箱資料或檔案的其中一個 keychains 的根。 客戶根金鑰只能透過 Microsoft online 服務代碼以間接方式存取，以進行資料加密，而且無法由 Microsoft 員工直接存取。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與加密和金鑰管理相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 10.1：加密控制項 <br> 18.1.5：加密控制項 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 10.1：加密控制項 <br> 18.1.5：加密控制項 | 2020 年 12 月 2 日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=56904fc3-0942-4ff5-9eef-7cabc751a25c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 11.6：以公用資料傳輸網路傳輸之 PII 的加密 | 2020 年 12 月 2 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | DS-1：加密憑證和金鑰的安全儲存 <br> DS-2：客戶資料是在傳輸中加密 <br> DS-3：在傳輸中加密的 Azure 元件內部通訊 <br> DS-4：加密控制項和程式 | 2021 年 3 月 31 日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | SC-8：傳輸機密性和完整性 <br> SC-13：使用密碼編譯 <br> SC-28：靜止資訊保護 <br>  | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 10.1：加密控制項 <br> 18.1.5：加密控制項 | 2021 年 4 月 20 日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=08ce227f-d1d9-4c4c-b255-4f2e4ec8f941&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=43e89534-f48d-42ea-a7a7-3523ff516036&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 11.6：以公用資料傳輸網路傳輸之 PII 的加密 | 2021 年 4 月 20 日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-44：資料中轉加密 <br> CA-54：靜止資料加密 <br> CA-62：客戶金鑰信箱加密 <br> CA-63：刪除客戶金鑰資料 <br> CA-64：客戶金鑰 | 2020月24日 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-16：客戶加密金鑰 <br> CUEC-17：客戶金鑰保存庫 <br>  CUEC-18：客戶金鑰輪替| 2020月24日 |
