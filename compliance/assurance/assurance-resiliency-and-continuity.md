---
title: 復原和連續性
description: 深入瞭解 Microsoft 365 中的恢復能力與連續性
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
ms.openlocfilehash: ff1719ce931a50904fb6b7e6069cd29a1883aa90
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947177"
---
# <a name="resiliency-and-continuity-overview"></a>復原和連續性概觀

## <a name="how-does-microsoft-ensure-business-continuity-if-a-disaster-or-other-threat-to-service-availability-occurs"></a>當發生嚴重損壞或其他威脅以進行服務可用性時，Microsoft 會如何保證業務連續性？

Microsoft 的 Enterprise 商務持續性管理 (EBCM) 小組監督整個 Microsoft 服務和雲端方案中的業務持續性管理和嚴重損壞修復活動。 Microsoft 商務單位與 EBCM 小組合作，以開發業務持續性計畫，並驗證業務持續性需求。

商務持續性管理 (BCM) 生命週期是我們的 BCM 方法的核心。 這三個階段的程式設計為可重新提供，所以可透過 Microsoft 的各種業務模型實施。 它會從 **評估** 階段開始，以識別應包含在商務持續性計畫中的重要程式和目標。 評估階段也需要 (BIA) 的「業務影響分析」。 **規劃** 階段著重于開發及實施修復原則，並在官方商務持續性計畫中記錄這些策略。 最後， **功能驗證** 會測試業務持續性計畫及其實施，以驗證有效性並識別可能的增強功能。

Microsoft online services 業務持續性策略會使用硬體、網路及資料中心冗余。 資料中心之間的資料複寫提供嚴重的事件時的高可用性和可靠性。 這種方式也會提升對諸如隔離硬體故障或資料損毀等常見事件的復原能力。

## <a name="how-does-microsoft-test-business-continuity-and-disaster-recovery-plans"></a>Microsoft 如何測試商務持續性和嚴重損壞修復計畫？

microsoft 的 Enterprise 商務持續性管理 (EBCM) 原則 stipulates，所有的 microsoft 商務持續性和嚴重損壞修復方案都必須每年測試、更新及複習。 Microsoft online services 每年至少會測試其業務持續性計畫。 EBCM 原則。 在建立並檢查動作報告以驗證、測試結果並通知計畫更新，以回應測試期間發現的任何問題。

為了針對各種潛在事件驗證復原性和復原策略，EBCM 計劃定義了影響人員、位置和技術的多個測試案例類別。 每個服務所需的驗證層級都是以服務的重要性為基礎，而比較重要的服務會收到更嚴格的驗證。 每個 Microsoft online 服務小組都會根據 EBCM 指導方針來測試其業務持續性計畫，以衡量方案的效能，以及服務小組是否準備好執行計畫。

根據 EBCM 指導方針，商務持續性計畫和功能驗證的年度評論必須在最後一次複查的12個月內進行。 功能驗證必須包含支援檔（如 BIA）的審查，以確保其保持正確。 Microsoft 會透過每季報告，讓客戶選擇可使用的 Microsoft online 服務的功能驗證結果。

## <a name="how-do-microsoft-online-services-ensure-system-capacity-meets-demand"></a>Microsoft 線上服務如何確保系統容量符合需求？

容量規劃可協助服務小組指派必要的資源，以支援 Microsoft 線上服務可用性。 Microsoft 的 EBCM 計劃需要一般容量規劃。 服務小組會在每季檢查期間和緊急狀況的情況下，查看容量資料，同時又可獲得更多的容量。

容量規劃的原始資料是由每個服務小組所維護，並包含系統處理、記憶體和硬體容量等標準。 排定的審查會使用系統目前容量的模型，並針對緊急情況下的預計需求進行測試。 如果模型指出容量缺口，則會將系統容量的提議變更提交給服務小組領導階層進行審查。 在服務小組工程師實作之前，核准的變更會併入新模型中。

## <a name="how-do-microsoft-online-services-maintain-service-availability-during-routine-system-failures"></a>Microsoft online services 如何在例行系統失敗期間維護服務可用性？

Microsoft 線上服務透過冗余架構、資料複寫及自動完整性檢查，以達到服務恢復能力。 重複架構包括在地理位置和實際獨立的硬體上部署服務的多個實例，為 Microsoft 線上服務提供更高的容錯能力。 資料複寫可確保不同的容錯區域中永遠有多個客戶資料複本，允許在客戶損毀、遺失甚至意外刪除時，復原重要的客戶資料。 自動完整性檢查會透過自動還原由許多實體或邏輯損毀所影響的資料，提高資料可用性。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與恢復性及連續性相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 17.1：資訊安全性持續性 <br> 17.2：冗余 | 2020 年 12 月 2 日 |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=6d388547-fc88-46e3-8de2-6bc2edc08b06&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=ee4b611b-bb4d-4056-b189-00da36e88949&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 所有控制項 | 2020年5月13日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | BC-1：商務持續性計畫 <br> BC-3：商務持續性和嚴重損壞修復程式 <br> BC-4： BCDR 測試 <br> BC-7：資料中心商務持續性計畫 <br> BC-8：資料中心商務持續性測試 <br> BC-9：資料中心恢復性評估 <br> DS-5：備份金鑰服務元件 <br> DS-6：重要元件的冗余 <br> DS-7：自動複寫客戶資料 <br> DS-8：備份排程 <br> DS-9：備份還原程式 <br> DS-11：異地備份 <br> DS-14：自動還原客戶服務 | 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | CP-2：應變計劃 <br> CP-3：應急訓練 <br> CP-4：應變計劃測試 <br> CP-6：替代儲存位置 <br> CP-7：備用處理網站 <br> CP-9：資訊系統備份 <br> CP-10：資訊系統復原和 reconstitution | 2020年9月24日 |
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 17.1：資訊安全性持續性 <br> 17.2：冗余 | 2021 年 4 月 20 日 |
| [ISO 22301](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=13951eb3-6339-4629-b80d-dd0d43812fe7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 所有控制項 | 2019 年 3 月 18 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49：備份原則 <br> CA-50：商務持續性 <br> CA-51：資料複寫 | 2020月24日 |
| [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-09： EXO 電子郵件還原 | 2020月24日 |

## <a name="resources"></a>資源

- [Microsoft Enterprise 商務持續性管理計畫白皮書](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=64f922a6-d624-40dd-a8ae-6f996b5186f3&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f)
- [Microsoft Cloud EBCM and 嚴重損壞修復計畫驗證報告： FY21 Q4](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=83dc940a-2078-4e14-8b7d-07128e5b453d&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## <a name="legal-disclaimer"></a>法律免責聲明

- [企業業務連續性法律免責聲明](assurance-ebcm-legal-disclaimer.md)