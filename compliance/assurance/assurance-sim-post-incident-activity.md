---
title: Microsoft 365 安全性事件管理：事件後活動
description: 本文概要說明 Microsoft 365 中的安全性事件管理後續事件處理常式。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 4ebd31c16f8abb3eddd6ed924a045d88597aba40
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51496717"
---
# <a name="microsoft-365-security-incident-management-post-incident-activity"></a>Microsoft 365 安全性事件管理：事件後活動

## <a name="postmortem"></a>死後

有些安全性事件，尤其是客戶影響或導致資料破壞的事件，會發生完整的事件總結。 Microsoft 365 安全性回應小組會針對安全性事件回應中的所有協力廠商，進行詳細總結：

- 記錄導致事件發生的事件順序
- 如已知) 所述，以包含違反違犯 (的演員所支援的證據，建立事件的技術摘要。 這項摘要會包含回應的執行方式和其他重要優點。
- 識別在安全性事件回應期間識別的技術停機、程式失敗、手動錯誤、程式缺陷和通訊不足，以及/或任何先前未知的攻擊媒介。

事後，您可以在 Microsoft 365 工程開發週期中設定新的優先順序，以直接影響 Microsoft 365 服務的改進、操作程式及檔。

## <a name="documentation"></a>文件

事後過程中的所有重要技術調查都會以錯誤或開發變更要求的形式，于報表和服務投資或修復中取得。 這些結果會遵循適當的工程團隊。 針對流程失敗及跨組織的問題，問題會記錄在 Microsoft 365 安全性回應小組的資料庫中，並遵循適當的群組來處理這些問題。

## <a name="process-improvement"></a>進程改進

回應 Microsoft 365 中的安全性事件，涉及與跨 Microsoft 不同組織的多個群組進行協調，以及可能的適當外部組織，例如法律強制執行。 我們知道，在每個安全性事件（sufficiency 及完整性）之後，評估我們的回應是很重要的。 針對任何已識別的改善或變更，Microsoft 365 安全性回應小組會評估與適當小組和專案關係人進行諮詢的建議，並在適當的情況下將其融入標準運作程式中。 在安全事件回應或事後活動中所識別的所有必要變更、bug 或服務改進都會在內部 Microsoft 365 工程資料庫中記錄及追蹤。 所有潛在的錯誤或功能會指派給適當的擁有者。 Microsoft 365 安全性回應小組會檢查所有專案，直到問題解決為止。

## <a name="related-articles"></a>相關文章

- [Microsoft 365 安全性中心事件管理](assurance-security-incident-management.md)
- [Microsoft 365 的安全性事件管理準備](assurance-sim-preparation.md)
- [Microsoft 365 安全性事件管理偵測和分析](assurance-sim-detection-analysis.md)
- [Microsoft 365 的安全性事件管理包容、eradication 及恢復](assurance-sim-containment-eradication-recovery.md)
