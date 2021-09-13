---
title: 資料保護影響評估 (DPIA) - 適用於使用 Windows 診斷資料處理者設定的控制器指引
description: 在使用 Microsoft 企業版的 Windows 資料處理者服務時，尋找相關資訊以判斷是否需要資料保護影響評估 (DPIA)。
keywords: DPIA, Microsoft 365, Microsoft 365 教育版, Microsoft 365 文件, GDPR
ms.localizationpriority: high
ROBOTS: NOINDEX, NOFOLLOW
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmaz
manager: laurawi
ms.reviewer: delinat
audience: itpro
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
hideEdit: true
ms.openlocfilehash: 325dc91f1d3480414236abfde38eb48d372f3e69
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158892"
---
# <a name="data-protection-impact-assessments-guidance-for-controllers-using-windows-diagnostic-data-processor-configuration"></a>資料保護影響評估：適用於使用 Windows 診斷資料處理者設定的控制器指引

>[!NOTE]
>本主題適用於 Windows 10 企業版、專業版和教育版 (版本 1809，2021 年 7 月更新及更新版本)。

在一般資料保護規定 (GDPR) 規範下，控制者需要為「可能導致自然人之權利和自由高風險」的處理作業準備資料保護影響評估 (DPIA)。 Windows 診斷資料處理者設定自身中沒有任何固有的功能，因此需要使用控制器建立 DPIA。 相反地，是否需要 DPIA 會視控制器部署、設定及使用 [Windows 診斷資料處理者設定](/windows/privacy/configure-windows-diagnostic-data-in-your-organization)的方式而有所不同。

本文件旨在提供控制者有關 Windows 診斷資料處理者設定的資訊，協助他們判斷是否需要 DPIA，以及若需要，應包含哪些詳細資料。

>[!Note]
>Microsoft 在本文章中不提供任何法律建議。本文章僅供參考。我們鼓勵客戶與其隱私權主管和法律顧問合作，以確定與他們使用 Windows 診斷資料處理器設定或任何其他 Microsoft 線上服務相關的任何 DPIA 的必要性和內容。

## <a name="part-1-determining-whether-a-dpia-is-needed"></a>第 1 部分：判斷是否需要 DPIA

GDPR 第 35 條規定，「如果某種處理，特別是使用新技術，並考慮到處理的性質、範圍、背景和目的，可能會對自然人的權利和自由造成高度風險」，控制者需要建立「資料保護影響評估」(DPIA)。它會進一步設定表示以下表格所述之高風險的特定因素。若要判斷是否需要 DPIA，控制者應考慮這些因素，以及任何其他相關因素，並將其用於 Windows 診斷資料處理者設定的特定執行和使用。

## <a name="table-1-windows-diagnostic-data-processor-configuration-dpia-risk-factors"></a>表 1：Windows 診斷資料處理者設定 DPIA 風險因素

| 高風險因素 | Windows 診斷資料處理者設定相關資訊 |
|:----|:----|
| 基於自動化處理對自然人的個人方面進行系統和廣泛的評估，包括概況分析，以及對自然人產生法律效果的決定或對自然人產生同樣重大影響的決定。 |Windows 診斷資料處理者設定未提供用來執行某些資料自動處理的功能。 <br><br> 不過，由於其他服務會使用根據 Windows 診斷資料處理者設定收集的診斷資料做為資料來源，資料控制器可能會將這些服務設定為用於此類處理。 控制者應該根據使用根據 Windows 診斷資料處理者設定所收集之診斷資料的服務使用狀況來判斷。|
| 大規模處理特殊類別的資料 (揭露種族或民族血統、政治傾向、宗教或哲學信仰，或貿易同盟會員資格的個人資料，用於唯一識別自然人的基因資料、計量生物學資料，有關健康的資料或有關自然人性生活或性向的資料)，或與刑事定罪和犯罪行為有關的個人資料。 | Windows 診斷資料處理者設定並非特別設計用來處理特殊類別的個人資料，Windows 診斷資料處理者設定的使用方式並不會增加控制者處理的固有風險。 <br><br> 不過，資料控制者可以使用使用根據 Windows 診斷資料處理者設定所收集之診斷資料的服務，處理列舉的特殊類別資料。 使用根據 Windows 診斷資料處理者設定所收集的診斷資料做為資料來源的服務，可讓客戶追蹤或以其他方式處理任何類型的資料，包括個人資料的特殊類別。 但身為資料處理者，Microsoft 對於這類使用無控制權，且只有少許或完全沒有對該使用的瞭解。 資料控制器擁有權，可決定資料控制器資料的適當使用。|

## <a name="part-2-contents-of-a-dpia"></a>第 2 部分：DPIA 的內容

第 35 (7) 條規定「資料保護影響評估」對設想的處理和處理目的進行有系統的描述。完整的 DPIA 系統描述可能包含像是處理的資料類型、資料會保留多久、資料位置和傳輸目的地，以及哪些第三方可以存取資料。此外，DPIA 也必須包含：

- 評估與目的有關的處理操作的必要性和比例性；
- 評估自然人的權利和自由風險；和 
- 旨在解決風險的措施，包括保障措施、安全措施和機制，以確保保護個人資料，並在考慮到資料主體和其他有關人員的權利和合法利益的情況下證明符合本條例。

下表包含與這些元素相關的 Windows 診斷資料處理者設定相關資訊。 在第 1 部分，資料控制器需考慮以下提供之細節，以及任何其他相關因素，並將其用於 Windows 診斷資料處理者設定的特定執行和使用。

## <a name="table-2-windows-diagnostic-data-processor-configuration-dpia-elements"></a>表 2：Windows 診斷資料處理者設定 DPIA 元素

| DPIA 的元素 | Windows 診斷資料處理者設定相關資訊 |
|:---|:---|
| 處理的目的 | 處理根據 Windows 診斷資料處理者設定收集之診斷資料的目的，取決於進行實作、設定及使用的控制者。 <br><br> Microsoft 作為資料處理者，會依據 Microsoft 產品條款中的條款處理 Windows 診斷資料。 <br><br> Microsoft 也會使用個人資料來支援限定的商務作業，包括：(1) 帳單和帳戶管理；(2) 薪酬 (例如，計算員工傭金和合作夥伴獎勵)；(3) 內部報告與建模 (例如，預測、收入、容量規劃、產品策略)；(4) 防範可能對 Microsoft 或 Microsoft 產品產生影響的欺詐、網路犯罪或網路攻擊；(5) 改善協助工具、隱私權或能效的核心功能；以及 (6) 財務報告和法律義務遵循 (遵守 Windows 診斷資料的相關限制)。 <br><br> Microsoft 是這些特定合法公司行號的 Windows 診斷資料處理的控制者。通常，Microsoft 在將 Windows 診斷資料用於我們的合法企業運作之前會彙總這些資料，進而去除 Microsoft 識別特定個人的能力，此外，並以最不易識別的形式使用 Windows 診斷資料，以支援合法企業運作所需的處理。 <br><br> Microsoft 不會使用啟用 Windows 診斷資料處理者設定時所收集的 Windows 診斷資料，或基於任何廣告或類似商業用途而衍生的資訊。|
| 已處理的個人資料類別 | **Windows 診斷資料**：來自 Windows 裝置的技術資料，那些資料和裝置以及 Windows 與相關軟體的執行狀況有關。 它用來讓 Windows 保持最新狀態、安全、可靠、高效能，以及改善產品。 Windows 診斷資料的一些範例是使用的硬體類型、按其各自用途安裝的應用程式以及裝置驅動程式上的可靠性資訊。 某些 Windows 元件及應用程式會直接連線到 Microsoft 服務，但是它們交換的資料並非 Windows 診斷資料。 例如，交換使用者位置以取得當地的天氣或新聞，並不是 Windows 診斷資料的範例。 <br><br> 有關使用 Windows 診斷資料處理者設定時資料處理的資訊，請參閱[設定貴組織中的 Windows 診斷資料](/windows/privacy/configure-windows-diagnostic-data-in-your-organization)，以及 [Microsoft 信任中心](https://www.microsoft.com/trust-center)。|
| 資料保留 | Microsoft 將保留並處理根據 Microsoft 產品條款啟用 Windows 診斷資料處理器設定時所收集的 Windows 診斷資料。 客戶可以使用 [Windows 診斷資料處理器設定 GDPR 和 CCPA 的資料主體要求](gdpr-dsr-windows.md)中所述的功能，根據資料主體要求刪除和匯出 Windows 診斷資料。|
| 個人資料的位置和傳輸 | 啟用 Windows 診斷資料處理器設定時所收集的 Windows 診斷資料位於美國的 Microsoft 資料中心。 |
| 與第三方共用資料 | Microsoft 可能會與充當我們次處理者 (也就是處理個人資料的次承攬人) 的第三方共用資料，以支援客戶、技術支援、服務維護及其他操作等功能。 Microsoft 根據 Windows 診斷資料處理者設定或支援資料傳輸所收集之 Windows 診斷資料的任何次承攬人，都將與 Microsoft 簽訂書面協定，其保護性不低於 Microsoft 產品條款中的條款。 所有共用 Windows 診斷資料或支援資料的第三方次承攬人都納入[次承攬人清單](https://www.microsoft.com/en-us/trust-center/privacy/data-access#subcontractors)中 (請參閱「我們限制次承攬人的存取」)。 <br><br>針對執法機關和第三方對根據 Windows 診斷資料處理者設定所收集之 Windows 診斷資料和支援資料的要求，Microsoft 回應的相關資訊在 Microsoft 產品條款中。除非法律禁止 Microsoft 這樣做，Microsoft 會嘗試引導執法機關或第三方直接向客戶提出要求。 |
| 資料主體權利 | 以處理者的身分操作時，Microsoft 會為客戶 (控制者) 提供資料主體的個人資料，及其依據 GDPR 行使其權利時履行資料主體要求的能力。Microsoft 執行此作業的方式與產品功能一致，且其角色如同是資料處理者。如果 Microsoft 收到客戶資料主體中的要求，指出想要依據 GDPR 行使其一或多項權利，該要求將會重新導向至資料控制者。<br><br> [GDPR 和 CCPA 的 Windows 診斷資料處理器設定資料主體要求](gdpr-dsr-windows.md)提供如何支援根據 Windows 診斷資料處理器設定所收集之 Windows 診斷資料的資料主體權利之說明。 |
| 評估與目的有關的處理操作的必要性和比例性 | 這類評估取決於資料控制者的需求和處理的目的。 <br><br> 關於 Microsoft 進行的處理，這種處理對於與 Microsoft 產品條款中反映的處理目的是必要的且符合比例原則。 |
| 評估資料主體的權利和自由風險  | 資料主體使用根據 Windows 診斷資料處理器設定所收集之 Windows 診斷資料在權利和自由方面的主要風險，將取決於控制者如何以及在何種情況下實作、設定及使用 Windows 診斷資料。 <br><br> 根據 Windows 診斷資料處理器設定所收集的 Windows 診斷資料，可能有未經授權的存取或意外洩漏的風險。 Microsoft 產品條款中會討論 Microsoft 為解決這些風險所採取的措施。 |
| 旨在解決風險的措施，包括保障措施、安全措施和機制，以確保保護個人資料，並在考慮到資料主體和其他有關人員的權利和合法利益的情況下證明符合 GDPR | Microsoft 致力於幫助保護 Windows 診斷資料的安全。Microsoft 所採取的安全性措施描述於 Microsoft 產品條款中。<br><br> Microsoft 採取合理且適當的技術和組織措施來保護其所處理的個人資料。這些措施包括（但不限於）內部隱私政策和做法、合約承諾，以及國際和地區性標準認證。如需詳細資訊，請移至[信任中心的隱私權標準頁面](https://www.microsoft.com/trustcenter/privacy/we-set-and-adhere-to-stringent-standards)。<br><br> Microsoft 提供重要、透明的面向客戶的安全性和隱私權材料，以幫助解釋 Microsoft 對個人資料的使用和處理。我們歡迎客戶連絡 Microsoft 提出問題。 <br><br> 此外，Microsoft 遵守適用於資料處理者的所有其他 GDPR 義務，包括但不限於提供資料保護影響評估和記錄保存。 <br><br> Microsoft 在處理 Windows 診斷資料以供合法的商務作業使用時，會善盡資料控制者適用的 GDPR 義務。 |

## <a name="learn-more"></a>深入了解

- [Microsoft 信任中心](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
