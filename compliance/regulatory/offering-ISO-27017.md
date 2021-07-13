---
title: 資訊安全性控制的 ISO/IEC 27017:2015 工作條例規定
description: Microsoft 雲端服務已實作此「資訊安全性控制的工作條例規定」。
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
ms.openlocfilehash: 6c431d856fc03f328148722c14dfc558082aacb5
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384723"
---
# <a name="isoiec-270172015-code-of-practice-for-information-security-controls"></a><span data-ttu-id="3d35c-104">資訊安全性控制的 ISO/IEC 27017:2015 工作條例規定</span><span class="sxs-lookup"><span data-stu-id="3d35c-104">ISO/IEC 27017:2015 Code of Practice for Information Security Controls</span></span>

## <a name="iso-iec-27017-overview"></a><span data-ttu-id="3d35c-105">ISO-IEC 27017 概觀</span><span class="sxs-lookup"><span data-stu-id="3d35c-105">ISO-IEC 27017 Overview</span></span>

<span data-ttu-id="3d35c-106">ISO/IEC 27017:2015 工作條例規定專為組織設計，可在基於 ISO/IEC 27002:2013 實作雲端運算資訊安全管理系統時，用來做為選取雲端服務資訊安全性控制的參考。</span><span class="sxs-lookup"><span data-stu-id="3d35c-106">The ISO/IEC 27017:2015 code of practice is designed for organizations to use as a reference for selecting cloud services information security controls when implementing a cloud computing information security management system based on ISO/IEC 27002:2013.</span></span> <span data-ttu-id="3d35c-107">雲端服務提供者也可以使用它做為實作常見防護控制的指導方針文件。</span><span class="sxs-lookup"><span data-stu-id="3d35c-107">It can also be used by cloud service providers as a guidance document for implementing commonly accepted protection controls.</span></span>

<span data-ttu-id="3d35c-108">此國際標準提供基於 ISO/IEC 27002 的額外雲端特定實作指導方針，並提供額外的控制來處理雲端特定資訊安全性威脅和風險，請查閱 ISO/IEC 27002:2013 的條款 5 至 18 中相關的控制、實作指導方針及其他資訊。</span><span class="sxs-lookup"><span data-stu-id="3d35c-108">This international standard provides additional cloud-specific implementation guidance based on ISO/IEC 27002, and provides additional controls to address cloud-specific information security threats and risks referring to clauses 5-18 in ISO/IEC 27002: 2013 for controls, implementation guidance, and other information.</span></span> <span data-ttu-id="3d35c-109">具體來說，此標準提供 ISO/IEC 27002 中 37 項控制的指導方針，並提供未與 ISO/IEC 27002 中重複的七項新控制。</span><span class="sxs-lookup"><span data-stu-id="3d35c-109">Specifically, this standard provides guidance on 37 controls in ISO/IEC 27002, and it also features seven new controls that are not duplicated in ISO/IEC 27002.</span></span> <span data-ttu-id="3d35c-110">這些新的控制能解決下列重要領域：</span><span class="sxs-lookup"><span data-stu-id="3d35c-110">These new controls address the following important areas:</span></span>

- <span data-ttu-id="3d35c-111">雲端運算環境內的共同角色和責任</span><span class="sxs-lookup"><span data-stu-id="3d35c-111">Shared roles and responsibilities within a cloud computing environment</span></span>
- <span data-ttu-id="3d35c-112">在合約終止時移除並退回雲端服務客戶資產</span><span class="sxs-lookup"><span data-stu-id="3d35c-112">Removal and return of cloud service customer assets upon contract termination</span></span>
- <span data-ttu-id="3d35c-113">保護客戶的虛擬環境並與其他客戶的虛擬環境隔離</span><span class="sxs-lookup"><span data-stu-id="3d35c-113">Protection and separation of a customer's virtual environment from environments of other customers</span></span>
- <span data-ttu-id="3d35c-114">虛擬機器強化需求，以滿足商務需求</span><span class="sxs-lookup"><span data-stu-id="3d35c-114">Virtual machine hardening requirements to meet business needs</span></span>
- <span data-ttu-id="3d35c-115">雲端運算環境系統管理操作的程序</span><span class="sxs-lookup"><span data-stu-id="3d35c-115">Procedures for administrative operations of a cloud computing environment</span></span>
- <span data-ttu-id="3d35c-116">讓客戶能夠監視雲端運算環境內的相關活動</span><span class="sxs-lookup"><span data-stu-id="3d35c-116">Enabling customers to monitor relevant activities within a cloud computing environment</span></span>
- <span data-ttu-id="3d35c-117">結合虛擬和實體網路的安全性管理</span><span class="sxs-lookup"><span data-stu-id="3d35c-117">Alignment of security management for virtual and physical networks</span></span>

## <a name="microsoft-and-isoiec-27017"></a><span data-ttu-id="3d35c-118">Microsoft 和 ISO/IEC 27017</span><span class="sxs-lookup"><span data-stu-id="3d35c-118">Microsoft and ISO/IEC 27017</span></span>

<span data-ttu-id="3d35c-119">ISO/IEC 27017 在為雲端服務提供者和雲端服務客戶提供指導方針方面與眾不同。</span><span class="sxs-lookup"><span data-stu-id="3d35c-119">ISO/IEC 27017 is unique in providing guidance for both cloud service providers and cloud service customers.</span></span> <span data-ttu-id="3d35c-120">它也會為雲端服務客戶提供有關他們應該對雲端服務提供者所預期的實務資訊。</span><span class="sxs-lookup"><span data-stu-id="3d35c-120">It also provides cloud service customers with practical information on what they should expect from cloud service providers.</span></span> <span data-ttu-id="3d35c-121">透過確保客戶了解在雲端中的共用責任，客戶可以直接從 ISO/IEC 27017 獲益。</span><span class="sxs-lookup"><span data-stu-id="3d35c-121">Customers can benefit directly from ISO/IEC 27017 by ensuring they understand the shared responsibilities in the cloud.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="3d35c-122">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="3d35c-122">Microsoft in-scope cloud platforms & services</span></span>

- [<span data-ttu-id="3d35c-123">Azure、Azure Government 和 Azure 德國</span><span class="sxs-lookup"><span data-stu-id="3d35c-123">Azure, Azure Government, and Azure Germany</span></span>](https://aka.ms/AzureCompliance)
- <span data-ttu-id="3d35c-124">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="3d35c-124">Microsoft Cloud App Security</span></span>
- [<span data-ttu-id="3d35c-125">Dynamics 365、Dynamics 365 和 Dynamics 365 德國</span><span class="sxs-lookup"><span data-stu-id="3d35c-125">Dynamics 365, Dynamics 365, and Dynamics 365 Germany</span></span>](https://aka.ms/d365-compliance-list)
- <span data-ttu-id="3d35c-126">Intune</span><span class="sxs-lookup"><span data-stu-id="3d35c-126">Intune</span></span>
- <span data-ttu-id="3d35c-127">適用於端點的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="3d35c-127">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="3d35c-128">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3d35c-128">Microsoft Graph</span></span>
- <span data-ttu-id="3d35c-129">Microsoft Healthcare Bot</span><span class="sxs-lookup"><span data-stu-id="3d35c-129">Microsoft Healthcare Bot</span></span>
- [<span data-ttu-id="3d35c-130">Microsoft 受管理的電腦</span><span class="sxs-lookup"><span data-stu-id="3d35c-130">Microsoft Managed Desktop</span></span>](/microsoft-365/managed-desktop/intro/compliance)
- <span data-ttu-id="3d35c-131">Office 365、Office 365 美國政府、Office 365 美國政府國防版和 Office 365 Germany</span><span class="sxs-lookup"><span data-stu-id="3d35c-131">Office 365, Office 365 U.S. Government, Office 365 U.S. Government Defense, and Office 365 Germany</span></span>
- <span data-ttu-id="3d35c-132">Power Automate (先前為 Microsoft Flow) 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="3d35c-132">Power Automate (formerly Microsoft Flow) cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="3d35c-133">PowerApps 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="3d35c-133">PowerApps cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="3d35c-134">Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="3d35c-134">Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite</span></span>
- <span data-ttu-id="3d35c-135">Power BI Embedded</span><span class="sxs-lookup"><span data-stu-id="3d35c-135">Power BI Embedded</span></span>

## <a name="azure-dynamics-365-and-iso-270172015"></a><span data-ttu-id="3d35c-136">Azure、Dynamics 365 和 ISO 27017:2015</span><span class="sxs-lookup"><span data-stu-id="3d35c-136">Azure, Dynamics 365, and ISO 27017:2015</span></span>

<span data-ttu-id="3d35c-137">如需 Azure、Dynamics 365 及其他線上服務合規性的詳細資訊，請參閱 [Azure ISO 27017 供應項目](/azure/compliance/offerings/offering-iso-27017)。</span><span class="sxs-lookup"><span data-stu-id="3d35c-137">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure ISO 27017 offering](/azure/compliance/offerings/offering-iso-27017).</span></span>

## <a name="office-365-and-iso-270172015"></a><span data-ttu-id="3d35c-138">Office 365 和 ISO 27017:2015</span><span class="sxs-lookup"><span data-stu-id="3d35c-138">Office 365 and ISO 27017:2015</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="3d35c-139">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="3d35c-139">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="3d35c-140">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="3d35c-140">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="3d35c-141">使用下表判斷 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="3d35c-141">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="3d35c-142">**適用性**</span><span class="sxs-lookup"><span data-stu-id="3d35c-142">**Applicability**</span></span> | <span data-ttu-id="3d35c-143">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="3d35c-143">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="3d35c-144">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="3d35c-144">**Office 365**</span></span> | <span data-ttu-id="3d35c-145">Access Online、Azure Active Directory、Azure Communications Service、合規性管理員、客戶加密箱、Delve、Exchange Online、Exchange Online Protection、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Defender for Office 365、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 客戶入口網站、Office 365 微服務 (包含但不限 Kaizala、ObjectStore、Sway、PowerPoint Online Document Service、Query Annotation Service、學校資料同步處理、Siphon、Speech、StaffHub、eXtensible Application Program)、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、Office Services Infrastructure、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、Project Online、使用客戶金鑰的服務加密、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="3d35c-145">Access Online, Azure Active Directory, Azure Communications Service, Compliance Manager, Customer Lockbox, Delve, Exchange Online, Exchange Online Protection, Forms, Griffin, Identity Manager, Lockbox (Torus), Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Customer Portal, Office 365 Microservices (including but not limited to Kaizala, ObjectStore, Sway, PowerPoint Online Document Service, Query Annotation Service, School Data Sync, Siphon, Speech, StaffHub, eXtensible Application Program), Office 365 Security & Compliance Center, Office Online, Office Pro Plus, Office Services Infrastructure, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, Project Online, Service Encryption with Customer Key, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="3d35c-146">**GCC**</span><span class="sxs-lookup"><span data-stu-id="3d35c-146">**GCC**</span></span> | <span data-ttu-id="3d35c-147">Azure Active Directory、Azure Communications Service、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream</span><span class="sxs-lookup"><span data-stu-id="3d35c-147">Azure Active Directory, Azure Communications Service, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream</span></span> |
| <span data-ttu-id="3d35c-148">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="3d35c-148">**GCC High**</span></span> | <span data-ttu-id="3d35c-149">Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="3d35c-149">Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business</span></span> |
| <span data-ttu-id="3d35c-150">**DoD**</span><span class="sxs-lookup"><span data-stu-id="3d35c-150">**DoD**</span></span> | <span data-ttu-id="3d35c-151">Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、Power BI、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="3d35c-151">Azure Active Directory, Azure Communications Service, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, Power BI, SharePoint Online, Skype for Business</span></span> |

### <a name="office-365-audits-reports-and-certificates"></a><span data-ttu-id="3d35c-152">Office 365 稽核、報告和認證</span><span class="sxs-lookup"><span data-stu-id="3d35c-152">Office 365 audits, reports, and certificates</span></span>

<span data-ttu-id="3d35c-153">Microsoft 雲端服務會每年隨著 ISO/IEC 27001:2013 的認證程序，針對 ISO/IEC 27017:2015 工作條例規定進行一次稽核。</span><span class="sxs-lookup"><span data-stu-id="3d35c-153">Microsoft cloud services are audited once a year for the ISO/IEC 27017:2015 code of practice as part of the certification process for ISO/IEC 27001:2013.</span></span>

- [<span data-ttu-id="3d35c-154">Office 365：ISO 27001、27018 和 27017 稽核評估報告</span><span class="sxs-lookup"><span data-stu-id="3d35c-154">Office 365: ISO 27001, 27018, and 27017 Audit Assessment Report</span></span>](https://aka.ms/o365isoreport)

### <a name="frequently-asked-questions"></a><span data-ttu-id="3d35c-155">常見問題集</span><span class="sxs-lookup"><span data-stu-id="3d35c-155">Frequently asked questions</span></span>

<span data-ttu-id="3d35c-156">**該標準適用於誰？**</span><span class="sxs-lookup"><span data-stu-id="3d35c-156">**To whom does the standard apply?**</span></span>

<span data-ttu-id="3d35c-157">此工作條例規定可提供雲端服務提供者和雲端服務客戶的控制和實作指導方針。</span><span class="sxs-lookup"><span data-stu-id="3d35c-157">This code of practice provides controls and implementation guidance for both cloud service providers and cloud service customers.</span></span> <span data-ttu-id="3d35c-158">它的結構格式類似於 ISO/IEC 27002:2013。</span><span class="sxs-lookup"><span data-stu-id="3d35c-158">It is structured in a format similar to ISO/IEC 27002:2013.</span></span>

<span data-ttu-id="3d35c-159">**可以在何處檢視 Microsoft 的 ISO/IEC 27017:2015 合規性資訊？**</span><span class="sxs-lookup"><span data-stu-id="3d35c-159">**Where can I view Microsoft's compliance information for ISO/IEC 27017:2015?**</span></span>

<span data-ttu-id="3d35c-160">您可以下載適用於 Azure、Intune 和 Power BI 的 [ISO/IEC 27017:2015 認證](https://aka.ms/azureiso27017)。</span><span class="sxs-lookup"><span data-stu-id="3d35c-160">You can download the [ISO/IEC 27017:2015 certificate](https://aka.ms/azureiso27017) for Azure, Intune, and Power BI.</span></span>

<span data-ttu-id="3d35c-161">**我是否可以在組織的認證程序中使用 Microsoft 服務的 ISO/IEC 27017 合規性？**</span><span class="sxs-lookup"><span data-stu-id="3d35c-161">**Can I use the ISO/IEC 27017 compliance of Microsoft services in my organization's certification process?**</span></span>

<span data-ttu-id="3d35c-162">是。</span><span class="sxs-lookup"><span data-stu-id="3d35c-162">Yes.</span></span> <span data-ttu-id="3d35c-163">如果貴公司正在尋求用於在任何 Microsoft 範圍內企業雲端服務上所部署實作的認證，則可以在您的合規性評定中使用 Microsoft 的相關認證。</span><span class="sxs-lookup"><span data-stu-id="3d35c-163">If your business is seeking certification for implementations deployed on any Microsoft in-scope enterprise cloud services, you can use Microsoft's relevant certifications in your compliance assessment.</span></span> <span data-ttu-id="3d35c-164">不過，您有責任確保評定者有參與評估合規性的實作，以及組織中的控制和程序。</span><span class="sxs-lookup"><span data-stu-id="3d35c-164">However, you are responsible for engaging an assessor to evaluate your implementation for compliance, and for the controls and processes within your own organization.</span></span>

<span data-ttu-id="3d35c-165">**如何取得適用稽核報告的複本？**</span><span class="sxs-lookup"><span data-stu-id="3d35c-165">**How can I get copies of the applicable audit reports?**</span></span>

<span data-ttu-id="3d35c-166">[服務信任入口網站](https://aka.ms/stphelp)提供獨立的協力廠商稽核報告和其他相關文件。</span><span class="sxs-lookup"><span data-stu-id="3d35c-166">The [Service Trust Portal](https://aka.ms/stphelp) provides independent, third-party audit reports and other related documentation.</span></span> <span data-ttu-id="3d35c-167">您可以使用入口網站來下載並檢閱此文件，以獲得您自己的法規需求的協助。</span><span class="sxs-lookup"><span data-stu-id="3d35c-167">You can use the portal to download and review this documentation for assistance with your own regulatory requirements.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="3d35c-168">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="3d35c-168">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="3d35c-169">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="3d35c-169">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="3d35c-170">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="3d35c-170">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="3d35c-171">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="3d35c-171">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="3d35c-172">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="3d35c-172">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="3d35c-173">資源</span><span class="sxs-lookup"><span data-stu-id="3d35c-173">Resources</span></span>

- [<span data-ttu-id="3d35c-174">ISO/IEC 27017:2015 工作條例規定</span><span class="sxs-lookup"><span data-stu-id="3d35c-174">ISO/IEC 27017:2015 code of practice</span></span>](https://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43757)
- [<span data-ttu-id="3d35c-175">Microsoft Online Services 條款</span><span class="sxs-lookup"><span data-stu-id="3d35c-175">Microsoft Online Services Terms</span></span>](https://aka.ms/Online-Services-Terms)
- [<span data-ttu-id="3d35c-176">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="3d35c-176">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
