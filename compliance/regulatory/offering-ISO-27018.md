---
title: 保護雲端中個人資料的 ISO/IEC 27018 工作條例規定
description: Microsoft 是第一個遵守此雲端隱私權工作條例規定的雲端提供者。
keywords: Microsoft 365, 合規性, 方案
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
ms.openlocfilehash: 579e300213f15d6416b7c0c8f9d37668c9934faa
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384733"
---
# <a name="isoiec-27018-code-of-practice-for-protecting-personal-data-in-the-cloud"></a><span data-ttu-id="abef3-104">保護雲端中個人資料的 ISO/IEC 27018 工作條例規定</span><span class="sxs-lookup"><span data-stu-id="abef3-104">ISO/IEC 27018 Code of Practice for Protecting Personal Data in the Cloud</span></span>

## <a name="isoiec-27018-overview"></a><span data-ttu-id="abef3-105">ISO/IEC 27018 概觀</span><span class="sxs-lookup"><span data-stu-id="abef3-105">ISO/IEC 27018 overview</span></span>

<span data-ttu-id="abef3-106">國際標準組織 (ISO) 是獨立的非政府組織，以及全球最大的自願性國際標準開發者。</span><span class="sxs-lookup"><span data-stu-id="abef3-106">The International Organization for Standardization (ISO) is an independent nongovernmental organization and the world's largest developer of voluntary international standards.</span></span> <span data-ttu-id="abef3-107">ISO/IEC 27000 標準系列可幫助各類型跟大小的組織保持資訊資產安全。</span><span class="sxs-lookup"><span data-stu-id="abef3-107">The ISO/IEC 27000 family of standards helps organizations of every type and size keep information assets secure.</span></span>

<span data-ttu-id="abef3-108">ISO 在 2014 年採用 ISO/IEC 27018:2014，此為 ISO/IEC 27001 的增補合約，並為雲端隱私權的第一個國際工作條例規定。</span><span class="sxs-lookup"><span data-stu-id="abef3-108">In 2014, the ISO adopted ISO/IEC 27018:2014, an addendum to ISO/IEC 27001, the first international code of practice for cloud privacy.</span></span> <span data-ttu-id="abef3-109">根據歐盟資料保護規定，它對作為個人識別資訊 (PII) 處理者的雲端服務提供者 (CSP) 提供特定指引，為保護 PII 評估風險和實作最先進的控制措施。</span><span class="sxs-lookup"><span data-stu-id="abef3-109">Based on EU data-protection laws, it gives specific guidance to cloud service providers (CSPs) acting as processors of personally identifiable information (PII) on assessing risks and implementing state-of-the-art controls for protecting PII.</span></span>

<span data-ttu-id="abef3-110">Microsoft 和 ISO/IEC 27018</span><span class="sxs-lookup"><span data-stu-id="abef3-110">Microsoft and ISO/IEC 27018</span></span>

<span data-ttu-id="abef3-111">在適用之獨立驗證的安全控制有實施並有效運作的情況下，合格的第三方驗證實體每年至少一次會稽核 Microsoft Azure 和 Azure 德國，已確定其 ISO/IEC 27001 與 ISO/IEC 27018 的合規性。</span><span class="sxs-lookup"><span data-stu-id="abef3-111">At least once a year, Microsoft Azure and Azure Germany are audited for compliance with ISO/IEC 27001 and ISO/IEC 27018 by an accredited third-party certification body, providing independent validation that applicable security controls are in place and operating effectively.</span></span> <span data-ttu-id="abef3-112">稽核者身為合規性驗證程序之一部分，在適用聲明中確認 Microsoft 範圍內雲端服務和商業技術支援服務已合併 ISO/IEC 27018 控制，用來保護 Azure 中的 PII。</span><span class="sxs-lookup"><span data-stu-id="abef3-112">As part of this compliance verification process, the auditors validate in their statement of applicability that Microsoft in-scope cloud services and commercial technical support services have incorporated ISO/IEC 27018 controls for the protection of PII in Azure.</span></span> <span data-ttu-id="abef3-113">若要維持合規性，Microsoft 雲端服務必須每年接受第三方檢閱。</span><span class="sxs-lookup"><span data-stu-id="abef3-113">To remain compliant, Microsoft cloud services must be subject to annual third-party reviews.</span></span>

<span data-ttu-id="abef3-114">透過遵循 ISO/IEC 27001 的標準以及具體化於 ISO/IEC 27018 的工作條例規定，第一家合併此工作條例規定的主要雲端提供者 Microsoft 證明其隱私原則和程序是穩健且符合其高標準。</span><span class="sxs-lookup"><span data-stu-id="abef3-114">By following the standards of ISO/IEC 27001 and the code of practice embodied in ISO/IEC 27018, Microsoft (the first major cloud provider to incorporate this code of practice) demonstrates that its privacy policies and procedures are robust and in line with its high standards.</span></span>

- <span data-ttu-id="abef3-115">**Microsoft 雲端服務的客戶知道其資料儲存的位置。**</span><span class="sxs-lookup"><span data-stu-id="abef3-115">**Customers of Microsoft cloud services know where their data is stored.**</span></span> <span data-ttu-id="abef3-116">由於 ISO/IEC 27018 要求經認證的 CSP 通知客戶其資料可能儲存的國家/地區，因此 Microsoft 雲端服務客戶具有所需的可見度以遵循任何適用的資訊安全規則。</span><span class="sxs-lookup"><span data-stu-id="abef3-116">Because ISO/IEC 27018 requires certified CSPs to inform customers of the countries in which their data may be stored, Microsoft cloud service customers have the visibility they need to comply with any applicable information security rules.</span></span>
- <span data-ttu-id="abef3-117">**客戶資料不會沒有明確許可前即用來行銷或廣告。**</span><span class="sxs-lookup"><span data-stu-id="abef3-117">**Customer data won't be used for marketing or advertising without explicit consent.**</span></span> <span data-ttu-id="abef3-118">某些 CSP 使用客戶資料做為其個別的商業目的，包括目標廣告。</span><span class="sxs-lookup"><span data-stu-id="abef3-118">Some CSPs use customer data for their own commercial ends, including for targeted advertising.</span></span> <span data-ttu-id="abef3-119">由於 Microsoft 採用 ISO/IEC 27018 作為其範圍內企業雲端服務，因此客戶大可放心其資料永遠不會在明確許可前以此目的遭使用，而許可也不能成為雲端服務使用的條件。</span><span class="sxs-lookup"><span data-stu-id="abef3-119">Because Microsoft has adopted ISO/IEC 27018 for its in-scope enterprise cloud services, customers can rest assured that their data will never be used for such purposes without explicit consent, and that consent cannot be a condition for use of the cloud service.</span></span>
- <span data-ttu-id="abef3-120">**Microsoft 客戶知道其 PII 的現行狀況。**</span><span class="sxs-lookup"><span data-stu-id="abef3-120">**Microsoft customers know what's happening with their PII.**</span></span> <span data-ttu-id="abef3-121">ISO/IEC 27018 需要允許在合理的期間內傳回、轉移和安全處置個人資訊的原則。</span><span class="sxs-lookup"><span data-stu-id="abef3-121">ISO/IEC 27018 requires a policy that allows for the return, transfer, and secure disposal of personal information within a reasonable period of time.</span></span> <span data-ttu-id="abef3-122">如果 Microsoft 與其他需要存取客戶資料的公司合作，Microsoft 會主動地公開這些子處理者的身分識別。</span><span class="sxs-lookup"><span data-stu-id="abef3-122">If Microsoft works with other companies that need access to your customer data, Microsoft proactively discloses the identities of those sub-processors.</span></span>
- <span data-ttu-id="abef3-123">**Microsoft 僅遵循具有法律約束力之客戶資料公開的要求。**</span><span class="sxs-lookup"><span data-stu-id="abef3-123">**Microsoft complies only with legally binding requests for disclosure of customer data.**</span></span> <span data-ttu-id="abef3-124">如果 Microsoft 必須遵守這項要求 (例如犯罪調查)，我們一定會先行通知客戶，除非法律有所禁止。</span><span class="sxs-lookup"><span data-stu-id="abef3-124">If Microsoft must comply with such a request (as in the case of a criminal investigation), it will always notify the customer unless it is prohibited by law from doing so.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="abef3-125">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="abef3-125">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="abef3-126">Azure、Azure Government 和 Azure 德國</span><span class="sxs-lookup"><span data-stu-id="abef3-126">Azure, Azure Government, and Azure Germany</span></span>
- <span data-ttu-id="abef3-127">Azure DevOps Services</span><span class="sxs-lookup"><span data-stu-id="abef3-127">Azure DevOps Services</span></span>
- [<span data-ttu-id="abef3-128">Dynamics 365、Dynamics 365 和 Dynamics 365 Germany</span><span class="sxs-lookup"><span data-stu-id="abef3-128">Dynamics 365, Dynamics 365, and Dynamics 365 Germany</span></span>](https://aka.ms/d365-compliance-list)
- <span data-ttu-id="abef3-129">Intune</span><span class="sxs-lookup"><span data-stu-id="abef3-129">Intune</span></span>
- <span data-ttu-id="abef3-130">Microsoft 雲端應用程式安全性</span><span class="sxs-lookup"><span data-stu-id="abef3-130">Microsoft Cloud App Security</span></span>
- <span data-ttu-id="abef3-131">Microsoft 專業服務：Azure、Dynamics 365、Intune 及商務用 Microsoft 365 中型企業和企業客戶的頂級與內部部署</span><span class="sxs-lookup"><span data-stu-id="abef3-131">Microsoft Professional Services: Premier and On Premises for Azure, Dynamics 365, Intune, and for medium business and enterprise customers of Microsoft 365 for business</span></span>
- <span data-ttu-id="abef3-132">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="abef3-132">Microsoft Graph</span></span>
- <span data-ttu-id="abef3-133">Microsoft Healthcare Bot</span><span class="sxs-lookup"><span data-stu-id="abef3-133">Microsoft Healthcare Bot</span></span>
- [<span data-ttu-id="abef3-134">Microsoft 受管理的電腦</span><span class="sxs-lookup"><span data-stu-id="abef3-134">Microsoft Managed Desktop</span></span>](/microsoft-365/managed-desktop/intro/compliance)
- <span data-ttu-id="abef3-135">Microsoft 威脅專家</span><span class="sxs-lookup"><span data-stu-id="abef3-135">Microsoft Threat Experts</span></span>
- <span data-ttu-id="abef3-136">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="abef3-136">Microsoft Stream</span></span>
- <span data-ttu-id="abef3-137">Office 365、Office 365 美國政府和 Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="abef3-137">Office 365, Office 365 U.S. Government, and Office 365 U.S. Government Defense</span></span>
- <span data-ttu-id="abef3-138">Office 365 德國</span><span class="sxs-lookup"><span data-stu-id="abef3-138">Office 365 Germany</span></span>
- <span data-ttu-id="abef3-139">OMS 服務對應</span><span class="sxs-lookup"><span data-stu-id="abef3-139">OMS Service Map</span></span>
- <span data-ttu-id="abef3-140">Power Automate (先前為 Microsoft Flow) 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="abef3-140">Power Automate (formerly Microsoft Flow): cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="abef3-141">PowerApps 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="abef3-141">PowerApps cloud service: either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="abef3-142">Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="abef3-142">Power BI cloud service: either as a standalone service or as included in an Office 365 branded plan or suite</span></span>
- <span data-ttu-id="abef3-143">Power BI Embedded</span><span class="sxs-lookup"><span data-stu-id="abef3-143">Power BI Embedded</span></span>
- <span data-ttu-id="abef3-144">Power Virtual Agent</span><span class="sxs-lookup"><span data-stu-id="abef3-144">Power Virtual Agents</span></span>
- <span data-ttu-id="abef3-145">適用於端點的 Microsoft Defender: 端點偵測與回應、自動調查與補救、安全分數</span><span class="sxs-lookup"><span data-stu-id="abef3-145">Microsoft Defender for Endpoint: Endpoint Detection & Response, Automatic Investigation & Remediation, Secure Score</span></span>

## <a name="azure-dynamics-365-and-iso-isoiec-27018"></a><span data-ttu-id="abef3-146">Azure、Dynamics 365 和 ISO/IEC 27018</span><span class="sxs-lookup"><span data-stu-id="abef3-146">Azure, Dynamics 365, and ISO ISO/IEC 27018</span></span>

<span data-ttu-id="abef3-147">如需 Azure、Dynamics 365 及其他線上服務合規性的詳細資訊，請參閱 [Azure ISO/IEC 27018 供應項目](/azure/compliance/offerings/offering-iso-27018)。</span><span class="sxs-lookup"><span data-stu-id="abef3-147">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure ISO/IEC 27018 offering](/azure/compliance/offerings/offering-iso-27018).</span></span>

## <a name="office-365-and-iso-isoiec-27018"></a><span data-ttu-id="abef3-148">Office 365 和 ISO ISO/IEC 27018</span><span class="sxs-lookup"><span data-stu-id="abef3-148">Office 365 and ISO ISO/IEC 27018</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="abef3-149">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="abef3-149">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="abef3-150">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="abef3-150">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="abef3-151">使用下表判斷 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="abef3-151">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="abef3-152">**適用性**</span><span class="sxs-lookup"><span data-stu-id="abef3-152">**Applicability**</span></span> | <span data-ttu-id="abef3-153">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="abef3-153">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="abef3-154">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="abef3-154">**Office 365**</span></span> | <span data-ttu-id="abef3-155">Access Online、Azure Active Directory、Azure Communications Service、合規性管理員、客戶加密箱、Delve、Exchange Online Protection、Exchange Online、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Defender for Office 365、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 客戶入口網站、Office 365 微服務 (包含但不限 Kaizala、ObjectStore、Sway、PowerPoint Online Document Service、Query Annotation Service、學校資料同步處理、Siphon、Speech、StaffHub、eXtensible Application Program)、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、Office Services Infrastructure、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、Project Online、使用客戶金鑰的服務加密、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="abef3-155">Access Online, Azure Active Directory, Azure Communications Service, Compliance Manager, Customer Lockbox, Delve, Exchange Online Protection, Exchange Online, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office 365 Security & Compliance Center, Office Online, Office Pro Plus, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Customer Key, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="abef3-156">**GCC**</span><span class="sxs-lookup"><span data-stu-id="abef3-156">**GCC**</span></span> | <span data-ttu-id="abef3-157">Azure Active Directory、Azure Communications Service、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="abef3-157">Azure Active Directory, Azure Communications Service, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="abef3-158">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="abef3-158">**GCC High**</span></span> | <span data-ttu-id="abef3-159">Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="abef3-159">Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="abef3-160">**DoD**</span><span class="sxs-lookup"><span data-stu-id="abef3-160">**DoD**</span></span> | <span data-ttu-id="abef3-161">Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="abef3-161">Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power BI, SharePoint Online, Skype for Business</span></span> |

### <a name="office-365-audits-reports-and-certificates"></a><span data-ttu-id="abef3-162">Office 365 稽核、報告和認證</span><span class="sxs-lookup"><span data-stu-id="abef3-162">Office 365 Audits, reports, and certificates</span></span>

<span data-ttu-id="abef3-163">Microsoft 雲端和商業技術支援服務會一年根據 ISO/IEC 27018 工作條例規定進行一次稽核，以作為 ISO/IEC 27001 認證程序的一部分。</span><span class="sxs-lookup"><span data-stu-id="abef3-163">Microsoft cloud and commercial technical support services are audited once a year for the ISO/IEC 27018 code of practice as part of the certification process for ISO/IEC 27001.</span></span>

- [<span data-ttu-id="abef3-164">Office 365：ISO 27001、27018 和 27017 稽核評估報告</span><span class="sxs-lookup"><span data-stu-id="abef3-164">Office 365: ISO 27001, 27018, and 27017 Audit Assessment Report</span></span>](https://aka.ms/o365isoreport)
- [<span data-ttu-id="abef3-165">Yammer ISO 27018 稽核評定報告</span><span class="sxs-lookup"><span data-stu-id="abef3-165">Yammer ISO 27018 Audit Assessment Report</span></span>](https://aka.ms/YammerISO27018Auditreport)

### <a name="frequently-asked-questions"></a><span data-ttu-id="abef3-166">常見問題集</span><span class="sxs-lookup"><span data-stu-id="abef3-166">Frequently asked questions</span></span>

<span data-ttu-id="abef3-167">**ISO/IEC 27018 適用於何者？**</span><span class="sxs-lookup"><span data-stu-id="abef3-167">**To whom does ISO/IEC 27018 apply?**</span></span>

<span data-ttu-id="abef3-168">此工作條例規定適用於在其他組織合約之下處理 PII 的 CSP。</span><span class="sxs-lookup"><span data-stu-id="abef3-168">This code of practice applies to CSPs that process PII under contract for other organizations.</span></span> <span data-ttu-id="abef3-169">在 Microsoft，這也適用於對這些 CSP 的支援。</span><span class="sxs-lookup"><span data-stu-id="abef3-169">At Microsoft, it also applies to the support of these CSPs.</span></span>

<span data-ttu-id="abef3-170">**「個人資訊控制者」與「個人資訊處理者」有何不同？**</span><span class="sxs-lookup"><span data-stu-id="abef3-170">**What is the difference between 'personal information controllers' and 'personal information processors'?**</span></span>

<span data-ttu-id="abef3-171">在 ISO/IEC 27018 之中：</span><span class="sxs-lookup"><span data-stu-id="abef3-171">In the context of ISO/IEC 27018:</span></span>

- <span data-ttu-id="abef3-172">「控制者」控制個人資訊的集合、持有、處理或使用；它們包含代表另一家公司控制的人員。</span><span class="sxs-lookup"><span data-stu-id="abef3-172">'Controllers' control the collection, holding, processing, or use of personal information; they include those who control it on another company's behalf.</span></span>
- <span data-ttu-id="abef3-173">「處理者」則代表控制者處理資訊；它們不會針對如何使用資訊或處理目的做決策。</span><span class="sxs-lookup"><span data-stu-id="abef3-173">'Processors' process information on behalf of controllers; they do not make decisions as to how to use the information or the purposes of the processing.</span></span> <span data-ttu-id="abef3-174">Microsoft 做為您的供應商，是為您提供企業雲端服務的資訊處理者。</span><span class="sxs-lookup"><span data-stu-id="abef3-174">In providing its enterprise cloud services, Microsoft (as a vendor to you) is an information processor.</span></span>

<span data-ttu-id="abef3-175">**我可以在何處檢視 ISO/IEC 27018 的 Office 365 合規性資訊？**</span><span class="sxs-lookup"><span data-stu-id="abef3-175">**Where can I view Office 365 compliance information for ISO/IEC 27018?**</span></span>

- <span data-ttu-id="abef3-176">您可以檢閱 BSI (驗證 Microsoft 是否符合 ISO/IEC 27018 的獨立稽核者)為 [Office 365](https://aka.ms/Office365-Cert) 頒發的 ISO/IEC 27018 認證。</span><span class="sxs-lookup"><span data-stu-id="abef3-176">You can review the ISO/IEC 27018 certificates from BSI (the independent auditor that validated Microsoft compliance with ISO/IEC 27018) for [Office 365](https://aka.ms/Office365-Cert).</span></span>

<span data-ttu-id="abef3-177">**我是否可以在組織的認證程序中使用 Microsoft 合規性？**</span><span class="sxs-lookup"><span data-stu-id="abef3-177">**Can I use Microsoft's compliance in my organization's certification process?**</span></span>

<span data-ttu-id="abef3-p110">是的。如果 ISO/IEC 27018 合規性對您的企業和在任何 Microsoft 範圍內的企業雲端服務所部署的實作很重要，您可以在合規性評定中使用 Microsoft 的 ISO/IEC 27018 認證，並搭配 Microsoft 的 ISO/IEC 27001 認證。</span><span class="sxs-lookup"><span data-stu-id="abef3-p110">Yes. If compliance with ISO/IEC 27018 is important for your business and implementations deployed on any of Microsoft in-scope enterprise cloud services, you can use Microsoft's attestation of compliance with ISO/IEC 27018 with Microsoft's certification for ISO/IEC 27001 in your compliance assessment.</span></span>

<span data-ttu-id="abef3-180">不過，您有責任確保處理者有參與評估合規性的實作，以及組織中的控制和程序。</span><span class="sxs-lookup"><span data-stu-id="abef3-180">However, you are responsible for engaging an assessor to evaluate your implementation for compliance, and for the controls and processes within your own organization.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="abef3-181">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="abef3-181">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="abef3-182">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="abef3-182">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="abef3-183">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="abef3-183">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="abef3-184">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="abef3-184">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="abef3-185">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="abef3-185">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="abef3-186">資源</span><span class="sxs-lookup"><span data-stu-id="abef3-186">Resources</span></span>

- [<span data-ttu-id="abef3-187">ISO/IEC 27018:2014 工作條例規定</span><span class="sxs-lookup"><span data-stu-id="abef3-187">ISO/IEC 27018:2014 code of practice</span></span>](https://aka.ms/ISO.IEC_27018.2014)
- [<span data-ttu-id="abef3-188">Microsoft 通用控制措施中樞合規性架構</span><span class="sxs-lookup"><span data-stu-id="abef3-188">Microsoft Common Controls Hub Compliance Framework</span></span>](https://www.microsoft.com/trustcenter/common-controls-hub)
- [<span data-ttu-id="abef3-189">Microsoft 企業雲端和技術服務的資料存取原則</span><span class="sxs-lookup"><span data-stu-id="abef3-189">Data access policies for Microsoft enterprise cloud and technical services</span></span>](https://www.microsoft.com/trustcenter/Privacy/Who-can-access-your-data-and-on-what-terms)
- [<span data-ttu-id="abef3-190">Microsoft Online Services 條款</span><span class="sxs-lookup"><span data-stu-id="abef3-190">Microsoft Online Services Terms</span></span>](https://aka.ms/Online-Services-Terms)
- [<span data-ttu-id="abef3-191">Microsoft 政府雲端</span><span class="sxs-lookup"><span data-stu-id="abef3-191">Microsoft Government Cloud</span></span>](https://go.microsoft.com/fwlink/p/?linkid=2087246)
- [<span data-ttu-id="abef3-192">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="abef3-192">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
