---
title: 資料中心商務持續性和嚴重損壞修復
description: 深入瞭解 Microsoft datacenter business 連續性和嚴重損壞修復。
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
ms.openlocfilehash: 948e1f9e1b15b83817c072e63ffaae0b444445f8
ms.sourcegitcommit: cf424cb1e7c12048120977f294f780b776119a96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/11/2021
ms.locfileid: "60265088"
---
# <a name="datacenter-business-continuity-and-disaster-recovery"></a>資料中心商務持續性和嚴重損壞修復

我們無法預測災害，但 Microsoft 資料中心和營運人員會為災害做好準備，以在突發事件發生時，持續提供作業。 復原性結構和最新測試的持續性計劃可降低潛在損害，並有助於資料中心作業的迅速復原。 危機管理計畫在危機之前、期間和之後，會明確説明角色、責任和緩解活動。 這些計畫中定義的角色和連絡人，會在危機的情況下促進事件在命令鏈上有效地升級。

## <a name="business-resilience"></a>企業復原性

在 Microsoft 雲端運作及創新 (共同 + I) 商務持續性計畫中，需要資料中心來測試持續作業，並回應危機事件。 每個 Microsoft 受管理的資料中心都有自己的商務持續性計畫，其建立方式是使用來自共同 + I 韌性中心卓越和資料中心作業的主要主題知識，以確保網站特有的內容考慮到應急準備。 這些計畫會針對不同的嚴重損壞案例，描述角色、責任、人員安全程式、通知準則、升級步驟及檢查清單。

Microsoft 的共同 + I 組織的恢復功能是由 Enterprise 商務持續性管理計畫來控制，並遵循 Enterprise 原則和標準。 商務持續性委員會、部門領導，以及最終 Microsoft 資深領導團隊會定期審查計畫的效能。

## <a name="crisis-management-and-pandemic-response"></a>危機管理和疫情回應

對於一家全球均有業務的公司來説，危機管理計畫是 Microsoft 回應重大事件不可或缺的一部分。 Microsoft 的資料中心危機管理計畫以產業的最佳作法為基礎，並包含重要元件以允許透過策略性的方式回應重大事件。 此外，CO + I 韌性 Center 已開發，並繼續維護 Pandemic 及 Infectious 疾病計畫，以用於回應可能具有操作影響的 Infectious 疾病。 在我們的 pandemic 回應中，恢復性支援小組會將重要且及時的當地疾病情報，提供給 Redmond 的 Microsoft 領導，以協助實施綜合性的緩解策略。

Microsoft 已建立組織的 Enterprise 商務持續性管理 (EBCM) 架構，其充當整個公司的業務連續性計畫指導方針。 此方案包括商務持續性原則、實施指導方針、業務影響分析 (BIA) 、風險評估、相依性分析，以及監控和改善程式的程式。 Enterprise恢復能力 Office 管理跨 Microsoft 的控管和效能報告。 共同處理 + I 恢復性計畫是透過共同 + I 恢復性中心進行協調，以確保程式遵循一致的長期設想和使命，並符合企業計畫標準、方法、原則及度量標準。 CO + I 適應性中心卓越，已確立一系列的標準，可為共同 + I 組織提供額外的管理。

共同 + I 技術恢復計畫 (TRPs) 適用于從高嚴重性事件或災難復原的各種工程群組，以協助確保重要的技術仍可供使用。

Business 韌性計畫 (BRP) 和 TRP 包含服務、還原程式及與事件管理小組進行通訊的範圍和適用的相依性。 BRP 和 TRP 的每一年，都是由專屬的計畫擁有者及所有適用的使用者提供，至少一年取得及核准。 根據定義的測試排程，以適用的標準來測試方案。

## <a name="resiliency-program"></a>復原計畫

Microsoft 已定義 BRP，做為在嚴重不利事件期間回應、復原及繼續作業的指南。 BRP 涵蓋繼續重要業務程式和作業所需的主要人員、資源、服務和動作。 BRP 的開發是以 Microsoft Enterprise 恢復 Office 的建議指導方針為基礎。

在此方案的範圍內，是 Microsoft 重要的商務程式，在24小時以內或更少的需要定義。 這些程式是在 BIA 期間決定的，在這種情況下，Microsoft 估計的潛在運作和財務影響是因為它們無法執行程式並決定恢復時間目標 (RTO) 和復原點目標 (RPO) 。 在 BIA 之後，會執行非技術相依性分析，以判斷執行程式所需的特定人員、應用程式、重要記錄和使用者需求。

Microsoft 會定期測試 BRP，以評估其效能、可用性，以及找出風險可以消除或緩解的地方。 適用時，如果有相關聯的相依性，協力廠商會參與測試。 測試的結果會以適當的人員記載、驗證、核准。 此資訊可用來建立工作專案並設定其優先順序。

## <a name="datacenter-resilience-program"></a>資料中心恢復計畫

作為資料中心恢復計畫的一部分，共同運作的卓越小組的共同 + I 韌性中心會開發出解決組織之商務持續性所需之資訊安全性需求的方法、原則及度量。 當發生中斷時，小組會為重要的處理常式及必要資源開發 TRPs。
