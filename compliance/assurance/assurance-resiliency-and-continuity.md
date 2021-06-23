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
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 9ac4a87670d1889e9c74e5ec6afe8920b96946fc
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088772"
---
# <a name="resiliency-and-continuity-overview"></a>復原和連續性概觀

## <a name="how-does-microsoft-ensure-business-continuity-in-the-case-of-a-disaster-or-other-threat-to-service-availability"></a>在發生嚴重損壞或其他威脅以進行服務可用性時，Microsoft 如何保證業務連續性？

Microsoft 的 Enterprise 商務持續性管理 (EBCM) 小組監督整個 Microsoft 服務和雲端方案中的業務持續性管理和嚴重損壞修復活動。 Microsoft 商務單位的代表，例如 Microsoft 365，與 EBCM 小組合作，以開發業務持續性計畫，並驗證業務持續性需求。

在我們的業務持續性管理 (BCM) 方法是 BCM 生命週期的核心。 這三個階段的程式設計為可重新提供，所以可透過 Microsoft 的各種業務模型實施。 它會從 **評估** 階段開始，以識別應包含在商務持續性計畫中的重要程式和目標。 評估階段也需要 (BIA) 的「業務影響分析」。 **規劃** 階段著重于開發及實施修復原則，以及將其記錄在正式的商務持續性計畫中。 最後， **功能驗證** 會測試業務持續性計畫及其實施，以驗證有效性並識別可能的增強功能。

Microsoft 365 的業務持續性策略會利用硬體、網路及資料中心冗余。 資料中心之間的資料複寫提供高可用性和可靠性，以防發生嚴重的事件。 這種方式也會提升對諸如隔離硬體故障或資料損毀等常見事件的復原能力。

## <a name="how-does-microsoft-test-business-continuity-and-disaster-recovery-plans"></a>Microsoft 如何測試商務持續性和嚴重損壞修復計畫？

microsoft 的 Enterprise 商務持續性管理 (EBCM) 原則 stipulates，所有的 microsoft 商務持續性和嚴重損壞修復方案都必須每年測試、更新及複習。 Microsoft 365 服務每年至少每個 EBCM 原則測試其業務持續性計畫。 在建立並檢查動作報告以驗證、測試結果並通知計畫更新，以回應測試期間發現的任何問題。

為了針對多種潛在的事件驗證修復原則，EBCM 程式會定義多個類別的測試案例，以影響人員、地點及技術。 每項服務所需的驗證層級取決於服務的重要程度，更重要的是服務會收到更嚴格的驗證。 每個 Microsoft 365 服務小組都會根據 EBCM 指導方針來測試其業務持續性計畫，以衡量方案的效能，以及服務小組是否準備好執行計畫。

根據 EBCM 指導方針，商務持續性計畫和功能驗證的年度評論必須在最後一次複查的12個月內進行。 功能驗證必須包含支援檔（如 BIA）的審查，以確保其保持正確。 Microsoft 會透過每季報告，讓客戶選取 Microsoft 365 服務可使用的功能驗證結果。

## <a name="how-does-microsoft-365-ensure-system-capacity-meets-demand"></a>Microsoft 365 如何確保系統容量符合需求？

容量規劃可協助服務小組指派支援 Microsoft 365 服務可用性所需的資源。 一般的容量規劃是 Microsoft 的 EBCM 程式所需的一部分。 服務小組會在每季檢查期間檢查容量資料，以及在緊急情況下進行額外的容量檢查。

容量規劃的原始資料是由每個服務小組所維護，並包含系統處理、記憶體和硬體容量等標準。 排程的評論使用系統目前容量的模型，並根據緊急狀況狀況的計畫需求進行測試。 如果模型指出容量缺口，系統容量的建議變更會送出至服務小組領導，以供審查。 已核准的變更新增至新的模型，然後由服務小組工程師執行。

## <a name="how-does-microsoft-365-maintain-service-availability-during-routine-system-failures"></a>Microsoft 365 如何在例行系統失敗期間維護服務可用性？

Microsoft 365 透過冗余架構、資料複寫及自動完整性檢查，達到服務恢復能力。 冗余架構包括在地理位置和實際獨立的硬體上部署服務的多個實例，為 Microsoft 365 服務提供更高的容錯能力。 資料複寫可確保不同的容錯區域中永遠有多個客戶資料複本，允許在客戶損毀、遺失甚至意外刪除時，復原重要的客戶資料。 自動完整性檢查會透過自動還原由許多實體或邏輯損毀所影響的資料，提高資料可用性。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與恢復性及連續性相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | CP-2：應變計劃 <br> CP-3：應急訓練 <br> CP-4：應變計劃測試 <br> CP-6：替代儲存位置 <br> CP-7：備用處理網站 <br> CP-9：資訊系統備份 <br> CP-10：資訊系統復原和 reconstitution | 2020年9月24日 |
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 17.1：資訊安全性持續性 <br> 17.2：冗余 | 2021 年 4 月 20 日 |
| [ISO 22301 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=13951eb3-6339-4629-b80d-dd0d43812fe7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=2bb29cc0-53e7-4a53-a9de-871316e1b80c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 所有控制項 | 2019 年 3 月 18 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49：備份原則 <br> CA-50：商務持續性 <br> CA-51：資料複寫 | 2020月24日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-49：備份原則 <br> CA-50：商務持續性 <br> CA-51：資料複寫 | 2020月24日 |
| [SOC 3 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=274054e5-4968-48d2-bf94-9a8eda5d7a93&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CUEC-09： EXO 電子郵件還原 | 2020月24日 |

## <a name="resources"></a>資源

- [Microsoft Enterprise 商務持續性管理計畫白皮書](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=64f922a6-d624-40dd-a8ae-6f996b5186f3&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f) 
- [Microsoft Cloud EBCM and 災難修復計畫驗證報告： FY21 Q3](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=c072d11c-9cc9-42e1-b1cf-7281572fb1dd&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_FAQ_and_White_Papers)

## <a name="legal-disclaimer"></a>法律免責聲明

- [企業業務連續性法律免責聲明](assurance-ebcm-legal-disclaimer.md)