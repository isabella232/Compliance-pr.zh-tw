---
title: 資料中心安全性綜述
description: 深入瞭解 Microsoft 365 中的資料中心安全性
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: Admin
ms.topic: article
f1_keywords:
- ms.o365.cc.SupervisoryReview
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
ms.openlocfilehash: 52b8841f8d89571ea73fa469b05a776e0e0d3557
ms.sourcegitcommit: 186caf3b458d014f127bdf6e2d927c413276d9e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "49520120"
---
# <a name="datacenter-security-overview"></a>資料中心安全性綜述

## <a name="how-does-microsoft-host-its-online-services"></a>Microsoft 如何主控其線上服務？

Microsoft 提供超過200個雲端服務，包括企業服務，例如 Microsoft Azure、Microsoft 365 和 Microsoft Dynamics 365，客戶可以24x7x365 為客戶。 這些服務是由全域分散式資料中心、edge 計算節點和服務運作中心組成的 Microsoft 雲端基礎結構所主控。 它們受到世界上最大的全域網路的支援和連線，具有大量的纖程空間。

為雲端服務提供動力的資料中心，主要是高可靠性、卓越運作、成本效益、環境可持續性，以及全球客戶和合作夥伴的信任線上體驗。 Microsoft 會定期透過內部和協力廠商的審計來測試我們的資料中心安全性。 因此，世界上最高的高管制組織會信任 Microsoft 雲端，其與其他任何雲端服務提供者的憑證相容。

## <a name="how-does-microsoft-protect-its-datacenters-from-unauthorized-access"></a>Microsoft 如何保護資料中心不會遭到未經授權的存取？

存取實體資料中心設施的方式，會嚴格由外部和內部周邊伺服器控制，每個層級的安全性增加，包括周邊環境防護、安全性監察官、鎖定的伺服器機架、整合的告警系統、運作中心的全天候視頻監控，以及多重要素存取控制。 只有必要人員有權存取 Microsoft 資料中心。 在 Microsoft 資料中心內完全禁止邏輯存取 Microsoft 365 基礎結構（包括客戶資料）。

我們的安全性運作中心會使用影片監控和整合式電子存取控制系統來監視資料中心網站和設施。 攝像頭的位置已策略性，可提供有效的設施周邊、入口、運送期間、伺服器 cages、內部通道及其他機密安全性點。 在多重階層式安全性狀態中，由於整合安全性系統所偵測到的任何未經授權的進入嘗試，會為安全性人員產生警示，以立即回應和修正。

## <a name="how-does-microsoft-protect-its-datacenters-from-environmental-hazards"></a>Microsoft 如何保護其資料中心免受環境危險的危害？

Microsoft 採用各種保護措施，以防禦資料中心可用性的環境威脅。 已策略性選擇資料中心網站，以最大限度降低各種因素的風險，包括水災、地震、颶風和其他自然災難。 我們的資料中心使用氣候控制，針對人員、設備及硬體，監控及維護優化的可調空間。 消防偵測和抑制系統和水感應器可協助偵測和防範設備的火災和水源損毀。

災難無法預測，但 Microsoft 資料中心和作業人員準備災難，以提供作業的連續性，應發生意外的事件。 彈性架構及最新的測試連續性計畫減輕潛在的損毀，並促進資料中心作業的快速恢復。 危機管理計畫在危機之前、期間和之後，都能提供角色、責任和緩解活動的清晰性。 在這些方案中定義的角色和連絡人，有助於在危機情況下提升命令鏈的效率。

## <a name="how-does-microsoft-verify-the-effectiveness-of-datacenter-security"></a>Microsoft 如何驗證資料中心安全性的有效性？

我們瞭解，我們的客戶若要完全實現雲端的優點，他們必須能夠信任其雲端服務提供者。 我們的雲端服務基礎結構和套件是從頭開始，以滿足客戶嚴格的安全性和隱私權需求。 我們可協助我們的客戶遵循國內、地區和行業特定的需求，其可提供任何雲端服務提供者的一組最全面的相容性選項，以管理個人資料的收集和使用。

我們的雲端基礎結構和服務，都是一組廣泛的國際和行業特有的合規性標準，例如 ISO、HIPAA、FedRAMP 和 SOC，以及國家特定的標準，例如澳大利亞的 IRAP、英國的 G-雲端和新加坡的 MTCS。 嚴格，協力廠商審核會驗證我們遵循這些標準所規定的嚴格安全性控制。 您可以在 [Microsoft 服務信任入口網站](https://servicetrust.microsoft.com/)中取得我們資料中心基礎結構和雲端產品的審計報告。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以取得與資料中心安全性相關的控制項驗證。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|  
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | PE-2：實體存取授權 <br> PE-3：實體存取控制 <br> PE-6：監控實體存取 <br> PE-11：緊急電源 <br> PE-13：防火防護 <br> PE-14：溫度和濕度控制 <br> PE-15：水源損毀防護 | 2020年9月24日 |
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 11：實體和環境安全性 | 2020 年 2 月 22 日 |
| [ISO 27017 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 11：實體和環境安全性 | 2020 年 2 月 22 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b07c0f7b-6bd5-4544-8255-7a5f14bf914a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA-39：資料中心存取控制 <br> CA-40：資料中心網路驗證 <br> CA-41：資料中心雙因素驗證 <br> CA-48：資料中心記錄 | 2019 年 9 月 30 日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=fa062990-e758-4ddc-ace3-7fb21a301d09&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Rep-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA-39：資料中心存取控制 <br> CA-40：資料中心網路驗證 <br> CA-41：資料中心雙因素驗證 <br> CA-48：資料中心記錄 | 2019 年 9 月 30 日 |
