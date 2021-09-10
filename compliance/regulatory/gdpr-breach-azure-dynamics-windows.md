---
title: GDPR 規定的 Azure、Dynamics 365 和 Windows 外洩通知
description: Azure 和 Dynamics 365 如何防止個人資料外洩，以及若發生外洩 Microsoft 會如何回應和通知您。
keywords: Azure, Microsoft 365, Dynamics 365, Microsoft 365 文件, GDPR
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft GDPR
hideEdit: true
ms.openlocfilehash: 23d6b1ebb30f34fcb549e3e1f44c98a0c0e11b12
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947738"
---
# <a name="azure-dynamics-365-and-windows-breach-notification-under-the-gdpr"></a>GDPR 規定的 Azure、Dynamics 365 和 Windows 外洩通知

Microsoft 十分重視歐盟一般資料保護規範 (GDPR) 所規定的義務。Microsoft 在其線上服務中採取了廣泛的安全性措施，以防範資料外洩的威脅。這包含實體和邏輯兩方面的安全性控制，和自動化的安全性程序、全面性的資訊安全與隱私權原則，以及所有人員的安全性與隱私權教育訓練。

從一開始 Microsoft Azure 內就已內建各種安全機制，首先是[安全性開發週期](https://www.microsoft.com/sdl/)這項強制性開發程序，結合了「從設計著手保護隱私」和「預設為保護隱私」的方法。Microsoft 安全性策略的最高指導原則是「假設已有缺口」，這是深度防禦策略的延伸。不斷挑戰 Azure 的安全性功能，Microsoft 才能先發制人，對抗接踵而來的新威脅。如需有關 Azure 安全性的詳細資訊，請參閱以下[資源](https://www.microsoft.com/trustcenter/security/azure-security)。

Microsoft 設有遍布全球的全天候事故回應服務，努力減少針對 Microsoft Azure 的攻擊所造成的影響。Microsoft 在資料中心採用了極為嚴密的作業和程序，以避免未經授權的存取，包括全天候的視訊監控、訓練精良的安全人員、智慧卡和生物特徵辨識控制等，通過多重安全性與合規性稽核 (例如 [ISO/IEC 27018](offering-iso-27018.md)) 的驗證。

## <a name="detection-of-potential-breaches"></a>偵測潛在缺口

由於現代雲端運算的性質，並非在客戶雲端環境所發生的所有資料外洩，都牽涉到 Microsoft Azure 服務。Microsoft 使用 Azure 服務的共用模型來定義安全性與操作的責任。在討論雲端服務的安全性時，責任分擔非常重要；因為雲端服務提供者和客戶雙方都要對雲端安全性負責。

Microsoft 不會監視或回應客戶責任領域範圍內的安全性事故。我們不會將純由客戶造成的安全性洩漏當作 Azure 安全性事件來處理，且需要客戶的租用戶來負責回應。根據適用的服務合約，客戶事故回應可能會涉及與 Microsoft Azure [客戶支援](https://azure.microsoft.com/support/options/)部門共同作業。Microsoft Azure 也提供了各種服務 (例如 [Azure 資訊安全中心](https://azure.microsoft.com/services/security-center/)) 供客戶利用，以開發和管理安全性事件回應。

Azure 會根據安全性事故回應程序 (也就是 Microsoft Azure 事故管理計劃的子集) 回應潛在的資料外洩。系統會使用以下五個階段程序來實作 Azure 安全性事故回應：偵測、評估、診斷、穩定，及關閉。安全性事故回應小組可能會隨著調查進度輪流進行診斷和穩定。安全性事故回應程序的概觀說明如下：

| 階段 | 說明 |
|:------- |------------- |
| ***1：偵測*** | 潛在事件的第一個徵兆。 |
| ***2：評估*** | 待命事件回應小組成員會評估事件的影響和嚴重性。取決於證據，可能會也可能不會進一步向安全性回應小組呈報評估。 |
| ***3：診斷*** | 安全性回應專家進行技術或鑑定調查、找出內含項目、風險降低及因應措施策略。 若安全性小組相信客戶資料可能遭受非法或未經授權的人員存取，將會同步進行客戶事件通知程序。 |
| ***4：穩定及復原*** | 事件回應小組會建立復原計劃，以降低問題的風險。危機抑制步驟 (例如隔離受影響的系統) 可能會立即與診斷同步進行。長期風險降低預計要等到眼前的風險過後才會進行規劃。 |
| ***5：結案與檢討*** | 事件回應小組會建立概述事件詳細資訊的檢討，目的是修改原則、步驟和流程，以避免該事件再次發生。 |

Microsoft Azure 使用的偵測程序旨在探索會讓 Azure 服務的機密性、完整性和可用性遭受風險的事件。有數種事件可能會觸發調查：

- 自動化系統會透過內部監視和警示架構發出警示。這些警示會以病毒碼式警訊 (例如反惡意程式碼軟體、入侵偵測)，或透過旨在分析預期活動並在異常時發出警示的演算法等方式提供。
- 來自 Microsoft Azure 和 Azure Government 上所執行 Microsoft 服務的第一方報告。
- [Microsoft 安全回應中心 (MSRC)](https://www.microsoft.com/msrc) 收到透過[回報問題](https://msrc.microsoft.com/create-report)所回報的安全性弱點。 MSRC 會與合作夥伴及全球安全性研究人員合作來防止安全性事件，並進一步提升 Microsoft 產品的安全性。
- 透過[客戶支援入口網站](https://www.windowsazure.com/support/contact/)或 Microsoft Azure 與 Azure Government 管理入口網站回報的客戶報告，其中說明了歸因於 Azure 基礎結構的可疑活動 (而非客戶責任範圍內所發生的活動)。
- 安全性[紅隊和藍隊](https://azure.microsoft.com/blog/red-teaming-using-cutting-edge-threat-simulation-to-harden-the-microsoft-enterprise-cloud/)活動。 此策略利用由 Microsoft 攻擊性安全專家組成的高度技巧紅隊，來找出並攻擊在 Azure 中的潛在弱點。 負責安全性回應的藍隊必須偵測並防禦紅隊的活動。 我們會用紅隊和藍隊雙方的動作，來確認 Azure 所做的安全性回應是否能有效地因應安全性事件。 安全性紅隊和藍隊活動的執行皆符合參與規則，以協助確保對客戶資料的保護。
- Azure 服務操作員的呈報。Microsoft 員工都受過訓練，可發現潛在的安全性問題並向上呈報。

## <a name="azures-data-breach-response"></a>Azure 的資料外洩回應

Microsoft 會判斷功能性影響、復原能力和事件的資訊影響，來指派適當的調查優先順序及嚴重性等級。在調查過程中，優先順序和嚴重性都有可能會變更，取決於新的發現和結論。涉及對客戶資料有迫切或經確認風險的安全性事件，我們會視為高嚴重性而不眠不休地設法解決。

安全性回應小組會與 Microsoft Azure 安全性工程師及主題專家 (SME) 合作，根據證據的事實資料將事件分類。安全性事件可以歸類為：

- **誤判**：事件符合偵測準則，但經查明其實是正常商業活動的一部分，且可能需要將其篩選出。服務小組會找出誤判的根本原因，並以系統化的方式視需要運用偵測來源和進行微調，來解決這些問題。
- **安全事件**：系統、服務和/或網路中可觀察到的企圖攻擊、規避安全控制的事件，或已確定的事實表明客戶資料或個人資料可能遺失、損毀、更改、披露或未經授權存取。
- **安全性事件/客戶可報告的安全性/隱私權事件 (CRSPI)**：在 Microsoft 處理客戶資料或個人資料時，已確認 (例如，聲明) 違反安全導致意外或非法損毀、遺失、更改、未經授權披露或存取客戶資料或個人資料。
- **隱私權事件**：影響個人資料或資料處理的安全性事件，會導致意外的隱私權後果，包括未遵守 Microsoft 隱私權原則、標準和控制措施。
- **隱私權事件/客戶可回報的安全性/隱私權事件 (CRSPI)**：影響個人資料、資料或資料處理的安全性事件，會導致意外的隱私權後果，包括未遵守 Microsoft 隱私權原則、標準和控制措施。

若要宣告 CRSPI，Microsoft 必須先判斷客戶資料已遭到或可能已遭到未經授權的存取，且 (或) 有必須通知客戶的法律或合約承諾。雖然並非必要，但您最好了解對特定客戶的影響、資源存取與修復步驟。通常要等到安全性事件的診斷階段結束後，才會宣告事件屬於 CRSPI。不過，在所有直接相關的資訊都可供使用時，也可能會隨時宣告。

Microsoft 會確認是否已成功遏制客戶和商業風險，並實施了矯正措施。如有需要，會進行緊急風險降低步驟，以解決與事件關聯的迫切安全性風險。

Microsoft 也會完成資料外洩的內部檢討。在此過程中，會評估回應的充分程度和作業程序，並找出和實施安全性事件回應 SOP 或相關程序所需的任何更新。資料外洩的內部檢討是客戶無法取得的極機密記錄。不過，我們可以將檢討摘要並納入客戶事件通知中。在 Azure 的例行稽核週期中，會向外部稽核者提供這些報告以供審查。

## <a name="customer-notification"></a>客戶通知

Microsoft 依要求會向受影響的客戶和法規機構通知資料外洩。Microsoft 仰賴在 Azure 作業上進行大量的內部劃分。資料流程記錄也相當健全。此設計的好處是可以將大部分的事件限制在特定客戶的範圍內。目標是當客戶資料遭到外洩時，提供他們正確、實用且及時的通知。

聲明 CRSPI 之後，通知流程將會盡快進行，但同時仍考慮快速行動的安全性風險。 通常，在事件調查進行中時，便會同時展開設計通知的流程。 客戶通知會在我們宣告遭入侵的 72 小時內傳遞，*除了* 下列情況：

- Microsoft 認為執行通知的動作會增加其他客戶的風險。例如，通知的動作可能會驚動攻擊者，因而無法補救。
- 經 Microsoft 法務部門和事故執行經理審查過的其他不尋常或特殊情況。
- 72 小時的時間表可能會讓某些事故的詳細資料可供使用。 這些詳細資訊會隨著調查進行提供給客戶和監管單位。

Microsoft 可提供客戶詳細資訊，讓他們能執行內部調查，並協助他們符合對使用者的承諾，而不會過度延遲通知程序。

個人資料外洩的通知會經由 Microsoft 選擇的方式 ，包括透過電子郵件，來傳送給客戶。 資料外洩的通知會傳送至 Azure 資訊安全中心提供的安全性連絡人清單。您可以按照[實作指南](/azure/security-center/security-center-provide-security-contact-details)中的指示設定該清單。 如果未在 Azure 資訊安全中心提供連絡人資訊，則通知會傳送給一或多個 Azure 月租方案的管理員。 為了確保通知能順利送達，客戶有責任確定每個適用之月租方案和線上服務管理入口網站上的管理連絡人資訊是正確的。

Microsoft Azure 或 Azure Government 小組還可以選擇通知其他 Microsoft 人員，例如 Microsoft 客戶支援服務 (CSS) 團隊的成員和客戶的客戶經理 (AM) 或技術客戶經理 (TAM)。這些人通常與客戶關係密切，可以促成更快的補救。

## <a name="microsoft-dynamics-365-built-in-security-features"></a>Microsoft Dynamics 365 內建的安全性功能

Microsoft Dynamics 365 利用雲端服務基礎結構和內建安全性功能，確保使用安全性措施和機制來保護資料的安全。此外，Dynamics 365 在下列領域中提供有效資料存取和對資料完整性及隱私權的共同作業：[保護身分識別、資料保護、角色型安全性與威脅管理](https://www.microsoft.com/trustcenter/security/dynamics365-security)。

Microsoft Dynamics 365 供應項目遵循相同的技術與組織措施，可評估一或多個 Microsoft Azure 服務小組的資料安全資料外洩程序。 因此，記錄在「Microsoft Azure 資料外洩」通知文件中的任何資訊也類似於 Microsoft Dynamics 365 服務。

## <a name="windows-diagnostic-data-processor-configuration"></a>Windows 診斷資料處理者設定

[Windows 診斷資料處理者設定](/windows/privacy/configure-windows-diagnostic-data-in-your-organization)利用雲端服務基礎結構和內建安全性功能，使用安全性措施和機制來保護資料，確保資料安全。

它遵循一個或多個 Microsoft Azure 服務團隊為防止資料外洩流程採取的相同技術和組織措施。 因此，記錄在「Microsoft Azure 資料外洩」通知文件中的任何資訊也與 Windows 診斷資料處理器設定類似。

## <a name="learn-more"></a>深入了解

[Microsoft 信任中心](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
