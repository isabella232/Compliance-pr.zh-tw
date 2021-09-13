---
title: 網路安全性
description: 深入瞭解 Microsoft 365 中的網路安全性
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
ms.openlocfilehash: 92da9e7bb2716f61088e02c244cb9905af142ead
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158819"
---
# <a name="network-security-overview"></a>網路安全性概觀

## <a name="how-do-microsoft-online-services-secure-the-network-boundary"></a>Microsoft online services 如何保護網路界限？

Microsoft 線上服務採用多種策略來保護其網路界限，包括自動偵測及防護網路型攻擊、特殊的防火牆裝置，以及 Exchange Online Protection 反垃圾郵件和反惡意程式碼保護的 (EOP) 。 此外，Microsoft online services 會將其實際執行環境分隔成邏輯隔離的網段，只需要在區段間進行必要的通訊。 網路流量會以邊界點為其他網路防火牆進行保護，以協助偵測、防止及緩解網路攻擊。

## <a name="how-do-microsoft-online-services-defend-against-ddos-attacks"></a>Microsoft online services 如何防禦 DDoS 攻擊？

Microsoft 的大型網際網路平臺服務會將其與許多分散式阻斷服務 (DDoS) 攻擊的負面影響隔離開來。 每個 Microsoft online 服務的分散式實例，以及每個服務的多個路由，都限制對系統的 DDoS 攻擊所造成的影響。 這項重複功能可提升 Microsoft 線上服務對 DDoS 攻擊的吸收能力，增加在影響服務可用性之前偵測及緩解 DDoS 攻擊的時間量。

除了 Microsoft 的重複系統架構之外，Microsoft 還使用複雜的偵測和緩解工具來回應 DDoS 攻擊。 特殊用途的防火牆會監視和丟棄不想要的流量，使邊界跨越網路，以減少位於網路界限內之系統的壓力。 若要進一步保護我們的雲端服務，Microsoft 會利用在 Microsoft Azure 中部署 DDoS 防護系統。 Azure DDoS 防護系統的設計是要經受外界和其他 Azure 承租人的攻擊。

## <a name="how-does-microsoft-protect-users-against-spam-and-malware-being-uploaded-or-sent-through-online-services"></a>Microsoft 如何針對透過線上服務上傳或傳送的垃圾郵件和惡意程式碼保護使用者？

Microsoft online services 會組建反惡意程式碼保護至可能為惡意程式碼之媒介的服務，例如 Exchange Online 和 SharePoint 線上。 Exchange Online Protection (EOP) 會掃描所有電子郵件和電子郵件附件中的惡意程式碼，以防惡意程式碼進入及結束系統，以防傳遞受感染的郵件和附件。 「高級垃圾郵件篩選」會自動套用至輸入和輸出郵件，以協助防止客戶組織接收和傳送垃圾郵件。 這種保護層會防範利用未經授權或未經授權電子郵件的攻擊，例如網路釣魚攻擊。 SharePoint線上使用相同的病毒偵測引擎，可選擇性地掃描上載的檔案中是否有惡意程式碼。 如果檔案標示為已感染，使用者就無法下載或同步處理該檔案，以保護用戶端端點。 同樣地，Azure 也會比較與上傳到 Azure 儲存體的檔案相關的雜湊與這些已知惡意程式碼雜湊值。 找到相符專案時，會在 Azure Security Center 中產生警示，針對警示的合法性及應如何解決此問題進行決策。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與網路安全性相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | VM-1：安全性事件記錄 <br> VM-3：入侵偵測和監控 <br> VM-4：惡意事件調查 <br> VM-6：弱點掃描 <br> VM-7：網路裝置設定 <br> VM-8：滲透測試 <br> VM-9：網路裝置安全性事件記錄 <br> VM-13：網路裝置弱點弱點 | 3月31日。 2021 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | SC-5：拒絕服務保護 <br> SC-7：界限保護 <br> SI-2：缺陷修正 <br> SI-3：惡意程式碼保護 <br> SI-8：垃圾郵件保護 | 2020年9月24日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27：薄弱環節掃描 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27：薄弱環節掃描 <br> CA-45：反惡意程式碼 | 2020月24日 |