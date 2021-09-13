---
title: 系統與組織控制 (SOC) 3
description: 深入了解 Microsoft 雲端服務符合系統與組織控制 (SOC) 3 的作業安全性標準。
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
ms.openlocfilehash: b3690ba79ba8adca1d01e4eda03831c431747d01
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158859"
---
# <a name="system-and-organization-controls-soc-3"></a>系統與組織控制 (SOC) 3

## <a name="soc-3-overview"></a>SOC 3 概觀

適用於服務組織的系統與組織控制 (SOC) 是由美國註冊會計師協會 (AICPA) 所建立的內部控制報告。 它們將用來檢查服務組織提供的服務，讓使用者能夠評估並解決與外包服務相關聯的風險。

*適用於服務組織的 SOC 3 SOC：一般用途報告的信任服務準則* 是一份簡短的公開 SOC 2 Type 2 證明報告版本，適用於需要保證服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施，但不需要完整 SOC 2 報告的使用者。 由於 SOC 3 報告是一般用途報告，因此可以自由發佈。

SOC 3 報告包含服務組織管理針對根據適用之信任服務準則達成承諾之控制措施有效性的書面聲明，以及服務稽核者對於是否合理說明管理判斷的意見。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

Microsoft 範圍內服務會顯示在 Azure [SOC 2 Type 2 證明](offering-soc-2.md)報告中。

- Azure (有關詳細深入資訊，請參閱 [Microsoft Azure 合規性方案](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/)或 Azure SOC 2 Type 2 證明報告)
- Dynamics 365 (有關詳細深入資訊，請參閱 Azure SOC 2 Type 2 證明報告)
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

## <a name="azure-dynamics-365-and-soc-3"></a>Azure、Dynamics 365 和 SOC 3

有關 Azure、Dynamics 365 及其他線上服務合規性詳細資訊，請參閱 [Azure SOC 3 方案](/azure/compliance/offerings/offering-soc-3)。

## <a name="office-365-and-soc-3"></a>Office 365 和 SOC 3

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | 合規性管理員、客戶 Lockbox、Delve、Exchange Online Protection、Exchange Online、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Teams、MyAnalytics、Office 365 客戶入口網站、Office 365 微服務 (包括但不限於 Kaizala、ObjectStore、Sway、PowerPoint Online 文件服務、查詢註釋服務、學校資料同步處理、Siphon、語音、StaffHub、eXtensible Application Program)、Office Online、Office Services 基礎結構、商務用 OneDrive，Planner，PowerApps，Power Automate，Power BI，Project Online，客戶金鑰服務加密，SharePoint Online，商務用 Skype |
| **GCC** | Azure Active Directory、合規性管理員、Delve、Exchange Online、 
、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream |
| **GCC High** | Azure Active Directory、Exchange Online、Flow、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype |
| **DoD** | Azure Active Directory、Exchange Online、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、Power Automate、Power BI、SharePoint Online、商務用 Skype |

### <a name="office-365-audit-reports"></a>Office 365 稽核報告

- [Office 365 核心版 - SSAE 18 SOC 3 報告](https://aka.ms/o365SOC-3)
- [請參閱橋接信件和其他稽核報告](https://aka.ms/auditreports)

您必須在 Office 365 或 Office 365 美國政府中擁有現有的訂閱或免費試用帳戶，才能下載 SOC 1 和 SOC 2 證明報告，以及任何橋接信件 (如果需要)。

### <a name="frequently-asked-questions"></a>常見問題集

**Office 365 SOC 報告多久發行一次？**

Office 365 和其他線上服務的 SOC 報告皆以 12 個月執行 (稽核期間) 為基礎，且每半年發行一次新報告 (期間結束於 3 月 31 日與 9 月 30 日)。 每季都會發放 *橋接信件*，以涵蓋前三個月的內容。 例如，1 月信件涵蓋 10 月 1 日到 12 月 31 日，4 月信件涵蓋 1 月 1 日到 3 月 31 日，7 月信件涵蓋 4 月 1 日到 6 月 30 日，而 10 月信件涵蓋 7 月 1 日到 9 月 30 日。

**我可以在哪裡取得 Office 365 SOC 稽核文件，包括橋接信件？** 有關稽核文件的連結，請參閱稽核報告一節。 您必須擁有 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府的現有訂閱或免費試用帳戶才能登入。 然後，您可以下載稽核憑證、評定報告及其他適用的文件，協助您符合自己的法規需求。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [服務信任入口網站稽核報告](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [適用於服務組織的 AICPA SOC](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [SSAE 第 18 號，證明標準：釐清與重新編纂 (AICPA 專業標準)](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- [SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (可供購買)
- [TSP 第 100 節 (AICPA，2017 年信任服務準則)](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
