---
title: 身分識別和存取管理概觀
description: 深入瞭解 Microsoft 365 中的身分識別和存取管理
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 373c910f4c97f7f9ff89ea346c8dceef84dd6a07
ms.sourcegitcommit: 01938022a292c07e98041dc6ae1312a1b8c617db
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260834"
---
# <a name="identity-and-access-management-overview"></a>身分識別和存取管理概觀

## <a name="how-do-microsoft-online-services-protect-production-systems-from-unauthorized-or-malicious-access"></a>Microsoft online services 如何防止未授權或惡意存取的實際執行系統？

Microsoft 線上服務的設計可讓 Microsoft 的工程師在未存取客戶內容的情況下操作服務。 根據預設，Microsoft 工程師會讓 Access (ZSA) 客戶內容，而且不會存取實際執行環境。 Microsoft online services 使用即時 (JIT) ，只要有足夠的存取 (JEA) 模型，就能讓服務小組工程師在必要時存取生產環境，以支援 Microsoft 線上服務。 JIT 存取模型可讓工程師在必要時要求暫時提升到具有特殊權限的角色，以此取代傳統的持續性系統管理存取權。

指派給服務小組以支援生產服務的工程師，可透過身分識別和存取管理解決方案，向服務小群組帳戶要求資格。 要求要求會觸發一系列的人員檢查，以確保工程師已超過所有雲端篩選需求、已完成必要的訓練，以及在建立帳戶之前接收適當的管理核准。 只有在符合所有資格要求之後，才能為要求的環境建立服務小組帳戶。 若要維護服務小群組帳戶的資格，各人員必須每年進行角色型訓練，並每兩年 rescreening。 無法完成或通過這些檢查會導致 eligibilities 自動撤銷。

服務小群組帳戶不會授與任何對客戶內容的系統管理員許可權或存取權。 當工程師需要其他存取權來支援 Microsoft online services 時，他們會使用稱為「密碼箱」的 access 管理工具，以暫時存取所需資源。 Lockbox 會將提升的存取權限制在完成指定工作所需的最低權限、資源和時間。 如果授權的檢閱者核准 JIT 存取要求，工程師會授與暫存檔，只具有完成所指派工作所需的許可權。 這個暫存帳戶需要多重因素驗證，而且會在已核准的期限到期後自動刪除。

JEA 會在要求進行 JIT 存取時由 eligibilities 和密碼箱角色強制執行。 只接受對工程師 eligibilities 範圍內資產的存取權，並傳遞給核准者。 「密碼箱」會自動拒絕在工程師的 eligibilities 和密碼箱角色範圍外的 JIT 要求，包括超過允許閾值的要求。  

## <a name="how-do-microsoft-online-services-use-role-based-access-control-rbac-with-lockbox-to-enforce-least-privilege"></a>Microsoft online services 如何使用擁有角色的存取控制 (RBAC) 使用密碼箱，以強制執行最低的許可權？

服務小群組帳戶不會授與任何對客戶內容的系統管理員許可權或存取權。 有限系統管理員許可權的 JIT 要求是透過密碼箱進行管理。 密碼箱使用 RBAC 限制工程師可進行的 JIT 提升要求類型，提供額外的保護層級，以強制執行最低的許可權。 RBAC 也會將服務小群組帳戶限制于適當的角色，以協助強制進行責任的分隔。
支援服務的工程師會根據其角色授與安全性群組的成員資格。 安全性群組中的成員資格不會授與任何許可權存取權。 相反地，安全性群組可讓工程師在必要時，使用密碼箱來要求 JIT 提升以支援系統。 工程師可以採取的特定 JIT 要求是由其安全性群組成員資格所限制。

## <a name="how-do-microsoft-online-services-handle-remote-access-to-production-systems"></a>Microsoft online services 如何處理對實際執行系統的遠端存取？

Microsoft 線上服務系統元件是存放在與運作小組分散在不同地理位置的資料中心。 資料中心人員不具備 Microsoft 線上服務系統的邏輯存取權。 因此，Microsoft 服務小組人員會透過遠端存取來管理環境。 需要遠端存取支援 Microsoft online 服務的服務小組人員，只會在核准者核准後，授與遠端存取權。 所有遠端存取都使用 FIPS 140-2 相容 TLS 進行安全的遠端連線。

Microsoft online services 使用安全的系統管理工作站 () 服務小組遠端存取，以協助保護 Microsoft online 服務環境不會遭到損害。 這些工作站的設計目的是防止故意或意外地遺失實際執行資料，包括鎖定 USB 埠，以及將安全系統管理員工作站上的軟體限制在支援環境所需的功能。 會密切追蹤和監控安全的系統管理員工作站，以偵測 Microsoft 工程師的客戶資料，並防止其惡意或不慎損損。

## <a name="how-does-customer-lockbox-add-additional-protection-for-customer-content"></a>客戶的密碼箱如何為客戶內容新增額外的保護？

客戶可以啟用客戶密碼箱，將其他的存取控制層級新增至其內容。 當密碼箱提升要求涉及客戶內容的存取權時，客戶加密箱需要客戶核准，成為核准工作流程的最後一個步驟。 此程式可讓組織選擇核准或拒絕這些要求，並為客戶提供直接的存取控制。 如果客戶拒絕客戶加密箱要求，就會拒絕存取要求的內容。 如果客戶在特定期間內未拒絕或核准要求，則要求會自動到期，而不會有 Microsoft 取得客戶內容的存取權。 如果客戶核准要求，則在指派完成疑難排解作業的時間到期後，Microsoft 暫時存取客戶內容將會自動進行記錄、審核和吊銷。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與身分識別與存取控制相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.1：存取控制的商務需求 <br> 9.2： User access management <br> 9.3：使用者責任 <br> 9.4：系統和應用程式存取控制 <br> 15.1：供應商關聯中的資訊安全性 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.1：存取控制的商務需求 <br> 9.2： User access management <br> 9.3：使用者責任 <br> 9.4：系統和應用程式存取控制 <br> 15.1：供應商關聯中的資訊安全性 | 2020 年 12 月 2 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | OA-2：布建存取 <br> OA-7： JIT 存取 <br> OA-21：安全的系統管理工作站和 MFA | 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-2：帳戶管理 <br> AC-3：存取強制 <br> AC-5：分隔職責 <br> AC-6：最低許可權 <br> AC-17：遠端存取 | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.1：存取控制的商務需求 <br> 9.2： User access management <br> 9.3：使用者責任 <br> 9.4：系統和應用程式存取控制 <br> 15.1：供應商關聯中的資訊安全性 | 2021 年 4 月 20 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-33：修改帳戶 <br> CA-34：使用者驗證 <br> CA-35：特殊許可權存取 <br> CA-36：遠端存取 <br> CA-57：客戶密碼箱 Microsoft 管理核准 <br> CA-58：客戶加密箱服務要求 <br> CA-59：客戶密碼箱通知 <br> CA-61： JIT 檢查和核准 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-32：共用帳戶原則 <br> CA-33：修改帳戶 <br> CA-34：使用者驗證 <br> CA-35：特殊許可權存取 <br> CA-36：遠端存取 <br> CA-53：協力廠商監控 <br> CA-56：客戶的密碼箱客戶核准 <br> CA-57：客戶密碼箱 Microsoft 管理核准 <br> CA-58：客戶加密箱服務要求 <br> CA-59：客戶密碼箱通知 <br> CA-61： JIT 檢查和核准 | 2020月24日 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-15：客戶加密箱要求 | 2020月24日 |