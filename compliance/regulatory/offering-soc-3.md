---
title: 系統與組織控制 (SOC) 3
description: 深入了解 Microsoft 雲端服務符合系統與組織控制 (SOC) 3 的作業安全性標準。
keywords: Microsoft 365、合規性、方案
localization_priority: Priority
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
ms.openlocfilehash: 1d6f6b0a4c9bd3ebbccb90331a8cf17df7ff8928
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385710"
---
# <a name="system-and-organization-controls-soc-3"></a><span data-ttu-id="27134-104">系統與組織控制 (SOC) 3</span><span class="sxs-lookup"><span data-stu-id="27134-104">System and Organization Controls (SOC) 3</span></span>

## <a name="soc-3-overview"></a><span data-ttu-id="27134-105">SOC 3 概觀</span><span class="sxs-lookup"><span data-stu-id="27134-105">SOC 3 overview</span></span>

<span data-ttu-id="27134-106">適用於服務組織的系統與組織控制 (SOC) 是由美國註冊會計師協會 (AICPA) 所建立的內部控制報告。</span><span class="sxs-lookup"><span data-stu-id="27134-106">System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA).</span></span> <span data-ttu-id="27134-107">它們將用來檢查服務組織提供的服務，讓使用者能夠評估並解決與外包服務相關聯的風險。</span><span class="sxs-lookup"><span data-stu-id="27134-107">They are intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.</span></span>

<span data-ttu-id="27134-108">*適用於服務組織的 SOC 3 SOC：一般用途報告的信任服務準則* 是一份簡短的公開 SOC 2 Type 2 證明報告版本，適用於需要保證服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施，但不需要完整 SOC 2 報告的使用者。</span><span class="sxs-lookup"><span data-stu-id="27134-108">*SOC 3 SOC for Service Organizations: Trust Services Criteria for General Use Report* is a short, publicly facing version of the SOC 2 Type 2 attestation report for users who need assurances about service organization's controls relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy but do not need a full SOC 2 report.</span></span> <span data-ttu-id="27134-109">由於 SOC 3 報告是一般用途報告，因此可以自由發佈。</span><span class="sxs-lookup"><span data-stu-id="27134-109">Because SOC 3 reports are general use reports, they can be freely distributed.</span></span>

<span data-ttu-id="27134-110">SOC 3 報告包含服務組織管理針對根據適用之信任服務準則達成承諾之控制措施有效性的書面聲明，以及服務稽核者對於是否合理說明管理判斷的意見。</span><span class="sxs-lookup"><span data-stu-id="27134-110">A SOC 3 report contains a written assertion by service organization management regarding control effectiveness to achieve commitments based on the applicable trust services criteria, as well as service auditor's opinion on whether management's assertion is stated fairly.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="27134-111">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="27134-111">Microsoft in-scope cloud platforms & services</span></span>

<span data-ttu-id="27134-112">Microsoft 範圍內服務會顯示在 Azure [SOC 2 Type 2 證明](offering-soc-2.md)報告中。</span><span class="sxs-lookup"><span data-stu-id="27134-112">Microsoft in-scope services are shown in the Azure [SOC 2 Type 2 attestation](offering-soc-2.md) report.</span></span>

- <span data-ttu-id="27134-113">Azure (有關詳細深入資訊，請參閱 [Microsoft Azure 合規性方案](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/)或 Azure SOC 2 Type 2 證明報告)</span><span class="sxs-lookup"><span data-stu-id="27134-113">Azure (for detailed insight, see [Microsoft Azure Compliance Offerings](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) or Azure SOC 2 Type 2 attestation report)</span></span>
- <span data-ttu-id="27134-114">Dynamics 365 (有關詳細深入資訊，請參閱 Azure SOC 2 Type 2 證明報告)</span><span class="sxs-lookup"><span data-stu-id="27134-114">Dynamics 365 (for detailed insight, see Azure SOC 2 Type 2 attestation report)</span></span>
- <span data-ttu-id="27134-115">Microsoft 365 Defender</span><span class="sxs-lookup"><span data-stu-id="27134-115">Microsoft 365 Defender</span></span>
- <span data-ttu-id="27134-116">Microsoft 雲端 App 安全性 (MCAS)</span><span class="sxs-lookup"><span data-stu-id="27134-116">Microsoft Cloud App Security (MCAS)</span></span>
- <span data-ttu-id="27134-117">適用於端點的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="27134-117">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="27134-118">適用於身分識別的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="27134-118">Microsoft Defender for Identity</span></span>
- <span data-ttu-id="27134-119">Microsoft Forms Pro (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="27134-119">Microsoft Forms Pro (not in scope for Azure Government)</span></span>
- <span data-ttu-id="27134-120">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="27134-120">Microsoft Graph</span></span>
- <span data-ttu-id="27134-121">Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="27134-121">Microsoft Intune</span></span>
- <span data-ttu-id="27134-122">Microsoft 受管理的電腦 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="27134-122">Microsoft Managed Desktop (not in scope for Azure Government)</span></span>
- <span data-ttu-id="27134-123">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="27134-123">Microsoft Stream</span></span>
- <span data-ttu-id="27134-124">Microsoft 威脅專家 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="27134-124">Microsoft Threat Experts (not in scope for Azure Government)</span></span>
- <span data-ttu-id="27134-125">提名入口網站</span><span class="sxs-lookup"><span data-stu-id="27134-125">Nomination Portal</span></span>
- <span data-ttu-id="27134-126">Office 365、Office 365 美國政府、Office 365 美國政府 - 高、Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="27134-126">Office 365, Office 365 U.S. Government, Office 365 U.S. Government - High, Office 365 U.S. Government Defense</span></span>
- <span data-ttu-id="27134-127">Power Apps</span><span class="sxs-lookup"><span data-stu-id="27134-127">Power Apps</span></span>
- <span data-ttu-id="27134-128">電源自動化</span><span class="sxs-lookup"><span data-stu-id="27134-128">Power Automate</span></span>
- <span data-ttu-id="27134-129">Power BI</span><span class="sxs-lookup"><span data-stu-id="27134-129">Power BI</span></span>
- <span data-ttu-id="27134-130">Power Virtual Agent (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="27134-130">Power Virtual Agents (not in scope for Azure Government)</span></span>
- <span data-ttu-id="27134-131">更新合規性 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="27134-131">Update Compliance (not in scope for Azure Government)</span></span>

## <a name="azure-dynamics-365-and-soc-3"></a><span data-ttu-id="27134-132">Azure、Dynamics 365 和 SOC 3</span><span class="sxs-lookup"><span data-stu-id="27134-132">Azure, Dynamics 365, and SOC 3</span></span>

<span data-ttu-id="27134-133">有關 Azure、Dynamics 365 及其他線上服務合規性詳細資訊，請參閱 [Azure SOC 3 方案](/azure/compliance/offerings/offering-soc-3)。</span><span class="sxs-lookup"><span data-stu-id="27134-133">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure SOC 3 offering](/azure/compliance/offerings/offering-soc-3).</span></span>

## <a name="office-365-and-soc-3"></a><span data-ttu-id="27134-134">Office 365 和 SOC 3</span><span class="sxs-lookup"><span data-stu-id="27134-134">Office 365 and SOC 3</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="27134-135">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="27134-135">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="27134-136">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="27134-136">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="27134-137">使用下表判斷 Office 365 服務和訂用帳戶的適用性：</span><span class="sxs-lookup"><span data-stu-id="27134-137">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="27134-138">**適用性**</span><span class="sxs-lookup"><span data-stu-id="27134-138">**Applicability**</span></span> | <span data-ttu-id="27134-139">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="27134-139">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="27134-140">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="27134-140">**Office 365**</span></span> | <span data-ttu-id="27134-141">合規性管理員、客戶 Lockbox、Delve、Exchange Online Protection、Exchange Online、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Teams、MyAnalytics、Office 365 客戶入口網站、Office 365 微服務 (包括但不限於 Kaizala、ObjectStore、Sway、PowerPoint Online 文件服務、查詢註釋服務、學校資料同步處理、Siphon、語音、StaffHub、eXtensible Application Program)、Office Online、Office Services 基礎結構、商務用 OneDrive，Planner，PowerApps，Power Automate，Power BI，Project Online，客戶金鑰服務加密，SharePoint Online，商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="27134-141">Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office Online, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Customer Key, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="27134-142">**GCC**</span><span class="sxs-lookup"><span data-stu-id="27134-142">**GCC**</span></span> | <span data-ttu-id="27134-143">Azure Active Directory、合規性管理員、Delve、Exchange Online、</span><span class="sxs-lookup"><span data-stu-id="27134-143">Azure Active Directory, Compliance Manager, Delve, Exchange Online,</span></span> 
<span data-ttu-id="27134-144">、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="27134-144">, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="27134-145">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="27134-145">**GCC High**</span></span> | <span data-ttu-id="27134-146">Azure Active Directory、Exchange Online、Flow、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="27134-146">Azure Active Directory, Exchange Online, Flow, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="27134-147">**DoD**</span><span class="sxs-lookup"><span data-stu-id="27134-147">**DoD**</span></span> | <span data-ttu-id="27134-148">Azure Active Directory、Exchange Online、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、Power Automate、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="27134-148">Azure Active Directory, Exchange Online, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power Automate, Power BI, SharePoint Online, Skype for Business</span></span> |

### <a name="office-365-audit-reports"></a><span data-ttu-id="27134-149">Office 365 稽核報告</span><span class="sxs-lookup"><span data-stu-id="27134-149">Office 365 audit reports</span></span>

- [<span data-ttu-id="27134-150">Office 365 核心版 - SSAE 18 SOC 3 報告</span><span class="sxs-lookup"><span data-stu-id="27134-150">Office 365 Core - SSAE 18 SOC 3 Report</span></span>](https://aka.ms/o365SOC-3)
- [<span data-ttu-id="27134-151">請參閱橋接信件和其他稽核報告</span><span class="sxs-lookup"><span data-stu-id="27134-151">See bridge letters and additional audit reports</span></span>](https://aka.ms/auditreports)

<span data-ttu-id="27134-152">您必須在 Office 365 或 Office 365 美國政府中擁有現有的訂閱或免費試用帳戶，才能下載 SOC 1 和 SOC 2 證明報告，以及任何橋接信件 (如果需要)。</span><span class="sxs-lookup"><span data-stu-id="27134-152">You must have an existing subscription or free trial account in Office 365 or Office 365 U.S. Government to download SOC 1 and SOC 2 attestation reports and any bridge letters as needed.</span></span>

### <a name="frequently-asked-questions"></a><span data-ttu-id="27134-153">常見問題集</span><span class="sxs-lookup"><span data-stu-id="27134-153">Frequently asked questions</span></span>

<span data-ttu-id="27134-154">**Office 365 SOC 報告多久發行一次？**</span><span class="sxs-lookup"><span data-stu-id="27134-154">**How often are Office 365 SOC reports issued?**</span></span>

<span data-ttu-id="27134-155">Office 365 和其他線上服務的 SOC 報告皆以 12 個月執行 (稽核期間) 為基礎，且每半年發行一次新報告 (期間結束於 3 月 31 日與 9 月 30 日)。</span><span class="sxs-lookup"><span data-stu-id="27134-155">SOC reports for Office 365 and other online services are based on a rolling 12-month run window (audit period) with new reports issued semi-annually (period ends are March 31 and September 30).</span></span> <span data-ttu-id="27134-156">每季都會發放 *橋接信件*，以涵蓋前三個月的內容。</span><span class="sxs-lookup"><span data-stu-id="27134-156">*Bridge letters* are issued each quarter to cover the prior three-month period.</span></span> <span data-ttu-id="27134-157">例如，1 月信件涵蓋 10 月 1 日到 12 月 31 日，4 月信件涵蓋 1 月 1 日到 3 月 31 日，7 月信件涵蓋 4 月 1 日到 6 月 30 日，而 10 月信件涵蓋 7 月 1 日到 9 月 30 日。</span><span class="sxs-lookup"><span data-stu-id="27134-157">For example, the January letter covers 1-Oct through 31-Dec, the April letter covers 1-Jan through 31-Mar, the July letter covers 1-Apr through 30-Jun, and the October letter covers 1-Jul through 30-Sep.</span></span>

<span data-ttu-id="27134-158">**我可以在哪裡取得 Office 365 SOC 稽核文件，包括橋接信件？**</span><span class="sxs-lookup"><span data-stu-id="27134-158">**Where can I get the Office 365 SOC audit documentation including bridge letters?**</span></span> <span data-ttu-id="27134-159">有關稽核文件的連結，請參閱稽核報告一節。</span><span class="sxs-lookup"><span data-stu-id="27134-159">For links to audit documentation, see the audit report section.</span></span> <span data-ttu-id="27134-160">您必須擁有 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府的現有訂閱或免費試用帳戶才能登入。</span><span class="sxs-lookup"><span data-stu-id="27134-160">You must have an existing subscription or free trial account in Office 365or [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 U.S. Government to login.</span></span> <span data-ttu-id="27134-161">然後，您可以下載稽核憑證、評定報告及其他適用的文件，協助您符合自己的法規需求。</span><span class="sxs-lookup"><span data-stu-id="27134-161">You can then download audit certificates, assessment reports, and other applicable documents to help you with your own regulatory requirements.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="27134-162">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="27134-162">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="27134-163">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="27134-163">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="27134-164">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="27134-164">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="27134-165">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="27134-165">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="27134-166">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="27134-166">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="27134-167">資源</span><span class="sxs-lookup"><span data-stu-id="27134-167">Resources</span></span>

- [<span data-ttu-id="27134-168">服務信任入口網站稽核報告</span><span class="sxs-lookup"><span data-stu-id="27134-168">Service Trust Portal audit reports</span></span>](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [<span data-ttu-id="27134-169">適用於服務組織的 AICPA SOC</span><span class="sxs-lookup"><span data-stu-id="27134-169">AICPA SOC for Service Organizations</span></span>](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [<span data-ttu-id="27134-170">SSAE 第 18 號，證明標準：釐清與重新編纂 (AICPA 專業標準)</span><span class="sxs-lookup"><span data-stu-id="27134-170">SSAE No. 18, Attestation Standards: Clarification and Recodification (AICPA Professional Standards)</span></span>](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- <span data-ttu-id="27134-171">[SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (可供購買)</span><span class="sxs-lookup"><span data-stu-id="27134-171">[SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (available for purchase)</span></span>
- [<span data-ttu-id="27134-172">TSP 第 100 節 (AICPA，2017 年信任服務準則)</span><span class="sxs-lookup"><span data-stu-id="27134-172">TSP section 100 (AICPA, 2017 Trust Services Criteria)</span></span>](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
