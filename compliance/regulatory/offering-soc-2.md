---
title: 系統與組織控制措施 (SOC) 2 Type 2
description: 了解 Microsoft 雲端服務如何符合系統與組織控制措施 (SOC) 2 Type 2 的作業安全性標準。
keywords: Microsoft 365、合規性、方案
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
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: 92fb47f98e60eb655ee68b38cb747a7d2eb9d2ff
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158923"
---
# <a name="system-and-organization-controls-soc-2-type-2"></a>系統與組織控制措施 (SOC) 2 Type 2

## <a name="soc-2-type-2-overview"></a>SOC 2 Type 2 概觀

適用於服務組織的系統與組織控制 (SOC) 是由美國會計師協會 (AICPA) 所建立的內部控制報告。 它們將用來檢查服務組織提供的服務，讓使用者能夠評估並解決與外包服務相關聯的風險。

SOC 2 Type 2 證明在以下條件下執行：

- SSAE 第 18 號，證明標準：釐清與重新編纂，其中包括 AT-C 第 105 節 *所有證明業務通用的概念* 和 AT-C 第 205 節 *檢查業務* (AICPA，專業標準)。
- SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)。
- TSP 第 100 節，2017 年安全性、可用性、處理完整性、機密性和隱私權的信任服務標準 (AICPA，2017 年信任服務標準)。

此外，Office 365 SOC 2 Type 2 證明報告滿足了雲端安全聯盟 (CSA) 雲端控制矩陣 (CCM) 和德國聯邦辦公室建立的雲端運算合規性標準目錄 (C5:2020) 中規定的資訊安全 (BSI) 要求。

Office 365 SOC 2 證明是根據信譽良好的 CPA 公司進行嚴格的獨立協力廠商稽核。 在 SOC 2 稽核結束時，稽核員會在 SOC 2 Type 2 報告中提出意見，其中描述雲端服務提供者 (CSP) 的系統，並評估 CSP 對其控制措施的描述是否公平。 並且評估 CSP 的控制項是否適當設計、是否已在指定日期執行，且在指定的期間內有效運作。 Office 365 SOC 2 Type 2 報告與系統安全性、可用性、處理完整性、機密性和隱私權相關。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

範圍中的 Microsoft 線上服務會顯示在 Azure SOC 2 Type 2 證明報告中：

- Azure (如何詳細深入資訊，請參閱 [Microsoft Azure 合規性方案](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/)或 Azure SOC 2 Type 2 證明報告)
- Azure DevOps (請參閱個別的 Azure DevOps SOC 2 Type 2 證明報告)
- Dynamics 365 (如需詳細深入資訊，請參閱 Azure SOC 2 Type 2 證明報告)
- Microsoft 365 Defender
- Microsoft 雲端 App 安全性 (MCAS)
- 適用於端點的 Microsoft Defender
- 適用於身分識別的 Microsoft Defender
- Microsoft Forms Pro (不在 Azure Government 的範圍內)
- Microsoft Graph
- Microsoft Intune
- Microsoft 受管理的電腦 (不在 Azure Government 的範圍內)
- Microsoft Stream
- Microsoft 威脅專家 (不在 Azure Government 的範圍內)
- 提名入口網站
- Office 365、Office 365 美國政府版、Office 365 美國政府版 - High、Office 365 美國政府國防版
- Power Apps
- 電源自動化
- Power BI
- Power Virtual Agent (不在 Azure Government 的範圍內)
- 更新合規性 (不在 Azure Government 的範圍內)

## <a name="azure-dynamics-365-and-soc-2"></a>Azure、Dynamics 365 和 SOC 2

如需 Azure、Dynamics 365 及其他線上服務合規性詳細資訊，請參閱 [Azure SOC 2 方案](/azure/compliance/offerings/offering-soc-2)。

## <a name="office-365-and-soc-2"></a>Office 365 和 SOC 2

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | 合規性管理員、客戶 Lockbox、Delve、Exchange Online Protection、Exchange Online、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Teams、MyAnalytics、Office 365 客戶入口網站、Office 365 微服務 (包括但不限於 Kaizala、ObjectStore、Sway、PowerPoint Online 文件服務、查詢註釋服務、學校資料同步處理、Siphon、語音、StaffHub、eXtensible Application Program)、Office Online、Office Services 基礎結構、商務用 OneDrive，Planner，PowerApps，Power Automate，Power BI，Project Online，客戶金鑰服務加密，SharePoint Online，商務用 Skype |
| **GCC** | Azure Active Directory、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream |
| **GCC High** | Azure Active Directory、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype |
| **DoD** | Azure Active Directory、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、Power BI、SharePoint Online、商務用 Skype |

### <a name="office-365-audit-reports"></a>Office 365 稽核報告

- [Office 365 核心版 - SSAE 18 SOC 2 報告](https://aka.ms/o365SOC-2)
- [Office 365 微服務 T1-SSAE 18 SOC2 Type I 報告](https://aka.ms/o365-MS-SOC-2-type1)
- [請參閱 Bridge Letter 和其他稽核報告](https://aka.ms/auditreports)

您必須在 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府中擁有現有的訂閱或免費試用帳戶，才能下載 SOC 1 和 SOC 2 證明報告，以及任何橋接信件 (如果需要)。

### <a name="frequently-asked-questions"></a>常見問題集

**Office 365 SOC 報告多久發行一次？**

Office 365 和其他線上服務的 SOC 報告皆以 12 個月執行 (稽核期間) 為基礎，且每半年發行一次新報告 (期間結束於 3 月 31 日與 9 月 30 日)。 每季都會發放 *橋接信件*，以涵蓋前三個月的內容。 例如，1 月信件涵蓋 10 月 1 日到 12 月 31 日，4 月信件涵蓋 1 月 1 日到 3 月 31 日，7 月信件涵蓋 4 月 1 日到 6 月 30 日，而 10 月信件涵蓋 7 月 1 日到 9 月 30 日。

**我可以在哪裡取得 Office 365 SOC 稽核文件，包括橋接信件？**

如需稽核文件的連結，請參閱稽核報告一節。 您必須擁有 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府的現有訂閱或免費試用帳戶才能登入。 然後，您可以下載稽核憑證、評定報告及其他適用的文件，協助您符合自己的法規需求。

**我可以在哪裡找到雲端安全性聯盟 CCM 控制措施的評定？**

Office 365 SOC 2 Type 2 稽核是根據美國會計師協會 (AICPA) 信任服務原則與準則 (包括安全性、可用性、機密性、隱私權和處理完整性) 以及雲端安全聯盟 (CSA) 雲端控制矩陣 (CCM) 中的準則所建立。 目標是同時符合上述的 AICPA 準則和 CCM 中規定的需求。 Office 365 SOC 2 Type 2 稽核會納入 CSA STAR 證明所需的 CCM 控制措施評定。 如需詳細資訊，請參閱 Office 365 SOC 2 Type 2 證明報告。

**我可以在哪裡查看已注意到的例外狀況管理回應？**

管理回應位於 SOC 證明報告的結尾處。 在文件中搜尋「管理回應」。

**我可以在哪裡查看使用者實體職責？**

使用者實體職責位於 SOC 證明報告的結尾。 在文件中搜尋「使用者實體職責」。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [服務信任入口網站稽核報告](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [適用於服務組織的 AICPA SOC](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE 第 18 號，證明標準：釐清與重新編纂 (AICPA 專業標準)](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (可供購買)
- [TSP 第 100 節 (AICPA，2017 年信任服務準則)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
