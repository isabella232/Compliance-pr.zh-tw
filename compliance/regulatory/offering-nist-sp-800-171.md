---
title: NIST SP 800-171
description: Microsoft 雲端服務遵循 NIST SP 800-171 指導方針，以保護 nonfederal 資訊系統中受控制的未分類資訊 (CUI) 。
keywords: Microsoft 365、合規性、方案
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
ms.openlocfilehash: 19b312d1b9f31683d775049010d390710554df01
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385663"
---
# <a name="nist-sp-800-171"></a><span data-ttu-id="7a614-104">NIST SP 800-171</span><span class="sxs-lookup"><span data-stu-id="7a614-104">NIST SP 800-171</span></span>

## <a name="about-nist-sp-800-171"></a><span data-ttu-id="7a614-105">關於 NIST SP 800-171</span><span class="sxs-lookup"><span data-stu-id="7a614-105">About NIST SP 800-171</span></span>

<span data-ttu-id="7a614-106">美國國家標準和技術協會 (NIST) 會促進及維護度量標準和準則，以協助保護聯邦機構的資訊和資訊系統。</span><span class="sxs-lookup"><span data-stu-id="7a614-106">The US National Institute of Standards and Technology (NIST) promotes and maintains measurement standards and guidelines to help protect the information and information systems of federal agencies.</span></span> <span data-ttu-id="7a614-107">如需管理受控未分類資訊的管理順序 13556 (CUI) ，它已發佈 [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-1/final)， *保護 Nonfederal 資訊系統和組織中的受控未分類資訊*。</span><span class="sxs-lookup"><span data-stu-id="7a614-107">In response to Executive Order 13556 on managing controlled unclassified information (CUI), it published [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-1/final), *Protecting Controlled Unclassified Information In Nonfederal Information Systems and Organizations*.</span></span> <span data-ttu-id="7a614-108">CUI 是定義為由政府 (或其代表) 所建立的資訊，但不是保密的，但仍然機密且需要保護。</span><span class="sxs-lookup"><span data-stu-id="7a614-108">CUI is defined as information, both digital and physical, created by a government (or an entity on its behalf) that, while not classified, is still sensitive and requires protection.</span></span>

<span data-ttu-id="7a614-109">NIST SP 800-171 最初發佈于6月2015，已于此後更新數次，以回應演變的 cyberthreats。</span><span class="sxs-lookup"><span data-stu-id="7a614-109">NIST SP 800-171 was originally published in June 2015 and has been updated several times since then in response to evolving cyberthreats.</span></span> <span data-ttu-id="7a614-110">它提供有關如何在 nonfederal 資訊系統和組織中安全地存取、傳送和儲存 CUI 的指導方針;其需求分為四個主要類別：</span><span class="sxs-lookup"><span data-stu-id="7a614-110">It provides guidelines on how CUI should be securely accessed, transmitted, and stored in nonfederal information systems and organizations; its requirements fall into four main categories:</span></span>

- <span data-ttu-id="7a614-111">管理及保護的控制項和程式</span><span class="sxs-lookup"><span data-stu-id="7a614-111">Controls and processes for managing and protecting</span></span>
- <span data-ttu-id="7a614-112">IT 系統的監控與管理</span><span class="sxs-lookup"><span data-stu-id="7a614-112">Monitoring and management of IT systems</span></span>
- <span data-ttu-id="7a614-113">適用于使用者的清晰做法和程式</span><span class="sxs-lookup"><span data-stu-id="7a614-113">Clear practices and procedures for end users</span></span>
- <span data-ttu-id="7a614-114">技術和實體安全性措施的實施</span><span class="sxs-lookup"><span data-stu-id="7a614-114">Implementation of technological and physical security measures</span></span>

## <a name="microsoft-and-nist-sp-800-171"></a><span data-ttu-id="7a614-115">Microsoft 和 NIST SP 800-171</span><span class="sxs-lookup"><span data-stu-id="7a614-115">Microsoft and NIST SP 800-171</span></span>

<span data-ttu-id="7a614-116">已取得協力廠商評估組織，Kratos Secureinfo 和 Coalfire，與 Microsoft 合作以證明其範圍內的雲端服務符合 NIST SP 800-171 中的準則， *保護受控未分類資訊 (CUI) 在 Nonfederal 資訊系統和組織中* 處理 CUI。</span><span class="sxs-lookup"><span data-stu-id="7a614-116">Accredited third-party assessment organizations, Kratos Secureinfo and Coalfire, partnered with Microsoft to attest that its in-scope cloud services meet the criteria in NIST SP 800-171, *Protecting Controlled Unclassified Information (CUI) in Nonfederal Information Systems and Organizations*, when they process CUI.</span></span> <span data-ttu-id="7a614-117">[Microsoft 對 FedRAMP](offering-fedramp.md)需求的實施，可協助確保 Microsoft 內部的雲端服務使用已到位的系統和做法，符合或超過 NIST SP 800-171 的需求。</span><span class="sxs-lookup"><span data-stu-id="7a614-117">The [Microsoft implementation of FedRAMP](offering-fedramp.md) requirements help ensure Microsoft in-scope cloud services meet or exceed the requirements of NIST SP 800-171 using the systems and practices already in place.</span></span>

<span data-ttu-id="7a614-118">NIST SP 800-171 的需求是 NIST SP 800-53 （FedRAMP 使用的標準）的子集。</span><span class="sxs-lookup"><span data-stu-id="7a614-118">NIST SP 800-171 requirements are a subset of NIST SP 800-53, the standard that FedRAMP uses.</span></span> <span data-ttu-id="7a614-119">NIST SP 800-171 的附錄 D 可將其 CUI 安全性需求直接對應至 NIST SP 800-53 中的相關安全性控制，其範圍內的雲端服務已在 FedRAMP 程式下評估並授權。</span><span class="sxs-lookup"><span data-stu-id="7a614-119">Appendix D of NIST SP 800-171 provides a direct mapping of its CUI security requirements to the relevant security controls in NIST SP 800-53, for which the in-scope cloud services have already been assessed and authorized under the FedRAMP program.</span></span>

<span data-ttu-id="7a614-120">任何處理或儲存我們政府 CUI 的實體（調研機構、諮詢公司、製造合同工）都必須遵守 NIST SP 800-171 的嚴格需求。</span><span class="sxs-lookup"><span data-stu-id="7a614-120">Any entity that processes or stores US government CUI — research institutions, consulting companies, manufacturing contractors, must comply with the stringent requirements of NIST SP 800-171.</span></span> <span data-ttu-id="7a614-121">這項證明意味著 Microsoft in 範圍的雲端服務可讓客戶在尋求部署 CUI 工作負載時，確保 Microsoft 符合完全規範。</span><span class="sxs-lookup"><span data-stu-id="7a614-121">This attestation means Microsoft in-scope cloud services can accommodate customers looking to deploy CUI workloads with the assurance that Microsoft is in full compliance.</span></span> <span data-ttu-id="7a614-122">例如，在其資訊系統中使用內部範圍的 Microsoft 雲端服務處理、儲存或傳輸「涵蓋的防禦資訊」的所有 DoD 承包商，都符合美國國防部 DFARS 子句，需要符合 NIST SP 800-171 的安全性需求。</span><span class="sxs-lookup"><span data-stu-id="7a614-122">For example, all DoD contractors who process, store, or transmit 'covered defense information' using in-scope Microsoft cloud services in their information systems meet the US Department of Defense DFARS clauses that require compliance with the security requirements of NIST SP 800-171.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="7a614-123">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="7a614-123">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="7a614-124">Azure 商用，Azure 政府版</span><span class="sxs-lookup"><span data-stu-id="7a614-124">Azure Commercial, Azure Government</span></span>
- <span data-ttu-id="7a614-125">美國政府的 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="7a614-125">Dynamics 365 U.S. Government</span></span>
- <span data-ttu-id="7a614-126">Intune</span><span class="sxs-lookup"><span data-stu-id="7a614-126">Intune</span></span>
- <span data-ttu-id="7a614-127">Office 365U.S. 政府社群雲端 (GCC) 、Office 365 GCC 高及 DoD</span><span class="sxs-lookup"><span data-stu-id="7a614-127">Office 365 U.S. Government Community Cloud (GCC), Office 365 GCC High, and DoD</span></span>

## <a name="azure-dynamics-365-and-nist-sp-800-171"></a><span data-ttu-id="7a614-128">Azure、Dynamics 365 和 NIST SP 800-171</span><span class="sxs-lookup"><span data-stu-id="7a614-128">Azure, Dynamics 365, and NIST SP 800-171</span></span>

<span data-ttu-id="7a614-129">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE NIST SP 800-171 服務](/azure/compliance/offerings/offering-nist-800-171)。</span><span class="sxs-lookup"><span data-stu-id="7a614-129">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure NIST SP 800-171 offering](/azure/compliance/offerings/offering-nist-800-171).</span></span>

## <a name="office-365-and-nist-sp-800-171"></a><span data-ttu-id="7a614-130">Office 365 和 NIST SP 800-171</span><span class="sxs-lookup"><span data-stu-id="7a614-130">Office 365 and NIST SP 800-171</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="7a614-131">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="7a614-131">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="7a614-132">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="7a614-132">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="7a614-133">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="7a614-133">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="7a614-134">**適用性**</span><span class="sxs-lookup"><span data-stu-id="7a614-134">**Applicability**</span></span> | <span data-ttu-id="7a614-135">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="7a614-135">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="7a614-136">**GCC**</span><span class="sxs-lookup"><span data-stu-id="7a614-136">**GCC**</span></span> | <span data-ttu-id="7a614-137">活動摘要服務，Bing 服務，Delve，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="7a614-137">Activity Feed Service, Bing Services, Delve, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |
| <span data-ttu-id="7a614-138">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="7a614-138">**GCC High**</span></span> | <span data-ttu-id="7a614-139">活動摘要服務，Bing 服務，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、</span><span class="sxs-lookup"><span data-stu-id="7a614-139">Activity Feed Service, Bing Services, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card,</span></span> 
<span data-ttu-id="7a614-140">SharePoint線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="7a614-140">SharePoint Online, Skype for Business, Windows Ink</span></span> |
| <span data-ttu-id="7a614-141">**DoD**</span><span class="sxs-lookup"><span data-stu-id="7a614-141">**DoD**</span></span> | <span data-ttu-id="7a614-142">活動摘要服務，Bing 服務，Exchange Online，智慧服務，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用方式報告、商務用 OneDrive、人員卡片、Microsoft Teams、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="7a614-142">Activity Feed Service, Bing Services, Exchange Online, Intelligent Services, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, Microsoft Teams, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="frequently-asked-questions"></a><span data-ttu-id="7a614-143">常見問題集</span><span class="sxs-lookup"><span data-stu-id="7a614-143">Frequently asked questions</span></span>

<span data-ttu-id="7a614-144">**我可以使用 Microsoft 對我的組織使用 NIST SP 800-171 的規範嗎？**</span><span class="sxs-lookup"><span data-stu-id="7a614-144">**Can I use Microsoft compliance with NIST SP 800-171 for my organization?**</span></span>

<span data-ttu-id="7a614-145">是。</span><span class="sxs-lookup"><span data-stu-id="7a614-145">Yes.</span></span> <span data-ttu-id="7a614-146">Microsoft 客戶可以使用來自獨立協力廠商評估組織的報告中所述的審核控制項， (3PAO) FedRAMP 標準的一部分 FedRAMP 及 NIST 風險分析和資格工作。</span><span class="sxs-lookup"><span data-stu-id="7a614-146">Microsoft customers may use the audited controls described in the reports from independent third-party assessment organizations (3PAO) on FedRAMP standards as part of their own FedRAMP and NIST risk analysis and qualification efforts.</span></span> <span data-ttu-id="7a614-147">這些報告證明 Microsoft 已在其範圍內雲端服務中實施之控制項的效能。</span><span class="sxs-lookup"><span data-stu-id="7a614-147">These reports attest to the effectiveness of the controls Microsoft has implemented in its in-scope cloud services.</span></span> <span data-ttu-id="7a614-148">客戶負責確保其 CUI 工作負載符合 NIST SP 800-171 指導方針。</span><span class="sxs-lookup"><span data-stu-id="7a614-148">Customers are responsible for ensuring that their CUI workloads comply with NIST SP 800-171 guidelines.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="7a614-149">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="7a614-149">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="7a614-150">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="7a614-150">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="7a614-151">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="7a614-151">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="7a614-152">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="7a614-152">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="7a614-153">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="7a614-153">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="7a614-154">資源</span><span class="sxs-lookup"><span data-stu-id="7a614-154">Resources</span></span>

- [<span data-ttu-id="7a614-155">Microsoft DoD 認證符合 NIST 800-171 的需求</span><span class="sxs-lookup"><span data-stu-id="7a614-155">Microsoft DoD Certification Meets NIST 800-171 Requirements</span></span>](offering-DoD-DISA-L2-L4-L5.md)
- [<span data-ttu-id="7a614-156">NIST 800-171 合規性始于 Cybersecurity 檔</span><span class="sxs-lookup"><span data-stu-id="7a614-156">NIST 800-171 Compliance Starts with Cybersecurity Documentation</span></span>](https://www.nist800171.com/)
- [<span data-ttu-id="7a614-157">Microsoft Cloud Services FedRAMP 授權</span><span class="sxs-lookup"><span data-stu-id="7a614-157">Microsoft Cloud Services FedRAMP Authorizations</span></span>](https://marketplace.fedramp.gov/index.html?status=Compliant&sort=productName#/products)
- [<span data-ttu-id="7a614-158">NIST 800-171 3.3 審計和責任制 Office 365 GCC 高</span><span class="sxs-lookup"><span data-stu-id="7a614-158">NIST 800-171 3.3 Audit and Accountability with Office 365 GCC High</span></span>](https://info.summit7systems.com/blog/nist-3.3-audit-and-accountability-with-office-365)
- [<span data-ttu-id="7a614-159">Microsoft 和 NIST Cybersecurity Framework</span><span class="sxs-lookup"><span data-stu-id="7a614-159">Microsoft and the NIST Cybersecurity Framework</span></span>](offering-nist-csf.md)
- [<span data-ttu-id="7a614-160">Microsoft 政府雲端</span><span class="sxs-lookup"><span data-stu-id="7a614-160">Microsoft Government Cloud</span></span>](https://www.microsoft.com/enterprise/government)
- [<span data-ttu-id="7a614-161">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="7a614-161">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
