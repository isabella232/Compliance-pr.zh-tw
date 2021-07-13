---
title: Microsoft 安全性事件管理：包容、eradication 及恢復
description: 本文概要說明 Microsoft online services 中的安全性事件管理包容、eradication 及復原程式。
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
ms.openlocfilehash: 95e52107df2f3e745d393c62929f7c169bcf9a33
ms.sourcegitcommit: 8bf2602d56eedee4447ddb374ef95b0587f254e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53377550"
---
# <a name="microsoft-security-incident-management-containment-eradication-and-recovery"></a>Microsoft 安全性事件管理：包容、eradication 及恢復

根據安全性回應小組、服務小組和其他人員所執行的分析，開發適當的包容和復原計畫，以盡可能降低安全性事件的影響。 然後，適當的服務小組會在生產環境中套用此方案，並提供來自安全性回應小組的支援。

## <a name="containment"></a>遏制

在偵測到安全性事件後，必須先包含入侵，才可存取更多資源或造成更大的損毀。 我們的安全性事件回應程式的主要目標是限制對客戶或其資料的影響，或是對 Microsoft 系統、服務和應用程式的影響。

## <a name="eradication"></a>根除

Eradication 是以高信心程度消除安全性事件根本原因的處理常式。 目標是兩折的：

- 完全從環境逐出對手
- 若要緩解此弱點 (請注意，) 如果已啟用或可能讓敵人重新輸入環境。

根據事件性質、安全性事件範圍、滲透程度與可能影響程度的深度，安全性回應小組會建議服務小組採用 eradication 技巧。 考慮到此 eradication 步驟可能導致的潛在業務影響，當必要時) ，服務小組和安全性回應小組會進行必要的分析和核准，以 (。

## <a name="recovery"></a>恢復

隨著回應小組獲得合理的信賴程度，讓敵人從環境逐出，而且已消除所有已知可靠的路徑，個別的服務小組會啟動還原步驟，以將服務帶入已知且良好的設定。 這些還原步驟將會與安全性回應小組進行諮詢。 此活動包含識別服務的最後一個已知良好狀態，從備份還原至此狀態，檢查還原的狀態中有漏洞的攻擊路徑等等。與服務小組互動的安全性回應小組會決定環境可能的最佳復原計畫。

復原的一個重要方面是要有增強的 vigilance 和控制措施，以驗證復原計畫是否已順利執行，且環境中不存在遭到破壞的跡象。

## <a name="customer-notification-of-security-incident"></a>客戶安全性事件的通知

如果 Microsoft 決定發生安全性事件，我們會以不需要的延遲，以及我們同意的合約和規範中的規定來通知您。 在識別所有受影響的承租人之後，對應的通訊小組會運作，識別可能適用于受影響承租人的任何相關規章。 通訊小組使用適用的規章中所定義的適當通訊通道，以通知適當的承租人連絡人。

通知會包含有關該事件的詳細資訊，例如事件的描述、對客戶資料的影響、Microsoft 採取的動作，以及/或建議的動作，以供客戶用以解決問題並避免週期。 通知將會傳送至 Microsoft online services 租使用者的指定系統管理員 (s) 。 為了確保收到通知，您應該確保您的系統管理員在其租使用者設定檔中提供及維護準確的連絡人資訊。 此外，視事件性質而定，也可以透過[Microsoft 365 服務健康情況儀表板](http://status.yammer.com/)通知 Microsoft 365 的客戶。

## <a name="related-articles"></a>相關文章

- [Microsoft 安全性事件管理](assurance-security-incident-management.md)
- [Microsoft 安全性事件管理：準備](assurance-sim-preparation.md)
- [Microsoft 安全性事件管理：偵測和分析](assurance-sim-detection-analysis.md)
- [Microsoft 安全性事件管理：事件後活動](assurance-sim-post-incident-activity.md)
- [如何記錄安全性事件支援票證](/azure/security/fundamentals/event-support-ticket)
- [GDPR 規定的 Azure 和 Dynamics 365 外洩通知](/compliance/regulatory/gdpr-breach-azure-dynamics)
