---
title: '狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) '
description: Azure 和 Office 365 會驗證健康資訊信任同盟 (HITRUST) 常見的安全性框架 (CSF) 。
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
ms.openlocfilehash: ef8f44309a8560341f456b3b2cace3b8038ae993
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384853"
---
# <a name="health-information-trust-alliance-hitrust-common-security-framework-csf"></a><span data-ttu-id="0d7c2-104">狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) </span><span class="sxs-lookup"><span data-stu-id="0d7c2-104">Health Information Trust Alliance (HITRUST) Common Security Framework (CSF)</span></span>

## <a name="hitrust-csf-overview"></a><span data-ttu-id="0d7c2-105">HITRUST CSF 一覽</span><span class="sxs-lookup"><span data-stu-id="0d7c2-105">HITRUST CSF overview</span></span>

<span data-ttu-id="0d7c2-106">狀況資訊信任同盟 (HITRUST) 是由醫療保健行業的代表所管理的組織。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-106">The Health Information Trust Alliance (HITRUST) is an organization governed by representatives from the healthcare industry.</span></span> <span data-ttu-id="0d7c2-107">HITRUST 建立並維護常見的安全性框架 (CSF) ，一種 certifiable 架構，可協助醫療保健組織及其提供者示範其安全性和符合性，以一致且簡潔的方式。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-107">HITRUST created and maintains the Common Security Framework (CSF), a certifiable framework to help healthcare organizations and their providers demonstrate their security and compliance in a consistent and streamlined manner.</span></span>

<span data-ttu-id="0d7c2-108">CSF 建立于 HIPAA 和高科技法案，這是美國醫療保健法，已針對個別身分識別健康資訊的使用、披露和保護，以及強制執行不相容的要求。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-108">The CSF builds on HIPAA and the HITECH Act, which are US healthcare laws that have established requirements for the use, disclosure, and safeguarding of individually identifiable health information, and that enforce noncompliance.</span></span> <span data-ttu-id="0d7c2-109">HITRUST 提供一個基準-標準化的規範架構、評估和認證程式，讓雲端服務提供者和涵蓋的健康情況實體可以測量規范。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-109">HITRUST provides a benchmark — a standardized compliance framework, assessment, and certification process — against which cloud service providers and covered health entities can measure compliance.</span></span> <span data-ttu-id="0d7c2-110">CSF 也會將這類現有架構的醫療保健特定安全性、隱私權及其他法規需求納入到支付卡行業資料安全性標準 ([PCI-DSS](https://www.microsoft.com/trustcenter/compliance/pci)) 、 [ISO/IEC 27001](https://www.microsoft.com/trustcenter/compliance/iso-iec-27001) 資訊安全性管理標準，以及 ([火星-E](https://www.microsoft.com/trustcenter/compliance/mars-e)) 的最小可接受風險標準。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-110">The CSF also incorporates healthcare-specific security, privacy, and other regulatory requirements from such existing frameworks as the Payment Card Industry Data Security Standard ([PCI-DSS](https://www.microsoft.com/trustcenter/compliance/pci)), [ISO/IEC 27001](https://www.microsoft.com/trustcenter/compliance/iso-iec-27001) information security management standards, and Minimum Acceptable Risk Standards for Exchanges ([MARS-E](https://www.microsoft.com/trustcenter/compliance/mars-e)).</span></span>

<span data-ttu-id="0d7c2-111">CSF 分為19個不同的網域，包括 endpoint protection、行動裝置安全性和存取控制。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-111">The CSF is divided into 19 different domains, including endpoint protection, mobile device security, and access control.</span></span> <span data-ttu-id="0d7c2-112">HITRUST 會針對這些控制項來驗證 IT 產品。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-112">HITRUST certifies IT offerings against these controls.</span></span> <span data-ttu-id="0d7c2-113">HITRUST 也會根據組織、系統和法規因素，改編組織風險的認證需求。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-113">HITRUST also adapts requirements for certification to the risks of an organization based on organizational, system, and regulatory factors.</span></span>

<span data-ttu-id="0d7c2-114">狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) </span><span class="sxs-lookup"><span data-stu-id="0d7c2-114">Health Information Trust Alliance (HITRUST) Common Security Framework (CSF)</span></span>

<span data-ttu-id="0d7c2-115">HITRUST 提供三種確定性或評估等級：自我評估、CSF 驗證及 CSF 認證。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-115">HITRUST offers three degrees of assurance, or levels of assessment: self-assessment, CSF validated, and CSF-certified.</span></span> <span data-ttu-id="0d7c2-116">每個層級組建都會在其下一個層級上增加嚴謹。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-116">Each level builds with increasing rigor on the one below it.</span></span> <span data-ttu-id="0d7c2-117">最高層次的組織，CSF 認證，符合 CSF 的所有認證需求。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-117">An organization with the highest level, CSF-certified, meets all the certification requirements of the CSF.</span></span> <span data-ttu-id="0d7c2-118">Microsoft Azure 和 Office 365 是第一個超大型雲端服務，可接收 HITRUST CSF 的認證。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-118">Microsoft Azure and Office 365 are the first hyperscale cloud services to receive certification for the HITRUST CSF.</span></span> <span data-ttu-id="0d7c2-119">Coalfire，HITRUST assessor 公司，根據 Azure 和 Office 365 如何執行安全性、隱私權和法規需求，以保護機密資訊，來執行評估。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-119">Coalfire, a HITRUST assessor firm, performed the assessments based on how Azure and Office 365 implement security, privacy, and regulatory requirements to protect sensitive information.</span></span> <span data-ttu-id="0d7c2-120">Microsoft 支援 HITRUST 共用責任計畫。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-120">Microsoft supports the HITRUST Shared Responsibility Program.</span></span>

<span data-ttu-id="0d7c2-121">瞭解如何使用 Azure 安全性和合規性藍圖加速您的 HITRUST 部署。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-121">Learn how to accelerate your HITRUST deployment with our Azure Security and Compliance Blueprint.</span></span>

[<span data-ttu-id="0d7c2-122"> (CRM) 藍圖 HITRUST，下載 Microsoft Azure 的客戶責任矩陣</span><span class="sxs-lookup"><span data-stu-id="0d7c2-122">Download the Microsoft Azure HITRUST Customer Responsibility Matrix (CRM) blueprint v9.0d</span></span>](https://servicetrust.microsoft.com/ViewPage/Blueprint?command=Download&downloadType=Document&downloadId=3ccde498-4761-4be0-be8b-cd8d379a3a4f&docTab=fc060920-cdb8-11e7-bacf-0bf52b09d912_Healthcare_Blueprint)

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="0d7c2-123">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="0d7c2-123">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="0d7c2-124">Azure 和 Azure Government</span><span class="sxs-lookup"><span data-stu-id="0d7c2-124">Azure and Azure Government</span></span>
- <span data-ttu-id="0d7c2-125">Intune</span><span class="sxs-lookup"><span data-stu-id="0d7c2-125">Intune</span></span>
- [<span data-ttu-id="0d7c2-126">Microsoft 受管理的電腦</span><span class="sxs-lookup"><span data-stu-id="0d7c2-126">Microsoft Managed Desktop</span></span>](/microsoft-365/managed-desktop/intro/compliance)
- <span data-ttu-id="0d7c2-127">Office 365</span><span class="sxs-lookup"><span data-stu-id="0d7c2-127">Office 365</span></span>

## <a name="azure-dynamics-365-and-hitrust"></a><span data-ttu-id="0d7c2-128">Azure、Dynamics 365 和 HITRUST</span><span class="sxs-lookup"><span data-stu-id="0d7c2-128">Azure, Dynamics 365, and HITRUST</span></span>

<span data-ttu-id="0d7c2-129">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE HITRUST 服務](/azure/compliance/offerings/offering-hitrust)。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-129">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure HITRUST offering](/azure/compliance/offerings/offering-hitrust).</span></span>

## <a name="office-365-and-hitrust"></a><span data-ttu-id="0d7c2-130">Office 365 和 HITRUST</span><span class="sxs-lookup"><span data-stu-id="0d7c2-130">Office 365 and HITRUST</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="0d7c2-131">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="0d7c2-131">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="0d7c2-132">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="0d7c2-132">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="0d7c2-133">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="0d7c2-133">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="0d7c2-134">**適用性**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-134">**Applicability**</span></span> | <span data-ttu-id="0d7c2-135">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-135">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="0d7c2-136">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-136">**Office 365**</span></span> | <span data-ttu-id="0d7c2-137">活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="0d7c2-137">Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="office-365-audits-reports-and-certificates"></a><span data-ttu-id="0d7c2-138">Office 365 審核、報告和憑證</span><span class="sxs-lookup"><span data-stu-id="0d7c2-138">Office 365 audits, reports, and certificates</span></span>

<span data-ttu-id="0d7c2-139">Office 365 的 HITRUST CSF 證書是兩年有效。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-139">The HITRUST CSF certification of Office 365 is valid for two years.</span></span>

- [<span data-ttu-id="0d7c2-140">Office 365憑證的 HITRUST 字母</span><span class="sxs-lookup"><span data-stu-id="0d7c2-140">Office 365 HITRUST Letter of Certification</span></span>](https://aka.ms/O365HITRUSTcertification)

### <a name="frequently-asked-questions"></a><span data-ttu-id="0d7c2-141">常見問題集</span><span class="sxs-lookup"><span data-stu-id="0d7c2-141">Frequently asked questions</span></span>

<span data-ttu-id="0d7c2-142">**為什麼有些 Office 365 服務不在此認證的範圍內？**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-142">**Why are some Office 365 services not in the scope of this certification?**</span></span>

<span data-ttu-id="0d7c2-143">Microsoft 提供最全面的選項，與其他雲端服務提供者相較。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-143">Microsoft provides the most comprehensive offerings compared to other cloud service providers.</span></span> <span data-ttu-id="0d7c2-144">為了維持跨地區和行業的廣泛合規性服務，我們根據市場需求、客戶意見反應及產品生命週期，在我們的保證工作範圍內加入服務。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-144">To keep up with our broad compliance offerings across regions and industries, we include services in the scope of our assurance efforts based on the market demand, customer feedback, and product lifecycle.</span></span> <span data-ttu-id="0d7c2-145">如果服務並未包含在特定規范產品的目前範圍內，則您的組織有責任根據您的合規性義務評估風險，並決定處理該服務中資料的方式。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-145">If a service is not included in the current scope of a specific compliance offering, your organization has the responsibility to assess the risks based on your compliance obligations and determine the way you process the data in that service.</span></span> <span data-ttu-id="0d7c2-146">我們會持續收集客戶的意見反應，與管理機構和審計員合作，以擴大我們的安全性和合規性需求。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-146">We continuously collect feedback from customers and work with regulators and auditors to expand our compliance coverage to meet your security and compliance needs.</span></span>

<span data-ttu-id="0d7c2-147">**Microsoft 憑證表示如果我的組織使用 Office 365，它符合 HITRUST CSF？**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-147">**Does Microsoft certification mean that if my organization uses Office 365, it is compliant with HITRUST CSF?**</span></span>

<span data-ttu-id="0d7c2-148">當您將資料儲存在 Office 365 的 SaaS 中時，Microsoft 與您組織之間的共同責任，以達成法規。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-148">When you store your data in a SaaS like Office 365, it's a shared responsibility between Microsoft and your organization to achieve compliance.</span></span> <span data-ttu-id="0d7c2-149">Microsoft 會管理大部分的基礎結構控制，包括實體安全性、網路控制、應用層級控制等，而且您的組織有責任管理存取控制和保護您的敏感性資料。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-149">Microsoft manages majority of the infrastructure controls including physical security, network controls, application level controls, etc., and your organization has the responsibility to manage access controls and protect your sensitive data.</span></span> <span data-ttu-id="0d7c2-150">Office 365 HITRUST 認證示範 Microsoft 的控制架構合規性。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-150">The Office 365 HITRUST certification demonstrates the compliance of Microsoft's control framework.</span></span> <span data-ttu-id="0d7c2-151">為此，您的組織必須實施及維護您自己的資料保護控制，以符合 HITRUST CSF 需求。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-151">Building on that, your organization needs to implement and maintain your own data protection controls to meet HITRUST CSF requirements.</span></span>

<span data-ttu-id="0d7c2-152">**當使用 Office 365 時，Microsoft 是否會為我的組織提供指導，以執行適當的控制項？**</span><span class="sxs-lookup"><span data-stu-id="0d7c2-152">**Does Microsoft provide guidance for my organization to implement appropriate controls when using Office 365?**</span></span>

<span data-ttu-id="0d7c2-153">是的，您可以在合規性分數中尋找建議的客戶動作，以協助您的組織在使用雲端服務時符合複雜的合規性義務。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-153">Yes, you can find recommended customer actions in Compliance Score, cross-Microsoft Cloud solutions that help your organization meet complex compliance obligations when using cloud services.</span></span> <span data-ttu-id="0d7c2-154">具體說來，針對 HITRUST CSF，我們建議您使用 NIST 800-53 和 NIST CSF 評估遵循合規性分數來執行風險評估。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-154">Specifically, for HITRUST CSF, we recommend that you perform risk assessments using the NIST 800-53 and NIST CSF assessments in Compliance Score.</span></span> <span data-ttu-id="0d7c2-155">在評估中，我們為您提供逐步指導方針，以及您可以用來實施資料保護控制的 Microsoft 解決方案。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-155">In the assessments, we provide you with step-by-step guidance and the Microsoft solutions you can use to implement your data protection controls.</span></span> <span data-ttu-id="0d7c2-156">您可以深入瞭解 [Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)中的合規性分數。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-156">You can learn more about Compliance Score in [Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager).</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="0d7c2-157">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="0d7c2-157">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="0d7c2-158">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-158">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="0d7c2-159">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-159">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="0d7c2-160">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-160">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="0d7c2-161">瞭解如何 [在合規性管理員中建立及管理評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="0d7c2-161">Learn how to [Build and manage assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="0d7c2-162">資源</span><span class="sxs-lookup"><span data-stu-id="0d7c2-162">Resources</span></span>

- [<span data-ttu-id="0d7c2-163">HITRUST 同盟</span><span class="sxs-lookup"><span data-stu-id="0d7c2-163">HITRUST Alliance</span></span>](https://hitrustalliance.net/)
- [<span data-ttu-id="0d7c2-164">HITRUST CSF 9。3</span><span class="sxs-lookup"><span data-stu-id="0d7c2-164">HITRUST CSF 9.3</span></span>](https://hitrustalliance.net/csf-license-agreement/)
- [<span data-ttu-id="0d7c2-165">瞭解和利用 CSF</span><span class="sxs-lookup"><span data-stu-id="0d7c2-165">Understanding and Leveraging the CSF</span></span>](https://hitrustalliance.net/understanding-leveraging-csf/)
- [<span data-ttu-id="0d7c2-166">進一步瞭解 HITRUST 共用責任計畫</span><span class="sxs-lookup"><span data-stu-id="0d7c2-166">Find out more about the HITRUST Shared Responsibility Program</span></span>](https://go.microsoft.com/fwlink/p/?linkid=2100268)
- [<span data-ttu-id="0d7c2-167">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="0d7c2-167">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
