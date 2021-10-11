---
title: 資料中心環境保護
description: 深入瞭解 Microsoft datacenter 環境保護。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 525aab55d3f56490ecd1f1da1e00d6c5ddd32dc4
ms.sourcegitcommit: cf424cb1e7c12048120977f294f780b776119a96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/11/2021
ms.locfileid: "60265091"
---
# <a name="datacenter-environmental-safeguards"></a>資料中心環境保護

Microsoft 採用各種保護措施，以防範資料中心可用性的環境威脅。 這些保護功能可讓 Microsoft 提供客戶所信任的安全且可用的雲端平臺。

## <a name="site-selection"></a>網站選取

要保護 Microsoft 資料中心不受環境危害，應從選取網站開始。 在選取資料中心結構之前，Microsoft 資料中心位置會經歷嚴格的評估。 已策略性選擇 Microsoft datacenter 網站，以最大限度降低風險，包括水災、地震、颶風和其他自然災難。 除了盡可能降低環境風險以外，資料中心選址的關鍵因素還包括低成本能源和可靠的電信基礎設施。

## <a name="climate-control"></a>氣候控制

氣候控制是資料中心內重要基礎設施的基本元件，用以監視和維護員工與設備/硬體的最佳化條件空間。 熱負載 (作為能源消耗的副產物) 和濕度皆需妥善管理，以確保可透過機械干預符合適當的操作條件。 當地氣候條件、各種法規需求和條件限制，將決定達到此目標的最有效方式。

溫度和濕度層級會依照每個資料中心預期的 IT 硬體環境需求進行維護。 Microsoft 資料中心與客戶保持運作層級合約，這樣就能在維護最低環境需求的情況下達到最佳效能。 資料中心的大樓管理系統 (BMS) ，可持續監控溫度和濕度層級。 關鍵環境 (CE) 小組成員會從「設施運作中心」 (FOC) 中監控 BMS，讓他們在任何告警點超出之前管理資料中心內的溫度和濕度。 BMS 已設定為在到達某些標記時通知 CE 小組，然後調查並進行調整以修正氣候問題。 溫度和濕度可接受的範圍與 Refrigerating 及空調 (工程師的美洲協會，都是一致的) 指導方針或類似本機適用的指導方針。 資料中心濕度是以相對濕度百分比為單位，在 40%-55% 之間的目前範圍內，以非冷凝。 溫度範圍通常介於18攝氏度和27攝氏度之間 (介於64.4 華氏度和80.6 華氏度) 之間。

## <a name="fire-and-water-damage-protection"></a>火災與水毀損防護

Microsoft 在每個資料中心設施內均採用最新式的火災偵測和滅火系統。 獨立的能源來源支援消防防護系統，以確保在有火災時，保護 Microsoft 員工和基礎結構。 資料中心設施還會在被認為有漏水風險的區域設置浸水感測器，以防護水災損害。 發生與水有關的緊急情況時，這些水感應器會快速通知適當的人員。 水開關閥設計成便於操作，且員工皆依據其作業和所在位置受過訓練。

Microsoft 資料中心會執行強健的消防偵測機制，包括在地面和天花板上安裝的 photoelectric 冒煙 detectors、Xtralis 非常初期的冒煙偵測儀器 (VESDA) 每個 colocation 中的系統、在整個資料中心內安裝的，以及在整個資料中心內每隔八小時，安全性人員 extinguishers 在所有大樓區域中的每一小時，安全性人員巡邏隊在所有大樓區域 而且，防火/抑制和緊急照明系統會連接到提供冗余電源來源的資料中心備份電源系統。 包含機密電氣裝置的區域會受到雙聯鎖巨集指令的保護， (幹管道) sprinkler 系統。

CE 小組會執行每日網站逐步 (DSWT) ，檢查每個會議室及其中許多元件元件，以確保符合所有的防火觀賞需求。

Microsoft 會為自動啟動的資訊系統使用防火偵測裝置/系統，並在發生火災時通知資料中心人員和緊急回應程式。 如果其中一個消防偵測機制在任何 colocation 空間中啟動，則系統會自動通知華盛頓州的本地防火部門和全域安全性作業中心。 防火 protection 和偵測系統會與安全性系統捆綁在一起，以通知本機的功能和安全性人員。

Microsoft 在有水不足風險的區域中提供水/洩漏偵測。 防火抑制系統也會有受到監控的洩漏偵測告警。 水/洩漏偵測系統會與設施告警和通知系統整合，並將資料中心內的 sprinkler 系統進行分區。 CE 和資料中心管理小組已熟悉需要使用水線閥和其位置的緊急程式。 Sprinkler riser 卡可以個別或透過門閥加以關閉，也可以是群組。 Sprinklers 中的所有 sprinklers 都是雙聯鎖動作類型，在開始流程之前需要兩種形式的啟用。 監視 sprinkler 系統的壓力，並對水洩漏發出警報。

## <a name="health-and-safety"></a>健康與安全

對 Microsoft 員工健康情況和安全性的承諾，都是衡量成功程度的基礎。 Microsoft 資料中心會依照本機、地區、國內和聯邦健康情況和安全性規定運作。 在大多數情況下，Microsoft 健康和安全性原則會超越政府和法規需求，以確保在資料中心生命週期的所有階段（從構造到解除委任）期間，對所有資料中心工作者的健康情況、安全性和 wellbeing 進行保護。 安全管理計畫、風險評估、高風險活動管理及安全性訓練都是核心原則，可為所有員工提供安全的工作環境。

## <a name="energy-efficiency"></a>能源效率

Microsoft 自 2012 年起營運即達到碳中和。 在2030的情況下，Microsoft 將會以負數和2050為單位，已從環境中移除公司所有的碳是由公司直接發出，或是因為其成立于1975。 在2025中，Microsoft 資料中心將會以100% 的 renewable 能量提供。 為了達成這專案標，Microsoft 已針對綠色能量實施了合約工具（如 proxy 產生電源購買協定），以提供所有資料中心消耗的100% 的碳電電量。
