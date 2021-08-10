---
title: GDPR 和 CCPA 的 Azure DevOps 資料主體要求
description: 了解如何使用 Microsoft 工具以匯出或刪除在 Azure DevOps Services 的驗證工作階段期間所收集的個人資料。
keywords: Visual Studio Team Services、VSTS、Azure DevOps 文件、隱私權、GDPR、CCPA
localization_priority: Priority
audience: itpro
ms.prod: devops
ms.topic: article
author: robmazz
ms.author: robmazz
f1.keywords:
- NOCSH
manager: laurawi
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
ms.workload:
- multiple
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-mar2020
hideEdit: true
ms.openlocfilehash: c159ea68bce536e0fcd273c6c1f8da721b2a863570c43c79c3678696641ea832
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54293060"
---
# <a name="azure-devops-services-data-subject-requests-for-the-gdpr-and-ccpa"></a>GDPR 和 CCPA 的 Azure DevOps Services 資料主體要求

歐盟[一般資料保護規範 (GDPR)](https://ec.europa.eu/justice/data-protection/reform/index_en.htm) 賦予人員 (在規範中稱為「資料主體」) 權限，以管理由「資料控制者」收集而來的個人資料，「資料控制者」(或簡稱「控制者」) 是雇主或其他類型的公司或組織。個人資料在 GDPR 中的定義很廣泛，係指與已識別或可識別的自然人相關的任何資料。GDPR 賦予資料主體對其個人資料的特定權限，這些權限包括取得個人資料副本、要求更正資料、限制資料的處理、刪除資料或以電子格式接收資料，以便轉交給其他控制者。由資料主體向控制者提出對其個人資料採取某項動作的正式要求，稱為「資料主體要求」或 DSR。

同樣地，加州消費者隱私法 (CCPA) 為加州客戶提供隱私權和義務，包括與 GDPR 資料主體權利相似的權利，例如有權刪除、存取和接收 (可攜性) 其個人資訊。  CCPA 也提供特定揭露、針對選擇行使權時的歧視提供保護，以及特定資料傳輸的「選擇退出/選擇加入」需求分類為「銷售」。 銷售的廣泛定義，包括出於有價值的考量而共用資料。 如需 CCPA 的詳細資訊，請參閱[加州消費者隱私法](offering-ccpa.md)和[常見問題集](ccpa-faq.yml)。

如需關於 GDPR 的一般資訊，請參閱[服務信任入口網站的 GDPR 區段](https://servicetrust.microsoft.com/ViewPage/GDPRGetStarted)。

本指南將討論如何使用 Microsoft 工具，將 Visual Studio Team Services (先前稱為 Visual Studio Team Services) 的驗證 (登入) 工作階段期間所收集的個人資料匯出或刪除。

## <a name="additional-privacy-information"></a>其他隱私權資訊

[Microsoft 隱私權聲明](https://privacy.microsoft.com/privacystatement)、[線上服務條款 (OST)](https://www.microsoft.com/licensing/product-licensing/products.aspx)，和 [Microsoft 的 GDPR 承諾](/legal/gdpr)文章描述我們的資料處理做法。

## <a name="personal-data-we-collect"></a>我們收集的個人資料

Microsoft 會向使用者收集資料來運作及改善 Azure DevOps Services。Azure DevOps Services 會收集兩個類型的資料：客戶資料和系統產生的記錄。客戶資料包括 Azure DevOps Services 運作服務所需的使用者識別交易式和互動式資料。系統產生的記錄包含針對每個產品區域和功能所彙總的服務使用狀況資料。

## <a name="delete-azure-devops-data"></a>刪除 Azure DevOps 資料

若要刪除相關聯的 Azure DevOps Services 客戶資料，並將系統產生的記錄中找到的個人識別資料匿名化，第一個步驟是關閉您的 Azure Active Directory (AAD) 或 Microsoft 帳戶 (MSA)。會利用嚴格的整合性、追蹤功能與稽核規則，仰賴 Azure DevOps Services 作為記錄的系統。這些現有規範會影響我們刪除及保留 GDPR 的義務。關閉身分識別帳戶並不會修改、移除或變更與 Azure DevOps 組織中個人身分識別相關聯的成品和記錄。我們已確定在刪除整個 Azure DevOps 組織時，該帳戶中找到的所有相關聯個人識別資料和系統產生的記錄都會從我們的系統中移除 (在必要的 Azure DevOps 組織 30 天虛刪除期間結束後)。

## <a name="export-azure-devops-data"></a>匯出 Azure DevOps 資料

控制者可以藉由兩種方法之一，將向其資料主題收集的客戶資料和系統產生記錄匯出，取決於用來登入 Azure DevOps Services 的身分識別提供者 (MSA 或 AAD) 而定。

- 使用 Azure 租用戶所支援帳戶，例如與 Azure 訂閱相關聯的 AAD 帳戶或 MSA 帳戶的使用者可遵循 [GDPR 的 Azure 資料主體要求](gdpr-dsr-azure.md)中的指示。

- 使用 MSA 身分識別進行驗證的使用者可以使用這個[隱私權要求網站](https://www.microsoft.com/concern/privacyrequest-msa)來查看多個 Microsoft 服務中繫結至 MSA 身分識別的活動資料。在此案例中，使用者是自己的個人資料的控制者。

## <a name="export-or-delete-issues"></a>匯出或刪除問題

針對 AAD 身分識別，如果您從 Azure 入口網站匯出或刪除資料時遇到問題，請前往 Azure 入口網站 **[協助 + 支援]** 刀鋒視窗，並在 **[訂閱管理]** > **[訂閱的隱私權和合規性要求]** > **[隱私權刀鋒視窗和 GDPR 要求]** 下提交新票證。

針對 MSA 身分識別，如果您從隱私權要求網站匯出資料時遇到問題，請登入[隱私權要求網站](https://www.microsoft.com/concern/privacyrequest-msa)並提交要求，以透過要求網路表格取得 Microsoft 隱私權小組提供的協助。

## <a name="learn-more"></a>深入了解

Microsoft 會竭盡所能確保 Azure DevOps Services 資料保持安全且隱私，沒有任何例外。若要深入了解我們如何保護您的 Azure DevOps Services 資料，請造訪 [Azure DevOps Services 資料保護概觀](/vsts/articles/team-services-security-whitepaper)白皮書。

## <a name="see-also"></a>另請參閱

- [Microsoft 對公開發行企業軟體產品客戶的 GDPR 承諾](/legal/gdpr)
- [Microsoft 信任中心](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
- [服務信任入口網站](https://servicetrust.microsoft.com/ViewPage/GDPRGetStarted)
- [Microsoft 隱私權儀表板](https://account.microsoft.com/privacy)
- [Microsoft 隱私權回應中心](https://aka.ms/userprivacysite)
- [GDPR 的 Azure 資料主體要求](gdpr-dsr-azure.md)
