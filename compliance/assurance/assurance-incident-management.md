---
title: 事件管理概觀
description: 深入瞭解 Microsoft 365 中的事件管理
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
ms.openlocfilehash: 203adce9b4c7167315abbbfbebce0efdd604fefe
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481945"
---
# <a name="incident-management-overview"></a>事件管理概觀

## <a name="what-is-a-security-incident"></a>什麼是安全性事件？

Microsoft 在其線上服務中定義的安全性事件為已確認的安全性缺口，其在 Microsoft 處理客戶資料或個人資料時，導致意外或非法損毀、遺失、更改、未經授權披露或存取客戶資料或個人資料。 例如，未經許可存取 Microsoft online services 基礎結構和 exfiltration 客戶資料會構成安全性事件，而不會影響服務或客戶資料的機密性、完整性或可用性的相容性事件，也不會被視為安全性事件。

## <a name="how-does-microsoft-respond-to-security-incidents"></a>Microsoft 如何回應安全性事件？

每當發生安全性事件時，Microsoft 會盡力快速且有效地回應，以保護 Microsoft 服務和客戶資料。 Microsoft 採用一個事件回應策略，其設計目的是快速且有效地調查、包含及移除安全性威脅。

Microsoft 雲端服務會持續受到危害的跡象。 除了自動化的安全性監控和警示之外，所有員工都會收到年度訓練，以辨識可能的安全性事件，並向其報告跡象。 員工、客戶或安全性監控工具所偵測到的任何可疑活動都會上報給服務特有的安全性回應小組以進行調查。 所有服務運作小組（包括服務特有的安全性回應小組）都會維護深入的呼叫輪替，以確保資源可供全天候事件回應使用。 我們的來電旋轉可讓 Microsoft 在任何時間或規模（包括廣泛或同時發生的事件）上裝載有效的事件回應。

偵測到可疑活動並上報可疑活動時，服務特有的安全性回應小組會啟動 **分析、包容、eradication 及** 復原的處理常式。 這些小組會協調潛在事件的分析，以判斷其範圍，包括對客戶或客戶資料的影響。 根據這項分析，服務特有的安全性回應小組會與受影響的服務小組合作，以制定包含威脅的計畫，並將事件的影響降至最低、消除環境中的威脅，以及完全恢復至已知的安全狀態。 相關的服務小組會利用服務特有安全性回應小組的支援來執行計畫，以確保已成功消除威脅，而且受影響的服務會進行完整的修復。

在解決事件後，服務小組會執行從該事件獲知的任何經驗教訓，以更好地避免、偵測及回應未來的類似事件。 選取安全性事件，尤其是對客戶造成影響的事件，或造成資料破壞的事件，檢討後會進行完整的事件。 事後剖析的設計旨在找出技術性失誤、程序性失敗、人工錯誤，以及可能導致事件或在事件回應程序期間所識別的其他程式瑕疵。 檢討後所識別的增強功能可與服務特有的安全性回應小組共同執行，以協助避免未來的事件，並改善偵測和回應功能。

## <a name="how-and-when-are-customers-notified-of-security-or-privacy-incidents"></a>客戶如何以及何時向客戶通報安全性或隱私權事件？

每當 Microsoft 意識到違反授權的安全性（包括客戶資料遺失、披露或修改）時，Microsoft 會在72小時內通知受影響的客戶，如線上服務條款 (OST) 的資料保護附錄 (DPA) 所述。 通知時間軸承諾在正式宣告安全性事件時開始。 宣告安全性事件時，通知程式會盡可能快速進行，而不會過度延遲。

通知包括對破壞性質的描述、使用者影響的大致，以及緩解步驟 (（如果適用）) 。 如果 Microsoft 的調查在初始通知時未完成，則通知也會指出後續通訊的後續步驟和時程表。

如果客戶意識到可能影響 Microsoft 的事件，包括但不限於資料洩密，客戶會負責立即向 Microsoft 通知 Microsoft 事件，如 DPA 中所定義。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與事件管理相關的控制措施。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 16.1：管理資訊安全性事件和增強功能 | 2021年12月2日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 16.1：管理資訊安全性事件和增強功能 | 2021年12月2日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=56904fc3-0942-4ff5-9eef-7cabc751a25c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 9.1：涉及 PII 的資料侵犯通知  | 2021年12月2日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1：事件管理架構 <br> IM-2：偵測機制及警示 <br> IM-3：事件回應執行 <br> IM-4：事件 mortems 後 <br> IM-6：事件回應測試 <br> OA-7：待命工程師存取 | 2021年3月31日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CCM-9：鑒證程式 <br> CUEC：報告事件 <br> IM-1：事件管理架構 <br> IM-2：偵測機制及警示 <br> IM-3：事件回應執行 <br> IM-4：事件 mortems 後 <br> IM-6：事件回應測試 <br> OA-7：待命工程師存取 <br> SOC2-6：客戶支援網站 <br> SOC2-9：服務儀表板 | 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | IR-4：事件處理 <br> IR-6：附隨報告 <br> IR-8：事件回應計畫 | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 16.1：管理資訊安全性事件和增強功能 | 2021 年 4 月 20 日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 10.1：涉及 PII 的資料侵犯通知  | 2021 年 4 月 20 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-26：安全性附隨報告 <br> CA-47：事件回應 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-12：服務等級協定 (Sla)  <br> CA-13：事件回應指南 <br> CA-15：服務健康情況通知  <br>  <br> CA-26：安全性附隨報告 <br> CA-29：待命工程師 <br> CA-47：事件回應 | 2020月24日 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08：報告事件  | 2020月24日  |

## <a name="resources"></a>資源

- [線上服務條款 (OST)](https://www.microsoft.com/licensing/product-licensing/products)
- [資料保護附錄 (DPA) ](https://www.microsoft.com/licensing/product-licensing/products)
- [Azure 和 Office 365 的 Microsoft 雲端事件管理執行指導方針](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=a8a7cb87-9710-4d09-8748-0835b6754e95&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)
- [Office 365-2019 的 Office 365 Third-Party 漏洞評估](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=e85e478f-2491-435d-9c1b-2f0ad7ca8e56&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_Pen_Test_and_Security_Assessments)
