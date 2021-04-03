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
ms.openlocfilehash: d431a7f04b156b003f5f4e213aef9bb9792874fe
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497161"
---
# <a name="identity-and-access-management-overview"></a>身分識別和存取管理概觀

## <a name="how-does-microsoft-365-protect-production-systems-from-unauthorized-or-malicious-access"></a>Microsoft 365 如何防止未授權或惡意存取的實際執行系統？

Microsoft 365 的設計可讓 Microsoft 的工程師在未存取客戶內容的情況下操作服務。 根據預設，Microsoft 365 工程師會將存取權 (ZSA) 客戶內容，而且不會存取實際執行環境。 Microsoft 365 使用即時 (JIT) ，只需足夠存取 (JEA) 模型，以提供服務小組工程師，以在支援 Microsoft 365 時，具有實際的許可權存取實際執行環境。 JIT 存取模型會取代傳統的持續性系統管理存取，讓工程師在必要時要求暫時提升為特權角色。

指派給服務小組以支援生產服務的工程師會透過身分識別管理工具 (IDM) ，向服務小群組帳戶要求資格。 要求要求會觸發一系列的人員檢查，以確保工程師已超過所有雲端篩選需求、已完成必要的訓練，以及在建立帳戶之前接收適當的管理核准。 只有在符合所有資格需求之後，才可為要求的環境建立服務小群組帳戶。

服務小群組帳戶不會授與任何對客戶內容的系統管理員許可權或存取權。 當工程師需要其他存取權來支援其 Microsoft 365 服務時，他們會使用稱為「密碼箱」的 access 管理工具，以暫時提升存取所需的資源。 「密碼箱」會限制完成所指派工作所需的最低許可權、資源和時間的許可權。 如果授權的檢閱者核准 JIT 存取要求，工程師會授與暫存檔，只具有完成所指派工作所需的許可權。 此暫存帳戶需要多重要素驗證，而且會在已核准的期限到期後自動刪除。

## <a name="how-does-microsoft-365-handle-remote-access-to-production-systems"></a>Microsoft 365 如何處理生產系統的遠端存取？

Microsoft 365 系統元件是存放在與運作小組分開的資料中心。 資料中心人員不具備 Microsoft 365 系統的邏輯存取權。 因此，Microsoft 365 服務小組人員會透過遠端存取來管理環境。 需要 Microsoft 365 的遠端存取權的服務小組人員，只會在核准者核准後授與遠端存取權。 所有遠端存取使用 FIPS 140-2 相容的 TLS，以進行安全的遠端連線。

Microsoft 365 使用安全的系統管理工作站 (SAWs) 以取得服務小組遠端存取，以協助保護 Microsoft 365 環境免受損損。 這些工作站專門設計用來避免實際或無意中的實際執行資料遺失，包括鎖定 USB 埠，並將所見即用的軟體限制為支援環境所需的功能。 SAWs 會密切追蹤並加以監控，以偵測 Microsoft 工程師的客戶資料，並防止其惡意或不慎損損。

## <a name="how-does-customer-lockbox-add-additional-protection-for-customer-content"></a>客戶的密碼箱如何為客戶內容新增額外的保護？

客戶可以啟用客戶密碼箱，將其他的存取控制層級新增至其內容。 當密碼箱提升要求涉及客戶內容的存取權時，客戶加密箱需要客戶核准，成為核准工作流程的最後一個步驟。 這可讓組織選擇核准或拒絕這些要求，並為客戶提供直接的存取控制。 如果客戶拒絕客戶加密箱要求，就會拒絕存取要求的內容。 如果客戶在特定期間內未拒絕或核准要求，則要求會自動到期，而不會有 Microsoft 取得客戶內容的存取權。 如果客戶核准要求，則在指派完成疑難排解作業的時間到期後，Microsoft 暫時存取客戶內容將會自動進行記錄、審核和吊銷。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與身分識別與存取控制相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | AC-2：帳戶管理 <br> AC-3：存取強制 <br> AC-5：分隔職責 <br> AC-6：最低許可權 <br> AC-17：遠端存取 | 2020年9月24日 |
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.1：存取控制的商務需求 <br> 9.2： User access management <br> 9.3：使用者責任 <br> 9.4：系統和應用程式存取控制 <br> 15.1：供應商關聯中的資訊安全性 | 2020 年 2 月 22 日 |
| [ISO 27017 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.2： User access management <br> 9.4：系統和應用程式存取控制 <br> 15.1：供應商關聯中的資訊安全性 | 2020 年 2 月 22 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-33：修改帳戶 <br> CA-34：使用者驗證 <br> CA-35：特殊許可權存取 <br> CA-36：遠端存取 <br> CA-57：客戶密碼箱 Microsoft 管理核准 <br> CA-58：客戶加密箱服務要求 <br> CA-59：客戶密碼箱通知 <br> CA-61： JIT 檢查和核准 | 2020月24日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-32：共用帳戶原則 <br> CA-33：修改帳戶 <br> CA-34：使用者驗證 <br> CA-35：特殊許可權存取 <br> CA-36：遠端存取 <br> CA-53：協力廠商監控 <br> CA-56：客戶的密碼箱客戶核准 <br> CA-57：客戶密碼箱 Microsoft 管理核准 <br> CA-58：客戶加密箱服務要求 <br> CA-59：客戶密碼箱通知 <br> CA-61： JIT 檢查和核准 | 2020月24日 |
| [SOC 3 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-15：客戶加密箱要求 | 2020月24日 |