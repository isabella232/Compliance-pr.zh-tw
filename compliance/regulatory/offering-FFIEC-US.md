---
title: '聯邦金融機構檢查委員會 (FFIEC) '
description: Microsoft 會協助金融服務用戶端遵守《聯邦金融機構檢查理事會 (FFIEC) 的審計要求。
keywords: Microsoft 365, 合規性, 方案
ms.localizationpriority: medium
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: 79d0f7bfff27f28b65d8f29c71f472024fbcd07e
ms.sourcegitcommit: cb0b058800d3a8f04921066b4c59fb427eb9c268
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2021
ms.locfileid: "59486350"
---
# <a name="federal-financial-institutions-examination-council-ffiec"></a>聯邦金融機構檢查委員會 (FFIEC) 

## <a name="ffiec-overview"></a>FFIEC 概述

「聯邦財務機構檢查委員會」 (FFIEC) 是由五個銀行機構組成的正式 interagency 本文，其適用于美國的美國聯邦政府檢查金融機構。 FFIEC 檢查程式教育 Office 會發佈 IT 考試手冊，以供來自 FFIEC 成員機構的欄位 examiners。

[FFIEC AUDIT IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/audit.aspx)包含這些 examiners 的指導方針，用以評估財務機構和 TSPS 的 IT 審計計畫的品質和效能。 具體而言，它包含對美洲認可的公開會計會計師 (AICPA) （如獨立的審計報告範例）所提的 SOC 1、SOC 2 和 SOC 3 認證報告。 不過，FFIEC 建議財務單位不只依賴這些報告中所含的資訊，但使用 [FFIEC 外包技術服務 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx)中詳細討論的驗證與監控程式。

## <a name="microsoft-and-ffiec"></a>Microsoft 和 FFIEC

Microsoft Azure、Microsoft Power BI 和 Microsoft Office 365 的建立，是為了符合為金融服務中心提供雲端服務的嚴格需求。 Azure 提供金融機構，含 SOC 1 Type 2、SOC 2 Type 2 和 SOC 3 認證報告（由獨立的審計公司產生），以協助客戶滿足其專屬的 FFIEC 合規性義務。 例如，在下列情況下， [SOC 1 類型2認證](./offering-soc-1.md) 會執行：

- SSAE 第 18 號，證明標準：釐清與重新編纂，其中包括 AT-C 第 320 節 *與使用者實體對財務報告之內部控制相關的服務組織控制措施檢查報告* (AICPA，專業標準)。
- SOC 1 報告在服務組織中與使用者實體對財務報告之內部控制相關的控制措施檢查 (AICPA 指南)

AICPA SSAE 18 standard 取代 SAS 70，其適用于與財務報告上的使用者實體相關的服務組織中的控制項報告。 當您在 Azure 上為部署的資產採取自己的 FFIEC 特定的合規性義務時，這是金融機構可利用技術服務提供者的協力廠商檢查的正式審核。 它包含審計員對控制效能的觀點，以在指定的監控期間達成相關的控制目標。

此外，Azure 已開發一個以 Excel 為基礎的雲端安全性診斷工具，其目的是為了加快金融機構可能想要與 Azure 服務相關執行的風險評估。 此工具是以試算表為基礎，其具有19個獨立的網域，可識別相關標準和金融服務相關規定中所規定的需求，包括 FFIEC IT 檢查手冊。  「風險評估」工具已預先填入說明，包含 Azure 如何符合雲端服務提供者的需求，並可協助客戶滿足其自身的 FFIEC 合規性需求。

此外，客戶也可以使用 Azure FFIEC cloud security 診斷活頁簿隨附的相關指引，它提供 Azure 服務的使用方式，以及客戶合規性與 FFIEC 需求的考慮

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- Intune
- Office 365，Office 365 美國政府
- Power BI 雲端服務 (可作為獨立服務或包含在 Office 365 品牌方案或套件中)

## <a name="azure-guidance-documents"></a>Azure 指導檔

為了協助金融機構受雲端採用的監管 FFIEC，Microsoft 已發佈下列指導檔，可從服務信任入口網站 [資料保護資源-合規性指南](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3) 一節中下載：

- Azure-雲端安全性診斷工具
- Azure-FFIEC cloud security 診斷活頁簿隨附

## <a name="office-365-and-ffiec"></a>Office 365 和 FFIEC

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | Azure Active Directory，Azure 資訊保護，預約，合規性管理員，Delve，Exchange Online，Exchange Online Protection，表單，Kaizala，microsoft Analytics，microsoft 預約，microsoft Defender for Office 365，microsoft Graph，Microsoft Teams，microsoft To-Do for Web、MyAnalytics Office 365 進階合規性安全性 Office 365 雲端 App 安全性相容性Center、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint 線上、商務用 Skype、StaffHub、Stream、Sway、Yammer Enterprise |
| **GCC** | Azure Active Directory、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream |

### <a name="office-365-audits-reports-and-certificates"></a>Office 365 稽核、報告和認證

請參閱 Office 365 SOC 認證報告。

### <a name="frequently-asked-questions"></a>常見問題集

**我可以使用 Microsoft 合規性與 SOC 標準，以符合我的機構的 FFIEC 合規性義務？**

為了協助您符合這些義務，Microsoft 會依照上述方式，提供與 SOC 標準的相容性相關資訊。 不過，最後，您可以決定我們的服務是否遵循適用于您機構的特定法律和規定。 FFIEC 也會建議 ' 審計報告或評論的使用者不應完全依賴報告中所包含的資訊，以驗證 TSP 的內部控制環境。 FFIEC IT 測驗手冊的 [外包技術手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx) 中所討論的功能，應使用其他驗證與監控程式。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評定風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

## <a name="resources"></a>資源

- [聯邦金融機構檢查委員會 (FFIEC) ](https://www.ffiec.gov/)
- [雲端計算和美國法規原則的符合性地圖](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [FFIEC 審計 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/audit.aspx)
- [FFIEC 外包技術服務 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx)

## <a name="other-microsoft-resources-for-financial-services"></a>其他適用於金融服務的 Microsoft 資源

- [Azure 合規性文件](/azure/compliance/)
- [Azure 可實現合規性世界](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Microsoft 雲端金融服務資源](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Microsoft 雲端金融服務規範計畫](https://aka.ms/FSCP-Print)
- [Microsoft Cloud 中金融機構的風險評估與規範指南](https://azure.microsoft.com/resources/risk-assessment-and-compliance-guide-for-financial-institutions-in-the-microsoft-cloud-/)
- [金融服務行業使用案例](/azure/industry/financial/)
