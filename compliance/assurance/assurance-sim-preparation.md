---
title: Microsoft 365 安全性事件管理：準備
description: 本文概要說明 Microsoft 365 中的安全性事件管理準備程式。
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
ms.openlocfilehash: b3f16620564d525245c21c375bbc9a3f5b0923b7
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497393"
---
# <a name="microsoft-365-security-incident-management-preparation"></a>Microsoft 365 安全性事件管理：準備

## <a name="training-and-background-checks"></a>訓練和背景檢查

在 Microsoft 365 上運作的每一名員工都會提供相關的安全性事件和回應程式的訓練，以符合他們的角色。 每個 Microsoft 365 員工會在加入時收到訓練，並在此後每年會收到一年複習訓練。 訓練的設計目的是讓員工能夠基本瞭解 Microsoft 的安全性方法，讓您在訓練完成訓練時，所有員工都會瞭解：

- 安全性事件的定義
- 所有員工報告安全性事件的責任
- 如何將潛在的安全性事件提升至 Microsoft 365 的安全性回應小組
- Microsoft 365 安全性事件回應小組如何回應安全性事件
- 有關隱私權的特殊考慮（特別是客戶隱私權）
- 哪裡可以找到安全性和隱私權的其他資訊，以及上報連絡人
- 任何其他相關的安全性區域會 (必要) 

適當的員工會每年于安全性接收復習訓練。 年度複習訓練著重于：

- 對前一年的標準作業程式所做的任何變更
- 所有人都要報告安全性事件，以及如何執行此動作
- 哪裡可以找到安全性和隱私權的其他資訊，以及上報連絡人
- 每年可能會相關的任何其他安全性重點領域

在 Microsoft 365 上運作的每一個員工也都會經歷適當且徹底的背景檢查，其中包含候選人的教育、雇傭、民事歷程記錄，以及其他美國法規（如健康保險業便攜性和責任法案）的特定資訊 (，例如健康保險業便攜性和責任法案 (HIPAA) 、) 的管理計畫 (FedRAMP) ，以及其他人員。

在 Microsoft 365 工程中執行的所有員工都必須使用背景檢查。 有些 Microsoft 365 環境和操作員角色可能也需要完整的指紋、公民需求、政府的淨空需求，以及其他更為嚴格的控制。 此外，有些服務小組和角色可能會視需要經過特殊的安全性訓練。 最後，安全性小組成員自行取得與安全性直接相關的專業訓練和會議參與。 這項訓練會因小組和員工的需求而異，但包括行業會議、內部 Microsoft 安全性會議，以及透過行業中知名的安全性訓練廠商進行的外部訓練課程等事項。 我們也會針對 Microsoft 的安全性群組，定期發佈整個年度的專門安全性訓練文章，並定期專用於 Microsoft 365。

## <a name="penetration-testing--assessment"></a>& 評估的滲透測試

Microsoft 與各種行業的團體及安全性專家合作，以瞭解新的威脅及不斷演化的趨勢。 Microsoft 會持續評估其自身的系統是否有弱點，以及具有相同之獨立外部專家的合約。

在 Microsoft 365 內執行服務強化的測試可以分為四個一般類別：

1. **自動化的安全性測試：** 內部和外部人員會定期掃描 Microsoft 365 環境，依 Microsoft SDL 的做法、開放式 Web 應用程式安全性專案 (OWASP) 前10個風險，以及不同的行業主體所報告的新威脅。
2. **弱點評估：** 使用獨立的協力廠商測試人員的正式服務，會定期驗證重要邏輯控制項是否運作有效，以履行各種規章主體的服務義務。 評估是由已註冊之道德安全性測試人員 (CREST) 認證的人員所進行，並以 OWASP 前10個風險和其他服務適用的威脅為基礎。 所有找到的威脅都會追蹤以結束。
3. **連續的系統弱點測試：** Microsoft 會執行定期測試，讓小組企圖利用新興威脅、混合威脅和/或高級威脅來破壞系統，而其他小組則嘗試封鎖遭到破壞的企圖。
4. **Microsoft Online Services 臭蟲 Bounty 程式**：此程式會運作原則，以允許在 Microsoft 365 上受到限制的用戶端安全性漏洞評估。 如需詳細資訊，請參閱 [Microsoft Online Services 錯誤 Bounty 字詞](https://www.microsoft.com/msrc/bounty-terms)。

Microsoft 365 工程小組會定期發佈各種規範檔。 在[Microsoft 雲端服務信任入口網站](https://aka.ms/STP)，或從[microsoft 365 規範中心](https://compliance.office.com)的服務保證區域中，可提供這些檔中的數個。

>[!NOTE]
>如需如何存取服務信任入口網站的詳細資訊，請參閱使用 Office 365 for business，Azure 及 Dynamics CRM Online 訂閱的服務信任入口網站入門。 若要存取 Microsoft 365 規範中心，必須使用 Microsoft 365 訂閱。

## <a name="attack-simulation"></a>攻擊模擬

Microsoft 參與了我們的安全性和回應方案，並有意圖改進偵測和回應功能的安全性和回應方案，以進行即時的攻擊類比和即時網站滲透測試。 Microsoft 會定期模擬實際行為、進行連續的安全性監控，並實行安全性事件回應，以驗證及提高 Microsoft 365 和 Azure 的安全性。

Microsoft 會執行使用兩個核心小組的假設安全性原則：

### <a name="red-teams"></a>紅色小組

Microsoft 365 安全紅色小組是 Microsoft 的全職員工群組，側重于 breaching Microsoft 的基礎結構、平臺及 Microsoft 自有的承租人和應用程式。 它們是一組道德駭客 (的專屬入侵者) 針對線上服務執行目標和持續攻擊 (但不是客戶應用程式或資料) 。 它們提供連續的「完整頻譜」驗證 (例如，技術控制、紙張原則、人力回應等服務事件回應功能 ) 。

### <a name="blue-teams"></a>藍色團隊

Microsoft 365 安全性藍色小組是由一組專屬的安全性回應程式和成員，由安全事件回應、工程及作業小組組成。 它們是獨立的，且與紅色小組分開運作。 藍色小組遵循已建立的安全性程式，並使用最新的工具和技術，偵測並回應攻擊和滲透嘗試。 就像現實世界的攻擊，藍色小組不知道紅色小組的攻擊發生的時間或方式，或可能使用哪些方法。 其工作不論是紅色小組攻擊或是實際 assault，都是偵測並回應所有的安全性事件。 基於這個理由，藍色的團隊會持續通話，而且必須回應紅色小組遭到破壞的方式與其他任何對手相同。

Microsoft 員工會將全時紅色小組和藍色小組分開，各部門的各項作業都執行跨服務和兩者之間的作業。 稱為 *紅色分組*，方法是使用與即時生產基礎結構不同的戰術、技術和程式，在 Microsoft 服務的系統和作業之間進行測試，而不需要基礎結構和平臺工程或作業小組的 foreknowledge。 這會測試安全性偵測和回應功能，並以可控的方式協助識別實際執行的漏洞、設定錯誤、假設或其他安全性問題。 每個紅色小組遭到破壞後，就會在紅色小組和藍色小組之間完全披露（包括服務小組），以找出差距、解決發現的情況，並大幅改善破壞性回應。

>[!NOTE]
>在紅色的組合或即時網站滲透練習中，不會為客戶資料設定目標。 測試是針對 Microsoft 365 和 Azure 基礎結構和平臺，以及 Microsoft 自有的承租人、應用程式和資料。 客戶租使用者、Microsoft 365 或 Azure 所裝載的應用程式和資料，永遠不會以合約的合約為合約規定目標。

### <a name="joint-exercises"></a>共同運動

在不同的情況下，Microsoft 365 Security Blue 和 Red 小組會執行共同作業，在作業期間的關聯性比每個小組的一組員工的 adversarial 更多。 透過道德駭客和回應程式之間的即時共同作業，小組之間的這些運動可共同進行協調，以促進更有針對性的結果集。 這些「紫色小組」練習對每個作業都具有極高的針對性，以最大化機遇，但是每個作業的基礎是高頻寬資訊共用和合作，以達成目標。

## <a name="related-articles"></a>相關文章

- [Microsoft 365 安全性中心事件管理](assurance-security-incident-management.md)
- [Microsoft 365 安全性事件管理偵測和分析](assurance-sim-detection-analysis.md)
- [Microsoft 365 的安全性事件管理包容、eradication 及恢復](assurance-sim-containment-eradication-recovery.md)
- [Microsoft 365 安全性事件管理後置事件活動](assurance-sim-post-incident-activity.md)
