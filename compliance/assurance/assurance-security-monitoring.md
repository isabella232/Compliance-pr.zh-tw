---
title: 安全性監視概觀
description: 深入瞭解 Microsoft 365 中的安全性監控
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
ms.openlocfilehash: c39acaae68ea8c9f6b4503df55a52d344f10c36fc2792b2202961b5ebe51f32a
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54292061"
---
# <a name="security-monitoring-overview"></a>安全性監視概觀

## <a name="what-is-microsofts-strategy-for-monitoring-security"></a>Microsoft 的監控安全性策略為何？

Microsoft 365 會持續監視其系統的安全性，以偵測及回應對 Microsoft 365 服務的威脅。 安全監控和警示的主要原則包括：

- 健壯：偵測各種攻擊行為的信號和邏輯
- 準確性：有意義的提醒可避免干擾干擾
- 速度：能夠快速吸引攻擊者，以停止攻擊

自動化、規模、雲端式解決方案為監測和回應策略的關鍵要點。 為了我們能有效捕捉和停止某些針對 Microsoft 365 核心服務規模的攻擊，我們的監視系統必須以近乎即時的方式自動發出高度精確的警示。 同樣地，當偵測到問題時，我們需要能夠以規模來緩解風險，我們無法依賴我們的團隊手動修正隨機器的問題。 為了大規模降低風險，我們使用雲端式工具以自動套用因應措施，並提供工具給工程師以在整個環境中快速套用獲核准的風險降低措施。

## <a name="how-does-microsoft-365-perform-security-monitoring"></a>Microsoft 365 如何執行安全性監控？

Microsoft 365 會使用集中式記錄，針對可能指出安全性事件的活動，收集和分析記錄事件。 集中式記錄工具會匯總來自所有系統元件的記錄，包括事件記錄、應用程式記錄、存取控制記錄，以及網路型入侵偵測系統。 除了伺服器記錄和程式層級資料之外，我們服務的核心基礎結構還配備自訂的安全性代理程式，可產生詳細的遙測並提供主機型入侵偵測。 我們會使用此遙測進行監視和取證。

我們收集的記錄和遙測資料可啟用24/7 安全性警示。 我們的警示系統會在記錄資料上傳時分析資料，以幾乎即時的方式產生警示。 這包括以規則型的警示，和其它以機器學習模型為基礎的更複雜警示。 我們的監視邏輯超越一般攻擊案例，並納入對服務架構和作業的深層認知。 我們使用安全性監視資料以持續改善我們的模型，以偵測新型攻擊並改善安全性監視的準確性。

## <a name="how-does-microsoft-365-respond-to-security-monitoring-alerts"></a>Microsoft 365 如何回應安全監控警示？

當我們需要採取行動以回應警示或透過服務進一步調查鑑定證據時，我們的雲端式工具可讓我們在整個環境中快速回應。 這些工具含有完全自動化的智慧型代理程式，可回應偵測到的威脅與安全性因應措施。 在許多情況下，這些代理程式會部署自動化因應措施，以在不需要人為介入的情況下大規模降低安全性偵測。 如果無法執行這項操作，安全性監視功能系統會自動向適當的待命工程師 (已配有一組工具) 發出警示，讓他們即時採取行動並大規模緩解偵測到的威脅。 已將潛在的事件上報至 Microsoft 365 的安全性回應小組，會使用安全性事件回應程式加以解決。

## <a name="how-does-microsoft-365-monitor-system-availability"></a>Microsoft 365 如何監視系統可用性？

Microsoft 365 主動監視其系統，以瞭解資源的使用狀況和反常使用方式。 資源監控是由服務冗余技術所結合，以協助避免意外停機，並讓客戶能夠可靠地存取產品和服務。 服務健康情況問題會透過服務健康情況儀表板 (SHD) ，立即向客戶傳遞。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與安全性監控相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------|:--------|:------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | AC-2：帳戶管理 <br> AC-17：遠端存取 <br> AU-7：審核減少與報告產生 <br> SI-4：資訊系統監控 <br> SI-7：軟體、固件和資訊完整性 <br> | 2020年9月24日 |
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.3：可用性監控與容量規劃 | 2021 年 4 月 20 日 |
| [ISO 27017 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.3：可用性監控與容量規劃 <br> 16.1：管理資訊安全性事件和增強功能 | 2021 年 4 月 20 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19：變更監控 <br> CA-26：安全性附隨報告 <br> CA-29：待命工程師 <br> CA-48：資料中心記錄 | 2020月24日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19：變更監控 <br> CA-26：安全性附隨報告 <br> CA-29：待命工程師 <br> CA-30：可用性監控 <br> CA-48：資料中心記錄 | 2020月24日 |
| [SOC 3 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08：報告事件 <br> CUEC-10：服務合約 | 2020月24日 |

## <a name="resources"></a>資源

- [幕後運作：保護為 Microsoft 365 服務提供後援的基礎結構](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
