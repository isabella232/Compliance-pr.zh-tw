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
ms.openlocfilehash: 37213f9c9ccab59bbd956cb64c1b2f16a8d72821
ms.sourcegitcommit: 1f30616328d7deb04e41dcbd44a330ea937fe94f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/26/2021
ms.locfileid: "60582476"
---
# <a name="security-monitoring-overview"></a>安全性監視概觀

## <a name="what-is-microsofts-strategy-for-monitoring-security"></a>Microsoft 的監控安全性策略為何？

Microsoft 參與了其系統的連續安全監控，以偵測和回應 Microsoft 線上服務的威脅。 安全監控和警示的主要原則包括：

- 健壯：偵測各種攻擊行為的信號和邏輯
- 準確性：有意義的提醒可避免干擾干擾
- 速度：能夠快速吸引攻擊者，以停止攻擊

自動化、規模、雲端式解決方案為監測和回應策略的關鍵要點。 為了讓我們能夠以一些 Microsoft 線上服務規模有效地防範攻擊，我們的監控系統需要在接近即時的時間內自動產生高準確性的警示。 同樣地，當偵測到問題時，我們需要能夠以規模來緩解風險，我們無法依賴我們的團隊手動修正隨機器的問題。 為了降低風險規模，我們使用雲端式工具自動套用對策，並為工程師提供工具，以在整個環境中快速套用核准的緩解動作。

## <a name="how-do-microsoft-online-services-perform-security-monitoring"></a>Microsoft online services 如何執行安全性監控？

Microsoft online services 使用集中式記錄，針對可能表示安全性事件的活動，收集和分析記錄事件。 集中式記錄工具會匯總來自所有系統元件的記錄，包括事件記錄、應用程式記錄、存取控制記錄，以及網路型入侵偵測系統。 除了伺服器記錄和應用層級資料之外，核心基礎結構還配自自訂的安全代理程式，其會產生詳細遙測，並提供以主機為基礎的入侵偵測。 我們會使用此遙測進行監視和取證。

我們收集的記錄和遙測資料可啟用24/7 安全性警示。 我們的警示系統會在記錄資料上傳時分析資料，以幾乎即時的方式產生警示。 這包括以規則型的警示，和其它以機器學習模型為基礎的更複雜警示。 我們的監視邏輯超越一般攻擊案例，並納入對服務架構和作業的深層認知。 我們會分析安全性監控資料，以不斷改進模型，以偵測新類型的攻擊，並提高安全性監控的準確性。

## <a name="how-do-microsoft-online-services-respond-to-security-monitoring-alerts"></a>Microsoft online services 如何回應安全監控警示？

當觸發警示的安全性事件需要回應動作或進一步調查整個服務中的辨識證據時，我們的雲端式工具允許整個環境快速回應。 這些工具含有完全自動化的智慧型代理程式，可回應偵測到的威脅與安全性因應措施。 在許多情況下，這些代理程式會部署自動化因應措施，以在不需要人為介入的情況下大規模降低安全性偵測。 當您無法進行此回應時，安全性監控系統會自動提醒適當的通話工程師，其具備一組工具，可讓他們即時即時執行，以在規模範圍內緩解偵測到的威脅。 潛在的事件會升級至適當的 Microsoft 安全性回應小組，並使用安全性事件回應程式加以解決。

## <a name="how-do-microsoft-online-services-monitor-system-availability"></a>Microsoft online services 如何監視系統可用性？

Microsoft 積極監控其系統，以瞭解資源的使用狀況和反常使用方式。 資源監控是由服務冗余技術所結合，以協助避免意外停機，並讓客戶能夠可靠地存取產品和服務。 透過服務健康情況儀表板 (SHD) ，透過「服務健康情況」儀表板向客戶傳遞 Microsoft online 服務健康情況問題。

Azure 及 Dynamics 365 線上服務利用多種基礎結構服務來監視其安全性和健康情況可用性。 實施綜合交易 (STX) 測試，可讓 Azure 及 Dynamics service 檢查其服務的可用性。 STX 架構的設計是為了支援執行服務中元件的自動測試，並在即時網站失敗警示上進行測試。 此外，Azure 安全性監控 (ASM) 服務已經實施集中式綜合測試程式，以驗證安全性警示在新的和執行的服務中如預期的運作。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與安全性監控相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------|:--------|:------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.3：可用性監控與容量規劃 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.3：可用性監控與容量規劃 <br> 16.1：管理資訊安全性事件和增強功能 | 2020 年 12 月 2 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1：事件管理架構 <br> IM-2：事件偵測設定 <br> IM-3：事件管理程式 <br> IM-4：事件檢討後 <br> VM-1：安全性事件記錄及收集 <br> VM-12： Azure 服務可用性監控 <br> VM-4：惡意事件調查 <br> VM-6：安全弱點監控 | 2021 年 3 月 31 日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | IM-1：事件管理架構 <br> IM-2：事件偵測設定 <br> IM-3：事件管理程式 <br> IM-4：事件檢討後 <br> PI-2： Azure 入口網站 SLA 效能檢查 <br> VM-1：安全性事件記錄及收集 <br> VM-12： Azure 服務可用性監控 <br> VM-4：惡意事件調查 <br> VM-6：安全弱點監控 | 2021 年 3 月 31 日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------|:--------|:------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-2：帳戶管理 <br> AC-17：遠端存取 <br> AU-7：審核減少與報告產生 <br> SI-4：資訊系統監控 <br> SI-7：軟體、固件和資訊完整性 <br> | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> <br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.3：可用性監控與容量規劃 | 2021 年 4 月 20 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19：變更監控 <br> CA-26：安全性附隨報告 <br> CA-29：待命工程師 <br> CA-48：資料中心記錄 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-19：變更監控 <br> CA-26：安全性附隨報告 <br> CA-29：待命工程師 <br> CA-30：可用性監控 <br> CA-48：資料中心記錄 | 2020月24日 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-08：報告事件 <br> CUEC-10：服務合約 | 2020月24日 |

## <a name="resources"></a>資源

- [幕後運作：保護為 Microsoft 365 服務提供後援的基礎結構](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
