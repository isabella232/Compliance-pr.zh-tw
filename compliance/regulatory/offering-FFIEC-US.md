---
title: '聯邦金融機構檢查委員會 (FFIEC) '
description: Microsoft 會協助金融服務用戶端遵守《聯邦金融機構檢查理事會 (FFIEC) 的審計要求。
keywords: Microsoft 365, 合規性, 方案
localization_priority: None
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
ms.openlocfilehash: 1830d0d61fe0787d7f8e8034af2e4ca64bdb0bc8
ms.sourcegitcommit: 01938022a292c07e98041dc6ae1312a1b8c617db
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58261021"
---
# <a name="federal-financial-institutions-examination-council-ffiec"></a>聯邦金融機構檢查委員會 (FFIEC) 

## <a name="ffiec-overview"></a>FFIEC 概述

「聯邦財務機構檢查委員會」 (FFIEC) 是由五個銀行機構組成的正式 interagency 本文，其適用于美國的美國聯邦政府檢查金融機構。 FFIEC 檢查程式教育 Office 會發佈 IT 考試手冊，以供來自 FFIEC 成員機構的欄位 examiners。

[FFIEC AUDIT IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/audit.aspx)包含這些 examiners 的指導方針，用以評估財務機構和 TSPS 的 IT 審計計畫的品質和效能。 具體而言，它包含對美洲認可的公開會計會計師 (AICPA) （如獨立的審計報告範例）所提的 SOC 1、SOC 2 和 SOC 3 認證報告。 不過，FFIEC 建議財務單位不只依賴這些報告中所含的資訊，但使用 [FFIEC 外包技術服務 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx)中詳細討論的驗證與監控程式。

## <a name="microsoft-and-ffiec"></a>Microsoft 和 FFIEC

Microsoft Azure、Microsoft Power BI 和 Microsoft Office 365 的建立，是為了符合為金融服務中心提供雲端服務的嚴格需求。 在我們的支援中，我們提供指導方針，協助您遵循資訊技術的 FFIEC 審核需求，以及在尋求您的 FFIEC 合規性義務時使用 Azure SOC attestations 的能力。

為了協助金融機構用戶端符合 Azure 的 FFIEC 合規性需求，Microsoft 已 [針對 FFIEC 管制服務工作負載開發 Azure 安全性與合規性藍圖](https://servicetrust.microsoft.com/ViewPage/FFIECBlueprint)。 它提供使用 Azure 雲端服務的指引，以及客戶遵循 FFIEC 需求和風險評估指導方針的考慮。

為了進一步協助您遵循 FFIEC 需求，Microsoft 雲端服務提供獨立 CPA 公司所產生的 [SOC 認證報告](offering-SOC.md) 。 例如，SOC 1 Type 2 認證是以 AICPA SSAE 18 standard (為基礎，請參閱105節) 取代的 SAS 70，且適用于報告某些財務報告的控制項。 SOC 報告包含審計員對 Microsoft 控制項效能的觀點，以在指定的監控期間達到相關的控制目標。 當針對 Azure、Power BI 和 Office 365 部署的資產採取 FFIEC 特定的合規性義務時，金融機構可使用此正式審計。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- Intune
- Office 365，Office 365 美國政府
- Power BI 雲端服務 (可作為獨立服務或包含在 Office 365 品牌方案或套件中)

## <a name="azure-dynamics-365-and-ffiec"></a>Azure、Dynamics 365 和 FFIEC

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE FFIEC 服務](/azure/compliance/offerings/offering-ffiec-us)。

## <a name="office-365-and-ffiec"></a>Office 365 和 FFIEC

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | Azure Active Directory、Azure 資訊保護、Bookings、合規性管理員、Delve、Exchange Online、Exchange Online Protection、Forms、Kaizala、Microsoft Analytics、Microsoft Booking、適用於 Office 365 的 Defender、Microsoft Graph、Microsoft Teams、Microsoft To-Do for Web、MyAnalytics、Office 365 進階合規性附加元件、Office 365 雲端 App 安全性、Office 365 群組、Office 365 安全性與合規性中心、Office 365 影片、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、StaffHub、Stream、Sway、Yammer Enterprise |
| **GCC** | Azure Active Directory、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream |

### <a name="office-365-audits-reports-and-certificates"></a>Office 365 稽核、報告和認證

請參閱 Office 365 SOC 認證報告。

### <a name="frequently-asked-questions"></a>常見問題集

**我可以使用 Microsoft 合規性與 SOC 標準，以符合我的機構的 FFIEC 合規性義務？**

為了協助您符合這些義務，Microsoft 會依照上述方式，提供與 SOC 標準的相容性相關資訊。 不過，最後，您可以決定我們的服務是否遵循適用于您機構的特定法律和規定。 FFIEC 也會建議 ' 審計報告或評論的使用者不應完全依賴報告中所包含的資訊，以驗證 TSP 的內部控制環境。 FFIEC IT 測驗手冊的 [外包技術手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx) 中所討論的功能，應使用其他驗證與監控程式。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [聯邦金融機構檢查委員會 (FFIEC) ](https://www.ffiec.gov/)
- [雲端計算和美國法規原則的符合性地圖](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [FFIEC 審計 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/audit.aspx)
- [FFIEC 外包技術服務 IT 測驗手冊](https://ithandbook.ffiec.gov/it-booklets/outsourcing-technology-services.aspx)

### <a name="other-microsoft-resources-for-financial-services"></a>其他適用於金融服務的 Microsoft 資源

- [Microsoft 金融服務合規性計劃](https://www.microsoft.com/download/details.aspx?id=55332)
- [Azure 的金融服務合規性](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Microsoft 商務用雲端服務與金融服務](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [共同承擔的雲端運算責任](https://aka.ms/sharedresponsibility)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
