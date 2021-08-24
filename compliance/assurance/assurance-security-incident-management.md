---
title: Microsoft 安全性事件管理
description: 本文概要說明 Microsoft online services 中的安全性事件管理程式。
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
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: a35e6757d64dd0c2bffc1b1cbc62e23f524b8ac9
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481735"
---
# <a name="microsoft-security-incident-management"></a>Microsoft 安全性事件管理

Microsoft 致力於為 Microsoft 客戶提供高安全性的企業級服務，但是安全性事件是不可避免的現實，必須徹底且快速地加以管理。 這份檔概要說明 Microsoft 如何使用企圖和真正的方法及技術來處理安全性事件，以盡可能降低其潛在影響。 安全性事件指的是對儲存在 Microsoft 設備或 Microsoft 設施中客戶資料的任何非法存取，或未經授權存取客戶資料的遺失、披露或變更的設備或設施。 當回應安全性事件時，Microsoft 的目標是保護客戶資料和 Microsoft 的線上服務。

Microsoft online services 安全小組和各種服務小組共同運作，並且採用相同的安全性事件方法：

- 準備
- 偵測和分析
- 包容、Eradication 及恢復
- 事件後活動

## <a name="microsoft-approach-to-security-incident-management"></a>Microsoft 安全性事件管理方法

Microsoft 的管理安全性事件的方法，就是與 [國內的標準和技術研究院 (NIST) ](https://www.nist.gov/) 特殊出版物 (SP) 800-61。 Microsoft 有幾個專門的小組共同運作，以防止、監控、偵測及回應安全性事件。

|**團隊/區域**|**描述**|
|:------------|:--------------|
| Microsoft 安全回應中心 | 識別、監視、解決及回應安全性事件和 Microsoft 軟體安全性弱點。 |
| 網路防護作業中心 | 「網路防護作業中心」是透過整個公司的安全性回應小組和專家整合的實體位置，可協助即時保護、偵測及回應威脅。 |
| 公司、外部及法律事務 | 針對可疑的安全性事件，提供法律和法規的建議。 |
| Microsoft Datacenter Security 團隊 | 側重于常見安全性工程投資的各種服務，以保護、偵測和回應服務架構風險和威脅的團隊。 |
| Microsoft 安全性回應小組 | 與服務小組合作的獨立 Azure、Dynamics 365 及 Microsoft 365 安全小組，以建立適當的安全性事件管理程式，並推動任何安全性事件回應。 |
| GRC) 小組的 Microsoft 控管、風險和合規性 ( | 提供法規需求、規範和隱私權的指導方針。 |
| 服務小組 | Azure、Dynamics 365 Microsoft 365 的工程小組負責每項服務的安全性相關原則及決策。 |
| Azure operations manager | 監督 Azure 相關的安全性和隱私權事件的調查和解決方法。 |
| Microsoft 威脅情報中心 (MSTIC)  | 在 Microsoft 基礎結構和資產的數位安全性威脅中提供目前的 art 狀態、協助 Microsoft 內部的小組成員排定緩解與防護工作量行動計畫，以及透過接近即時事件監控/偵測來加強保護。 |
| 客戶經驗的通訊團隊 | 工程師小組負責安全性和服務事件的所有客戶通訊。 不同的小組專用於 Azure、Dynamics 365 和 Microsoft 365。 |

## <a name="response-management-process"></a>回應管理程式

Microsoft 線上服務安全性小組和服務小組共同運作，並對以 NIST 800-61 回應管理階段為基礎的安全性事件採取相同的做法：

- **準備**：指能夠進行回應的組織準備工作，包括工具、處理常式、稱職狀況和準備就緒。
- **偵測 & 分析**：指的是在實際執行環境中偵測安全性事件的活動，並分析所有事件，以確認安全性事件的真偽。
- **包容，eradication，** 復原：指的是根據上一個階段所做的分析所採取的安全性事件所需及適當的動作。 在此階段中，您也可能需要更多分析，以完全從安全性事件復原。
- **事件後活動**：指復原安全性事件之後所執行的檢討後分析。 在處理過程中所執行的作業動作會經過檢查，以判斷是否需要在準備或偵測和分析階段進行任何變更。

![安全性事件管理階段](../media/assurance-sim-phases.png)

## <a name="federated-security-response-model"></a>同盟安全性回應模型

Microsoft 線上服務是由 Microsoft 的核心產品所組成，包含 Azure、Dynamics 365 及 Microsoft 365。 每一項服務都是由不同的小組運作，其具有自己的安全性運作過程。 其他 Microsoft 的小組，例如 MSTIC，也會涉嫌從事 Microsoft 線上服務的各種安全性方面。 由於許多團隊都在處理所有組成 Microsoft online 服務的各種服務上進行安全性運作管理，所以 Microsoft 已實現同盟安全性回應模型。

此表格顯示各種 Microsoft 線上服務安全性運作小組和 Microsoft 服務小組之間的運作界限：

|**活動**|**Microsoft 安全小組作業**|**Microsoft 服務小組作業**|
|:-----------|:-----------------------------------------|:----------------------------------------|
| 偵測和分析 | -偵測需求 <br> -安全性監控和分析 <br> - (IOC) 掃描的安全指示器 <br> -違反搜尋 <br> -24x7 安全性待命和事件回應線索 | -偵測需求 <br> -監控基礎結構部署 <br> -服務分析和洞察力 <br> -事件和警示會審 <br> -24x7 服務工程待命  |
| 包容、eradication、恢復 | -事件回應線索 <br> -辯論調查 <br> -安全性專業知識與諮詢 <br> 修復指導 | -安全性事件擁有者 <br> -服務洞察力和專業知識 <br> -執行包容、eradication 及恢復 |
| 事件後活動 | -事件後分析線索 <br> -資料收集和封存 <br> -經驗教訓和 bug 要求 <br> -附隨報告 | -服務端事件分析 <br> -優先順序追蹤活動 <br> -實施安全性投資 <br> -服務安全性準備 |

## <a name="related-articles"></a>相關文章

- [Microsoft 安全性事件管理：準備](assurance-sim-preparation.md)
- [Microsoft 安全性事件管理：偵測和分析](assurance-sim-detection-analysis.md)
- [Microsoft 安全性事件管理：包容、eradication 及恢復](assurance-sim-containment-eradication-recovery.md)
- [Microsoft 安全性事件管理：事件後活動](assurance-sim-post-incident-activity.md)
