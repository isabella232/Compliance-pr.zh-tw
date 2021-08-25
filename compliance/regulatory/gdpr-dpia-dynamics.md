---
title: 符合 GDPR 的 Dynamics DPIA
description: 提供資料控制者有關 Dynamics 365 的資訊，協助您判斷是否需要 DPIA 及要包含哪些詳細資料。
keywords: DPIA, Microsoft 365, Dynamics 365, Microsoft 365 文件, GDPR
robots: NOINDEX,NOFOLLOW
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
hideEdit: true
titleSuffix: Microsoft GDPR
ms.openlocfilehash: ed23af0982dd5ce066c78963f108c2b7eaa2403a
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482436"
---
# <a name="data-protection-impact-assessments-guidance-for-data-controllers-using-dynamics-365"></a>資料保護影響評估：資料控制者使用 Dynamics 365 的指引

在一般資料保護法規 (GDPR) 規範下，資料控制者需要為「可能導致自然人之權利和自由高風險」的處理作業準備資料保護影響評估 (DPIA)。 Dynamics 365 自身沒有任何固有的功能需要使用它的資料控制者建立 DPIA。 相反，是否需要 DPIA 將取決於資料控制者 *如何* 部署、設定和使用 Dynamics 365 的詳細資料和內容。 無論如何，DPIA 應該在專案生命週期的早期開始，並與規劃和開發程序並行執行。

本文件旨在提供資料控制者有關 Dynamics 365 的資訊，協助他們判斷是否需要 DPIA，以及若需要，應包含哪些詳細資料。

>[!Note]
>Microsoft 在本文章中不提供任何法律建議。本文章僅供參考。我們鼓勵客戶與其隱私權主管 (及/或指派的資料保護長 (DPO)) 及/或法律顧問及/或顧問合作，以確定與使用 Microsoft Azure 或任何其他 Microsoft 線上服務相關的任何 DPIA 的必要性和內容。

## <a name="part-1-determining-whether-a-dpia-is-needed"></a>第 1 部分：判斷是否需要 DPIA

GDPR 第 35 條規定，「如果某種處理，特別是使用新技術，並考慮到處理的性質、範圍、背景和目的，可能會對自然人的權利和自由造成高度風險」，資料控制者需要建立資料保護影響評估。它進一步闡述會發生這類高風險的特定因素，如下表所述。判斷是否需要 DPIA 時，資料控制者應根據控制者的特定 Dynamics 365 實作和使用，考慮這些因素，以及任何其他相關因素。

|**風險因素**|**Dynamics 365 的相關資訊**|
|:----|:----|
| 基於自動化處理對自然人的個人方面進行系統和廣泛的評估，包括概況分析，以及對自然人產生法律效果的決定或對自然人產生同樣重大影響的決定； | Dynamics 365 確實會執行特定的自動化資料處理，例如潛在客戶或商機評分 (例如預測銷售發生機率)。但它並非設計用來執行對個人產生法律效果或對個人產生同樣重大影響的決定的處理。<br><br> 不過，由於 Dynamics 365 是高度自訂的服務，資料控制者有可能設定它用於這類處理，例如雇用決定或信用申請的評分。 |
| 大規模處理 <sup>1</sup> 特殊類別的資料 (揭露種族或民族血統、政治傾向、宗教或哲學信仰或貿易同盟會員資格的個人資料，用於唯一識別自然人的基因資料、計量生物學資料，有關健康的資料或有關自然人性生活或性向的資料)，或與刑事定罪和犯罪行為有關的個人資料； | Dynamics 365 並非設計用來處理特殊類別的個人資料。 <br><br> 不過，資料控制者也 *可以* 使用 Dynamics 365 來處理列舉之特殊類別的資料。 例如，Dynamics 365 提供的醫療保健產業範本，可以用來處理與健康情況相關聯的個人資料。 再者，Dynamics 365 是個能高度自訂的服務，可讓客戶追蹤，或處理任何類型的個人資料，包括特殊類別的個人資料。 但身為資料處理者，Microsoft 對於這類使用無控制權，且通常僅有少許或完全沒有對該使用的瞭解。 |
| 大規模有系統地監視可公開進入的地區 | Dynamics 365 並非特別設計用來進行或協助這類監視。 <br><br> 不過，資料控制可以使用它來處理透過這類監視收集到的資料。 |

>[!Note]
><sup>1</sup> 關於「大規模」處理的準則，GDPR 第 91 條闡明：「如果處理是有關於個別醫生、其他醫療保健專業人員或律師之病患或客戶的個人資料，則處理個人資料不應視為大規模。 在此類情況下，資料保護影響評估不應強制」。

## <a name="part-2-contents-of-a-dpia"></a>第 2 部分：DPIA 的內容

第 35 (7) 條規定「資料保護影響評估」對設想的處理和處理目的進行有系統的描述。完整的 DPIA 系統描述可能包含像是處理的資料類型、資料會保留多久、資料位置和傳輸目的地，以及哪些第三方可以存取資料。此外，DPIA 也必須包含：

- 評估與目的有關的處理操作的必要性和比例性；
- 評估自然人的權利和自由風險；和 
- 旨在解決風險的措施，包括保障措施、安全措施和機制，以確保保護個人資料，並在考慮到資料主體和其他有關人員的權利和合法利益的情況下證明符合本條例。

下表包含與每個要素相關的 Dynamics 365 資訊。如同第 1 部分，資料控制者必須根據控制者的特定 Dynamics 365 實作和使用，考慮下列詳細資料，以及任何其他相關因素。

|**DPIA 的要素**|**Dynamics 365 的相關資訊**|
|:---|:---|
| 處理的目的 | 使用 Dynamics 365 進行處理的目的取決於實作、設定及使用 Dynamics 365 的控制者。 <br><br> Dynamics 365 是線上平台，由多個不相連的線上服務構成，每一個都有不同的處理目的。以下是 Dynamics365 提供的服務類型： <br><br> 核心的 **客戶參與** 是客戶關係管理服務。它包含下列線上服務： Dynamics 365 for Sales、Dynamics 365 for Marketing、Dynamics 365 for Customer Service、Dynamics 365 for Project Service、Dynamics 365 for Field Service。<br><br>**Dynamics 365 財務營運企業版** (D365FOEE) 是「軟體即服務」(SaaS) 形式的企業資源規劃套件，主要提供企業客戶銷售、服務、金融、營運、 製造、人力資源等管理。<br><br>**Dynamics 365 零售版**(D365FR) 是以「軟體即服務」(SaaS) 的形式提供，整合了適合企業零售商和經銷商的內部部署銷售點解決方案。<br><br>**Dynamics 365 生命週期服務 (LCS)** 是一項線上輔助服務，主要供企業用來部署、管理、維護客戶的 D365FOEE、D365FR 實作。<br><br>**Dynamics 365 Business Central** 是一種企業資源規劃服務，由 Microsoft 以「軟體即服務」(SaaS) 的形式提供給小型和中型企業。此服務可處理個人資料，以提供財務、製造、客戶關係管理、供應鏈、分析、電子商務方面的協助。<br><br>**Dynamics 365 for Talent** 是以「軟體即服務」(SaaS) 的形式提供，可為客戶提供人力資源管理以及下列服務：<br><br> *核心人力資源* - 此服務可簡化記錄保存工作，以及自動進行與組織人員配置相關的程序。這些程序包括員工留任、權益管理、報酬、訓練、績效審查以及變更管理。<br><br> *吸引* - 此服務可尋找、面談以聘雇人員。<br> *到任* - 此服務可協助新進人員熟悉他們的工作 *。<br><br>**Microsoft 社交參與** (MSE) 是提供給企業客戶的 Dynamics 365 輔助服務，用於 (i) 處理少數社交媒體窗口中張貼的公用社交媒體貼文和個人資料，協助它們分析並找出有興趣的主題 (例如趨勢)，以及管理公司或這些虛擬位置 (例如粉絲頁面) 中的團體，包括發佈內容到特定社交媒體窗口 (聆聽)；以及 (ii) 透過社交媒體中的私人通訊與資料主體直接互動 (參與)。<br><br> 在進行上述服務的處理者能力中，Dynamics 365 處理個人資料只是為了能如上所述提供客戶線上服務，包括符合目的並提供這些服務，例如個人化、安全性、網路詐騙和惡意程式碼防護、疑難排解、改進。<br><br> 根據[線上服務條款](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46)和[資料保護增訂版](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=67)的規定，Microsoft 作為資料處理者，可根據客戶提供的指示處理客戶資料，為客戶提供線上服務。 <br><br> 如標準[線上服務條款](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46)和[資料保護增訂版](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=67)所詳列，Microsoft 也會使用個人資料來支援限定的合法商務作業，包括：(1) 帳單和帳戶管理；(2) 薪酬 (例如，計算員工傭金和合作夥伴獎勵)；(3) 內部報告與建模 (例如，預測、收入、產能規劃、產品策略)；(4) 防範可能對 Microsoft 或 Microsoft 產品產生影響的欺詐、網路犯罪或網路攻擊；(5) 改善協助工具、隱私權或能源效率的核心功能；以及 (6) 財務報告和法律義務遵循 (遵守線上服務條款所述之客戶資料披露的相關限制)。 <br><br> Microsoft 可控制個人資料的處理方式，以支援前述特定的合法商務作業。一般情況下，Microsoft 會先彙總個人資料，再將其用於我們合法的商務作業，而去除 Microsoft 識別特定人員的能力，此外，在使用個人資料支援合法商務作業所需的處理時，會採用最低限度識別性的形式。<br><br> Microsoft 不會將客戶資料或其衍生的資料用於分析、廣告或類似的商業用途。 |
| 處理的個人資料類別  | **客戶資料：** 這是所有資料，包括文字、音訊、視訊或影像檔和軟體，由客戶提供給 Microsoft 或是透過使用 Microsoft 線上服務代表客戶提供。 其包括客戶上傳用於儲存或處理以及自訂的資料。 在 Office 365 中處理客戶資料的範例，包括 Exchange Online 中的電子郵件內容，和 SharePoint Online 或商務用 OneDrive 中儲存的文件或檔案。 <br><br> **服務產生的資料：** 這是 Microsoft 透過服務的運作而產生或衍生的資料，例如使用或效能資料。 這些資料大部分都包含由 Microsoft 產生的 pseudonymous 識別碼。 <br><br> **支援資料：** 這是為了獲得線上服務的技術支援，由客戶或代表客戶 (或客戶授權 Microsoft 從線上服務取得) 透過與 Microsoft 的合作向 Microsoft 提供的資料。 <br><br> 客戶資料、系統所產生的記錄資料和支援資料不包含系統管理員和帳單資料，例如客戶系統管理員連絡資訊、訂閱資訊和付款資料，Microsoft 會利用其資料控制者身分 (本文件範疇外) 所具備的功能收集和處理這些資料。 |
| 資料保留 | Microsoft 將在客戶使用服務的權利期間保留客戶資料，直到根據客戶指示或線上服務條款的條款刪除或退回所有客戶資料。在客戶訂閱期間的任何時候，客戶都可以存取和擷取儲存在服務中的客戶資料。Microsoft 將在客戶訂閱到期或終止訂閱後的 90 天內，將儲存在線上服務中的客戶資料保留在功能有限的帳戶中，以便客戶可以存取資料。90 天的保留期結束後，Microsoft 將停用客戶的帳戶並刪除客戶資料。<br><br> 客戶隨時可以使用 Dynamics 的[資料主體權利指南](gdpr-dsr-dynamics365.md)中描述的功能，刪除客戶資料和假名化資料。 |
| 個人資料的位置和傳輸 | 如果客戶將其 Dynamics 365 核心服務執行個體佈建在澳洲、加拿大、歐盟、印度、日本、英國或美國，Microsoft 會將靜態客戶資料儲存在指定的地理區域內，但受限於線上服務條款中的某些例外情況。如需客戶資料儲存空間的詳細資訊，可以在[信任中心](https://www.microsoft.com/trustcenter/cloudservices/dynamics365)找到。<br><br> 針對來自歐洲經濟區、瑞士和英國的個人資料，Microsoft 會確保個人資料傳輸給第三個國家/地區或國際組織時會受限於 GDPR 第 46 條所述的適當保護措施。 除了 Microsoft 承諾 (在處理程式和其他模型協定的標準契約條款下)，Microsoft 持續遵守 [隱私盾架構](https://www.privacyshield.gov/) 的條款，但是將不會再從歐盟/EEA 將個人資料傳輸到美國。 |
| 評估與目的有關的處理操作的必要性和比例性 | 這類評估取決於控制者的需求和處理的目的。<br><br>在處理者能力中，Microsoft 提供處理個人資料的 D365，僅為了能提供客戶線上服務，其中包含與提供這些服務相合之目的，例如客戶、安全性、詐騙和惡意程式碼防護、疑難排解和改進的個人化。Microsoft 代表客戶 (租用戶) 的要求處理資料，以提供位於線上服務條款 ([https://microsoft.com/licensing/contracts](https://microsoft.com/licensing/contracts)) 中規定之要求的服務。 |
| 評估資料主體的權利和自由風險  | 資料主體使用 Dynamics 365 在權利和自由方面的主要風險將取決於資料控制者如何以及在何種情況下實作、設定及使用 Dynamics 365。<br><br> Microsoft 對於其用來支援合法商務作業以利佈建服務的個人資料，會採用匿名化或彙總之類的機制，並盡可能降低使用服務的資料主體進行此類處理的風險。 <br><br> 但是，與任何服務一樣，服務中保存的個人資料可能存在未經授權的存取或無意揭露的風險。下面討論 Microsoft 為解決這些風險所採取的措施。 |
| 與第三方子處理者共用資料 | Microsoft 與充當我們子處理者的第三方共用資料，以支援客戶、技術支援、服務維護及其他操作等功能。接收 Microsoft 傳輸的客戶資料或支援資料的所有轉包商，都會與 Microsoft 達成書面協議，提供的保護不低於線上服務條款中的資料保護條款。所有共用 Microsoft 核心線上服務客戶資料的第三方子處理者都納入線上服務轉包商清單中。可能會存取支援資料 (包括客戶選擇在支援互動期間共用的客戶資料) 的第三方子處理者都納入 Microsoft 商業支援承包商清單中。 |
| 資料主體權利 | 以處理者的身分操作時，Microsoft 會為客戶 (資料控制者) 提供資料主體的個人資料，及其依據 GDPR 行使其權利時履行資料主體要求的能力。我們執行此作業的方式與產品功能一致，且角色如同是處理者。如果我們收到客戶資料主體中的要求，指出想要依據 GDPR 行使其一或多項權利，我們會將資料主體重新導向。針對 GDPR 和 CCPA 的 Dynamics 365 資料主體要求向資料控制者提供了如何使用 Dynamics 365 中的功能支援資料主體權利的描述。 <br><br> 若來自資料主體的要求旨在依據 GDPR 對處理後用以支援合法商務程序的個人資料行使權利，則該要求應按照 Microsoft 隱私權聲明中的說明導向至 Microsoft。 <br><br> Microsoft 通常會先彙總個人資料，再將其用於我們合法的商務作業，且無法在彙總資料中識別特定人員的個人資料。 這樣可以大幅降低個人承受的隱私權風險。  Microsoft 在無法識別個人身分的情況下，便無法支援存取、清除、可攜性、處理限制或異議等方面的資料主體權利。 |
| 旨在解決風險的措施，包括保障措施、安全措施和機制，以確保保護個人資料，並在考慮到資料主體和其他有關人員的權利和合法利益的情況下證明符合 GDPR | Microsoft 致力於協助保護客戶資訊的安全。根據 GDPR 第 32 條的規定，Microsoft 已經並將保持並遵循適當的技術和組織措施，旨在保護客戶資料和支援資料，避免遭受意外、未經授權或非法的存取、洩漏、更改、遺失或銷毀。<br><br>如需 Dynamics 365 實作的安全性中 Microsoft 管理控制項目 (技術和業務流程控制) 詳細清單，請前往[服務信任入口網站](https://servicetrust.microsoft.com/)。 此外，Microsoft 遵守適用於資料處理者的所有其他 GDPR 義務，包括但不限於提供資料保護影響評估和準確的記錄保存。 <br><br> Microsoft 在處理個人資料以供合法的商務作業使用時，會善盡資料控制者適用的 GDPR 義務。 |

## <a name="learn-more"></a>深入了解

- [Microsoft 信任中心](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
