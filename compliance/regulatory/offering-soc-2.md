---
title: 系統與組織控制措施 (SOC) 2 Type 2
description: 了解 Microsoft 雲端服務如何符合系統與組織控制措施 (SOC) 2 Type 2 的作業安全性標準。
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
ms.openlocfilehash: c20ad27b244825e017d7545e669262ca61202b60
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385713"
---
# <a name="system-and-organization-controls-soc-2-type-2"></a><span data-ttu-id="be149-104">系統與組織控制措施 (SOC) 2 Type 2</span><span class="sxs-lookup"><span data-stu-id="be149-104">System and Organization Controls (SOC) 2 Type 2</span></span>

## <a name="soc-2-type-2-overview"></a><span data-ttu-id="be149-105">SOC 2 Type 2 概觀</span><span class="sxs-lookup"><span data-stu-id="be149-105">SOC 2 Type 2 overview</span></span>

<span data-ttu-id="be149-106">適用於服務組織的系統與組織控制 (SOC) 是由美國會計師協會 (AICPA) 所建立的內部控制報告。</span><span class="sxs-lookup"><span data-stu-id="be149-106">System and Organization Controls (SOC) for Service Organizations are internal control reports created by the American Institute of Certified Public Accountants (AICPA).</span></span> <span data-ttu-id="be149-107">它們將用來檢查服務組織提供的服務，讓使用者能夠評估並解決與外包服務相關聯的風險。</span><span class="sxs-lookup"><span data-stu-id="be149-107">They are intended to examine services provided by a service organization so that end users can assess and address the risk associated with an outsourced service.</span></span>

<span data-ttu-id="be149-108">SOC 2 Type 2 證明在以下條件下執行：</span><span class="sxs-lookup"><span data-stu-id="be149-108">A SOC 2 Type 2 attestation is performed under:</span></span>

- <span data-ttu-id="be149-109">SSAE 第</span><span class="sxs-lookup"><span data-stu-id="be149-109">SSAE No.</span></span> <span data-ttu-id="be149-110">18 號，證明標準：釐清與重新編纂，其中包括 AT-C 第 105 節 *所有證明業務通用的概念* 和 AT-C 第 205 節 *檢查業務* (AICPA，專業標準)。</span><span class="sxs-lookup"><span data-stu-id="be149-110">18, Attestation Standards: Clarification and Recodification, which includes AT-C section 105, *Concepts Common to All Attestation Engagements*, and AT-C section 205, *Examination Engagements* (AICPA, Professional Standards).</span></span>
- <span data-ttu-id="be149-111">SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)。</span><span class="sxs-lookup"><span data-stu-id="be149-111">SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide).</span></span>
- <span data-ttu-id="be149-112">TSP 第 100 節，2017 年安全性、可用性、處理完整性、機密性和隱私權的信任服務標準 (AICPA，2017 年信任服務標準)。</span><span class="sxs-lookup"><span data-stu-id="be149-112">TSP section 100, 2017 Trust Services Criteria for Security, Availability, Processing Integrity, Confidentiality, and Privacy (AICPA, 2017 Trust Services Criteria).</span></span>

<span data-ttu-id="be149-113">此外，Office 365 SOC 2 Type 2 證明報告滿足了雲端安全聯盟 (CSA) 雲端控制矩陣 (CCM) 和德國聯邦辦公室建立的雲端運算合規性標準目錄 (C5:2020) 中規定的資訊安全 (BSI) 要求。</span><span class="sxs-lookup"><span data-stu-id="be149-113">In addition, the Office 365 SOC 2 Type 2 attestation report addresses the requirements set forth in the Cloud Security Alliance (CSA) Cloud Controls Matrix (CCM), and the Cloud Computing Compliance Criteria Catalogue (C5:2020) created by the German Federal Office for Information Security (BSI).</span></span>

<span data-ttu-id="be149-114">Office 365 SOC 2 證明是根據信譽良好的 CPA 公司進行嚴格的獨立協力廠商稽核。</span><span class="sxs-lookup"><span data-stu-id="be149-114">Office 365 SOC 2 attestations are based on rigorous independent third-party audits conducted by a reputable CPA firm.</span></span> <span data-ttu-id="be149-115">在 SOC 2 稽核結束時，稽核員會在 SOC 2 Type 2 報告中提出意見，其中描述雲端服務提供者 (CSP) 的系統，並評估 CSP 對其控制措施的描述是否公平。</span><span class="sxs-lookup"><span data-stu-id="be149-115">At the conclusion of a SOC 2 audit, the auditor renders an opinion in a SOC 2 Type 2 report, which describes the cloud service provider's (CSP) system and assesses the fairness of the CSP's description of its controls.</span></span> <span data-ttu-id="be149-116">並且評估 CSP 的控制項是否適當設計、是否已在指定日期執行，且在指定的期間內有效運作。</span><span class="sxs-lookup"><span data-stu-id="be149-116">It also evaluates whether the CSP's controls are designed appropriately, were in operation on a specified date, and were operating effectively over a specified time period.</span></span> <span data-ttu-id="be149-117">Office 365 SOC 2 Type 2 報告與系統安全性、可用性、處理完整性、機密性和隱私權相關。</span><span class="sxs-lookup"><span data-stu-id="be149-117">Office 365 SOC 2 Type 2 reports are relevant to system Security, Availability, Processing Integrity, Confidentiality, and Privacy.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="be149-118">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="be149-118">Microsoft in-scope cloud platforms & services</span></span>

<span data-ttu-id="be149-119">範圍中的 Microsoft 線上服務會顯示在 Azure SOC 2 Type 2 證明報告中：</span><span class="sxs-lookup"><span data-stu-id="be149-119">Microsoft online services in scope are shown in the Azure SOC 2 Type 2 attestation report:</span></span>

- <span data-ttu-id="be149-120">Azure (如何詳細深入資訊，請參閱 [Microsoft Azure 合規性方案](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/)或 Azure SOC 2 Type 2 證明報告)</span><span class="sxs-lookup"><span data-stu-id="be149-120">Azure (for detailed insight, see [Microsoft Azure Compliance Offerings](https://azure.microsoft.com/resources/microsoft-azure-compliance-offerings/) or Azure SOC 2 Type 2 attestation report)</span></span>
- <span data-ttu-id="be149-121">Azure DevOps (請參閱個別的 Azure DevOps SOC 2 Type 2 證明報告)</span><span class="sxs-lookup"><span data-stu-id="be149-121">Azure DevOps (see separate Azure DevOps SOC 2 Type 2 attestation report)</span></span>
- <span data-ttu-id="be149-122">Dynamics 365 (如需詳細深入資訊，請參閱 Azure SOC 2 Type 2 證明報告)</span><span class="sxs-lookup"><span data-stu-id="be149-122">Dynamics 365 (for detailed insight, see Azure SOC 2 Type 2 attestation report)</span></span>
- <span data-ttu-id="be149-123">Microsoft 365 Defender</span><span class="sxs-lookup"><span data-stu-id="be149-123">Microsoft 365 Defender</span></span>
- <span data-ttu-id="be149-124">Microsoft 雲端 App 安全性 (MCAS)</span><span class="sxs-lookup"><span data-stu-id="be149-124">Microsoft Cloud App Security (MCAS)</span></span>
- <span data-ttu-id="be149-125">適用於端點的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="be149-125">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="be149-126">適用於身分識別的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="be149-126">Microsoft Defender for Identity</span></span>
- <span data-ttu-id="be149-127">Microsoft Forms Pro (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="be149-127">Microsoft Forms Pro (not in scope for Azure Government)</span></span>
- <span data-ttu-id="be149-128">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="be149-128">Microsoft Graph</span></span>
- <span data-ttu-id="be149-129">Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="be149-129">Microsoft Intune</span></span>
- <span data-ttu-id="be149-130">Microsoft 受管理的電腦 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="be149-130">Microsoft Managed Desktop (not in scope for Azure Government)</span></span>
- <span data-ttu-id="be149-131">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="be149-131">Microsoft Stream</span></span>
- <span data-ttu-id="be149-132">Microsoft 威脅專家 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="be149-132">Microsoft Threat Experts (not in scope for Azure Government)</span></span>
- <span data-ttu-id="be149-133">提名入口網站</span><span class="sxs-lookup"><span data-stu-id="be149-133">Nomination Portal</span></span>
- <span data-ttu-id="be149-134">Office 365、Office 365 美國政府版、Office 365 美國政府版 - High、Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="be149-134">Office 365, Office 365 U.S. Government, Office 365 U.S. Government - High, Office 365 U.S. Government Defense</span></span>
- <span data-ttu-id="be149-135">Power Apps</span><span class="sxs-lookup"><span data-stu-id="be149-135">Power Apps</span></span>
- <span data-ttu-id="be149-136">電源自動化</span><span class="sxs-lookup"><span data-stu-id="be149-136">Power Automate</span></span>
- <span data-ttu-id="be149-137">Power BI</span><span class="sxs-lookup"><span data-stu-id="be149-137">Power BI</span></span>
- <span data-ttu-id="be149-138">Power Virtual Agent (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="be149-138">Power Virtual Agents (not in scope for Azure Government)</span></span>
- <span data-ttu-id="be149-139">更新合規性 (不在 Azure Government 的範圍內)</span><span class="sxs-lookup"><span data-stu-id="be149-139">Update Compliance (not in scope for Azure Government)</span></span>

## <a name="azure-dynamics-365-and-soc-2"></a><span data-ttu-id="be149-140">Azure、Dynamics 365 和 SOC 2</span><span class="sxs-lookup"><span data-stu-id="be149-140">Azure, Dynamics 365, and SOC 2</span></span>

<span data-ttu-id="be149-141">如需 Azure、Dynamics 365 及其他線上服務合規性詳細資訊，請參閱 [Azure SOC 2 方案](/azure/compliance/offerings/offering-soc-2)。</span><span class="sxs-lookup"><span data-stu-id="be149-141">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure SOC 2 offering](/azure/compliance/offerings/offering-soc-2).</span></span>

## <a name="office-365-and-soc-2"></a><span data-ttu-id="be149-142">Office 365 和 SOC 2</span><span class="sxs-lookup"><span data-stu-id="be149-142">Office 365 and SOC 2</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="be149-143">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="be149-143">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="be149-144">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="be149-144">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="be149-145">使用下表判斷 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="be149-145">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="be149-146">**適用性**</span><span class="sxs-lookup"><span data-stu-id="be149-146">**Applicability**</span></span> | <span data-ttu-id="be149-147">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="be149-147">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="be149-148">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="be149-148">**Office 365**</span></span> | <span data-ttu-id="be149-149">合規性管理員、客戶 Lockbox、Delve、Exchange Online Protection、Exchange Online、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Teams、MyAnalytics、Office 365 客戶入口網站、Office 365 微服務 (包括但不限於 Kaizala、ObjectStore、Sway、PowerPoint Online 文件服務、查詢註釋服務、學校資料同步處理、Siphon、語音、StaffHub、eXtensible Application Program)、Office Online、Office Services 基礎結構、商務用 OneDrive，Planner，PowerApps，Power Automate，Power BI，Project Online，客戶金鑰服務加密，SharePoint Online，商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="be149-149">Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Teams, MyAnalytics, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office Online, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Customer Key, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="be149-150">**GCC**</span><span class="sxs-lookup"><span data-stu-id="be149-150">**GCC**</span></span> | <span data-ttu-id="be149-151">Azure Active Directory、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="be149-151">Azure Active Directory, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="be149-152">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="be149-152">**GCC High**</span></span> | <span data-ttu-id="be149-153">Azure Active Directory、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="be149-153">Azure Active Directory, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="be149-154">**DoD**</span><span class="sxs-lookup"><span data-stu-id="be149-154">**DoD**</span></span> | <span data-ttu-id="be149-155">Azure Active Directory、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office Pro Plus、商務用 OneDrive、Planner、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="be149-155">Azure Active Directory, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power BI, SharePoint Online, Skype for Business</span></span> |

### <a name="office-365-audit-reports"></a><span data-ttu-id="be149-156">Office 365 稽核報告</span><span class="sxs-lookup"><span data-stu-id="be149-156">Office 365 audit reports</span></span>

- [<span data-ttu-id="be149-157">Office 365 核心版 - SSAE 18 SOC 2 報告</span><span class="sxs-lookup"><span data-stu-id="be149-157">Office 365 Core - SSAE 18 SOC 2 Report</span></span>](https://aka.ms/o365SOC-2)
- [<span data-ttu-id="be149-158">Office 365 微服務 T1-SSAE 18 SOC2 Type I 報告</span><span class="sxs-lookup"><span data-stu-id="be149-158">Office 365 Microservices T1-SSAE 18 SOC2 Type I Report</span></span>](https://aka.ms/o365-MS-SOC-2-type1)
- [<span data-ttu-id="be149-159">請參閱 Bridge Letter 和其他稽核報告</span><span class="sxs-lookup"><span data-stu-id="be149-159">See bridge letters and additional audit reports</span></span>](https://aka.ms/auditreports)

<span data-ttu-id="be149-160">您必須在 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府中擁有現有的訂閱或免費試用帳戶，才能下載 SOC 1 和 SOC 2 證明報告，以及任何橋接信件 (如果需要)。</span><span class="sxs-lookup"><span data-stu-id="be149-160">You must have an existing subscription or free trial account in Office 365 or [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 U.S. Government to download SOC 1 and SOC 2 attestation reports and any bridge letters as needed.</span></span>

### <a name="frequently-asked-questions"></a><span data-ttu-id="be149-161">常見問題集</span><span class="sxs-lookup"><span data-stu-id="be149-161">Frequently asked questions</span></span>

<span data-ttu-id="be149-162">**Office 365 SOC 報告多久發行一次？**</span><span class="sxs-lookup"><span data-stu-id="be149-162">**How often are Office 365 SOC reports issued?**</span></span>

<span data-ttu-id="be149-163">Office 365 和其他線上服務的 SOC 報告皆以 12 個月執行 (稽核期間) 為基礎，且每半年發行一次新報告 (期間結束於 3 月 31 日與 9 月 30 日)。</span><span class="sxs-lookup"><span data-stu-id="be149-163">SOC reports for Office 365 and other online services are based on a rolling 12-month run window (audit period) with new reports issued semi-annually (period ends are March 31 and September 30).</span></span> <span data-ttu-id="be149-164">每季都會發放 *橋接信件*，以涵蓋前三個月的內容。</span><span class="sxs-lookup"><span data-stu-id="be149-164">*Bridge letters* are issued each quarter to cover the prior three-month period.</span></span> <span data-ttu-id="be149-165">例如，1 月信件涵蓋 10 月 1 日到 12 月 31 日，4 月信件涵蓋 1 月 1 日到 3 月 31 日，7 月信件涵蓋 4 月 1 日到 6 月 30 日，而 10 月信件涵蓋 7 月 1 日到 9 月 30 日。</span><span class="sxs-lookup"><span data-stu-id="be149-165">For example, the January letter covers 1-Oct through 31-Dec, the April letter covers 1-Jan through 31-Mar, the July letter covers 1-Apr through 30-Jun, and the October letter covers 1-Jul through 30-Sep.</span></span>

<span data-ttu-id="be149-166">**我可以在哪裡取得 Office 365 SOC 稽核文件，包括橋接信件？**</span><span class="sxs-lookup"><span data-stu-id="be149-166">**Where can I get the Office 365 SOC audit documentation including bridge letters?**</span></span>

<span data-ttu-id="be149-167">如需稽核文件的連結，請參閱稽核報告一節。</span><span class="sxs-lookup"><span data-stu-id="be149-167">For links to audit documentation, see the audit report section.</span></span> <span data-ttu-id="be149-168">您必須擁有 Office 365 或 [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 美國政府的現有訂閱或免費試用帳戶才能登入。</span><span class="sxs-lookup"><span data-stu-id="be149-168">You must have an existing subscription or free trial account in Office 365or [Office](https://azure.microsoft.com/global-infrastructure/government/request/) 365 U.S. Government to log in.</span></span> <span data-ttu-id="be149-169">然後，您可以下載稽核憑證、評定報告及其他適用的文件，協助您符合自己的法規需求。</span><span class="sxs-lookup"><span data-stu-id="be149-169">You can then download audit certificates, assessment reports, and other applicable documents to help you with your own regulatory requirements.</span></span>

<span data-ttu-id="be149-170">**我可以在哪裡找到雲端安全性聯盟 CCM 控制措施的評定？**</span><span class="sxs-lookup"><span data-stu-id="be149-170">**Where can I find an assessment of the Cloud Security Alliance CCM controls implementation?**</span></span>

<span data-ttu-id="be149-171">Office 365 SOC 2 Type 2 稽核是根據美國會計師協會 (AICPA) 信任服務原則與準則 (包括安全性、可用性、機密性、隱私權和處理完整性) 以及雲端安全聯盟 (CSA) 雲端控制矩陣 (CCM) 中的準則所建立。</span><span class="sxs-lookup"><span data-stu-id="be149-171">The Office 365 SOC 2 Type 2 audit is based on the American Institute of Certified Public Accountants (AICPA) Trust Services Principles and Criteria, including security, availability, confidentiality, privacy, and processing integrity, and the criteria in the Cloud Security Alliance (CSA) Cloud Controls Matrix (CCM).</span></span> <span data-ttu-id="be149-172">目標是同時符合上述的 AICPA 準則和 CCM 中規定的需求。</span><span class="sxs-lookup"><span data-stu-id="be149-172">The objective is to meet both the AICPA criteria and requirements set forth in the CCM.</span></span> <span data-ttu-id="be149-173">Office 365 SOC 2 Type 2 稽核會納入 CSA STAR 證明所需的 CCM 控制措施評定。</span><span class="sxs-lookup"><span data-stu-id="be149-173">The Office 365 SOC 2 Type 2 audit incorporates the CCM controls assessment as required by the CSA STAR Attestation.</span></span> <span data-ttu-id="be149-174">如需詳細資訊，請參閱 Office 365 SOC 2 Type 2 證明報告。</span><span class="sxs-lookup"><span data-stu-id="be149-174">For more information, see the Office 365 SOC 2 Type 2 attestation report.</span></span>

<span data-ttu-id="be149-175">**我可以在哪裡查看已注意到的例外狀況管理回應？**</span><span class="sxs-lookup"><span data-stu-id="be149-175">**Where can I see management responses to exceptions noted?**</span></span>

<span data-ttu-id="be149-176">管理回應位於 SOC 證明報告的結尾處。</span><span class="sxs-lookup"><span data-stu-id="be149-176">Management responses are located towards the end of the SOC attestation report.</span></span> <span data-ttu-id="be149-177">在文件中搜尋「管理回應」。</span><span class="sxs-lookup"><span data-stu-id="be149-177">Search the document for 'Management Response'.</span></span>

<span data-ttu-id="be149-178">**我可以在哪裡查看使用者實體職責？**</span><span class="sxs-lookup"><span data-stu-id="be149-178">**Where can I see user entity responsibilities?**</span></span>

<span data-ttu-id="be149-179">使用者實體職責位於 SOC 證明報告的結尾。</span><span class="sxs-lookup"><span data-stu-id="be149-179">User entity responsibilities are located at the very end of the SOC attestation report.</span></span> <span data-ttu-id="be149-180">在文件中搜尋「使用者實體職責」。</span><span class="sxs-lookup"><span data-stu-id="be149-180">Search the document for 'User Entity Responsibilities'.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="be149-181">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="be149-181">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="be149-182">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="be149-182">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="be149-183">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="be149-183">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="be149-184">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="be149-184">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="be149-185">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="be149-185">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="be149-186">資源</span><span class="sxs-lookup"><span data-stu-id="be149-186">Resources</span></span>

- [<span data-ttu-id="be149-187">服務信任入口網站稽核報告</span><span class="sxs-lookup"><span data-stu-id="be149-187">Service Trust Portal audit reports</span></span>](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3)
- [<span data-ttu-id="be149-188">適用於服務組織的 AICPA SOC</span><span class="sxs-lookup"><span data-stu-id="be149-188">AICPA SOC for Service Organizations</span></span>](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/socforserviceorganizations.html)
- [<span data-ttu-id="be149-189">SSAE 第 18 號，證明標準：釐清與重新編纂 (AICPA 專業標準)</span><span class="sxs-lookup"><span data-stu-id="be149-189">SSAE No. 18, Attestation Standards: Clarification and Recodification (AICPA Professional Standards)</span></span>](https://www.aicpa.org/Research/Standards/AuditAttest/DownloadableDocuments/SSAE_No_18.pdf)
- <span data-ttu-id="be149-190">[SOC 2 報告服務組織與安全性、可用性、處理完整性、機密性或隱私權相關的控制措施檢查 (AICPA 指南)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (可供購買)</span><span class="sxs-lookup"><span data-stu-id="be149-190">[SOC 2 Reporting on an Examination of Controls at a Service Organization Relevant to Security, Availability, Processing Integrity, Confidentiality, or Privacy (AICPA Guide)](https://future.aicpa.org/cpe-learning/publication/soc-2-reporting-on-an-examination-of-controls-at-a-service-organization-relevant-to-security-availability-processing-integrity-confidentiality-or-privacy-OPL) (available for purchase)</span></span>
- [<span data-ttu-id="be149-191">TSP 第 100 節 (AICPA，2017 年信任服務準則)</span><span class="sxs-lookup"><span data-stu-id="be149-191">TSP section 100 (AICPA, 2017 Trust Services Criteria)</span></span>](https://www.aicpa.org/content/dam/aicpa/interestareas/frc/assuranceadvisoryservices/downloadabledocuments/trust-services-criteria.pdf)
