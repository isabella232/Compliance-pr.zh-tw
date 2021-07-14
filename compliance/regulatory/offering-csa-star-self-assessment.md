---
title: 合規性方案 - 雲端安全性聯盟 (CSA) STAR 自我評定
description: Microsoft STAR 自我評定詳細說明雲端服務如何符合雲端安全性聯盟需求。
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
ms.openlocfilehash: c2736c5ddb9c29a65d37f95c271bfb56e97fee88
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384213"
---
# <a name="cloud-security-alliance-csa-star-self-assessment"></a><span data-ttu-id="a664f-104">雲端安全性聯盟 (CSA) STAR 自我評定</span><span class="sxs-lookup"><span data-stu-id="a664f-104">Cloud Security Alliance (CSA) STAR self-assessment</span></span>

## <a name="csa-star-self-assessment-overview"></a><span data-ttu-id="a664f-105">CSA STAR 自我評定概觀</span><span class="sxs-lookup"><span data-stu-id="a664f-105">CSA STAR self-assessment overview</span></span>

<span data-ttu-id="a664f-106">雲端安全性聯盟 (CSA) 是一個非贏利組織，由廣泛的行業從業者、公司和其他重要專案關係人聯盟所領導。</span><span class="sxs-lookup"><span data-stu-id="a664f-106">The Cloud Security Alliance (CSA) is a nonprofit organization led by a broad coalition of industry practitioners, corporations, and other important stakeholders.</span></span> <span data-ttu-id="a664f-107">該組織致力於定義最佳做法，以協助確保更安全的雲端運算環境，並協助潛在的雲端客戶在將其 IT 營運轉換到雲端時做出明智的決策。</span><span class="sxs-lookup"><span data-stu-id="a664f-107">It is dedicated to defining best practices to help ensure a more secure cloud computing environment, and to helping potential cloud customers make informed decisions when transitioning their IT operations to the cloud.</span></span>  
  
<span data-ttu-id="a664f-108">在 2010 年，CSA 發佈了一套可評估雲端 IT 營運的工具：CSA Governance、Risk Management 及 Compliance (GRC) Stack。</span><span class="sxs-lookup"><span data-stu-id="a664f-108">In 2010, the CSA published a suite of tools to assess cloud IT operations: the CSA Governance, Risk Management, and Compliance (GRC) Stack.</span></span> <span data-ttu-id="a664f-109">這是專為協助雲端客戶評估雲端服務提供者 (CSP) 遵循業界最佳做法和標準並遵守法規的方式而設計。</span><span class="sxs-lookup"><span data-stu-id="a664f-109">It was designed to help cloud customers assess how cloud service providers (CSPs) follow industry best practices and standards and comply with regulations.</span></span>  
  
<span data-ttu-id="a664f-110">在 2013 年，CSA 和英國標準協會 (British Standards Institution) 推出了安全性、信任與保證註冊 (STAR)，這是一個免費且可公開存取的註冊服務，CSA 可以在其中發佈與 CSA 相關的評定。</span><span class="sxs-lookup"><span data-stu-id="a664f-110">In 2013, the CSA and the British Standards Institution launched the Security, Trust & Assurance Registry (STAR), a free, publicly accessible registry in which CSPs can publish their CSA-related assessments.</span></span>  
  
<span data-ttu-id="a664f-111">CSA STAR 是以 CSA GRC Stack 的兩個重要元件為基礎：</span><span class="sxs-lookup"><span data-stu-id="a664f-111">CSA STAR is based on two key components of the CSA GRC Stack:</span></span>

- <span data-ttu-id="a664f-112">雲端控制矩陣 (CCM)：這是一個控制措施架構，涵蓋 16 個網域之間的基本安全性原則，以協助雲端客戶評估 CSP 的整體安全性風險。</span><span class="sxs-lookup"><span data-stu-id="a664f-112">Cloud Controls Matrix (CCM): a controls framework covering fundamental security principles across 16 domains to help cloud customers assess the overall security risk of a CSP.</span></span>
- <span data-ttu-id="a664f-113">自我評定問卷 (Consensus Assessments Initiative Questionnaire，CAIQ)：以 CCM 為主的 140 多個問題，客戶或雲端稽核人員可能會想要詢問 CSP，以評估其對 CSA 最佳做法的合規性。</span><span class="sxs-lookup"><span data-stu-id="a664f-113">The Consensus Assessments Initiative Questionnaire (CAIQ): a set of more than 140 questions based on the CCM that a customer or cloud auditor may want to ask of CSPs to assess their compliance with CSA best practices.</span></span>

<span data-ttu-id="a664f-114">STAR 提供三個保證層級；CSA-STAR 自我評定是層級 1 的介紹性方案，免費開放給所有 CSP 使用。</span><span class="sxs-lookup"><span data-stu-id="a664f-114">STAR provides three levels of assurance; CSA-STAR Self-Assessment is the introductory offering at Level 1, which is free and open to all CSPs.</span></span> <span data-ttu-id="a664f-115">STAR 方案的層級 2 進一步提升保證堆疊，其中涉及協力廠商評定的認證，而層級 3 則涉及以持續監視為主的認證。</span><span class="sxs-lookup"><span data-stu-id="a664f-115">Going further up the assurance stack, Level 2 of the STAR program involves third-party assessment-based certifications, and Level 3 involves certifications based on continuous monitoring.</span></span>

## <a name="microsoft-and-csa-star-self-assessment"></a><span data-ttu-id="a664f-116">Microsoft 和 CSA STAR 自我評定</span><span class="sxs-lookup"><span data-stu-id="a664f-116">Microsoft and CSA STAR self-assessment</span></span>

<span data-ttu-id="a664f-117">在 STAR 自我評定中，CSP 可以提交下列兩種不同類型的文件，以表示對 CSA 最佳做法的合規性：已完成的 CAIQ，或是記載對 CCM 之合規性的報告。</span><span class="sxs-lookup"><span data-stu-id="a664f-117">As part of the STAR Self-Assessment, CSPs can submit two different types of documents to indicate their compliance with CSA best practices: a completed CAIQ, or a report documenting compliance with CCM.</span></span> <span data-ttu-id="a664f-118">對於 CSA STAR 自我評定，Microsoft 會為 Microsoft Azure 發佈將 CAIQ 和 CCM 的報告，並為 Microsoft Dynamics 365 和 Microsoft Office 365 發佈 CCM 的報告。</span><span class="sxs-lookup"><span data-stu-id="a664f-118">For the CSA STAR Self-Assessment, Microsoft publishes both a CAIQ and a CCM-based report for Microsoft Azure, and CCM-based reports for Microsoft Dynamics 365 and Microsoft Office 365.</span></span>  

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="a664f-119">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="a664f-119">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="a664f-120">Azure 和 Azure Government</span><span class="sxs-lookup"><span data-stu-id="a664f-120">Azure and Azure Government</span></span>
- [<span data-ttu-id="a664f-121">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a664f-121">Dynamics 365</span></span>](https://aka.ms/d365-compliance-list)
- <span data-ttu-id="a664f-122">Office 365</span><span class="sxs-lookup"><span data-stu-id="a664f-122">Office 365</span></span>

## <a name="azure-dynamics-365-and-csa-star-self-assessment"></a><span data-ttu-id="a664f-123">Azure、Dynamics 365 和 CSA STAR 自我評定</span><span class="sxs-lookup"><span data-stu-id="a664f-123">Azure, Dynamics 365, and CSA STAR self-assessment</span></span>

<span data-ttu-id="a664f-124">如需 Azure、Dynamics 365 及其他線上服務合規性詳細資訊，請參閱 [Azure CSA STAR 自我評定供應項目](/azure/compliance/offerings/offering-csa-star-self-assessment)。</span><span class="sxs-lookup"><span data-stu-id="a664f-124">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure CSA STAR self-assessment offering](/azure/compliance/offerings/offering-csa-star-self-assessment).</span></span>

## <a name="office-365-and-csa-star-self-assessment"></a><span data-ttu-id="a664f-125">Office 365 和 CSA STAR 自我評定</span><span class="sxs-lookup"><span data-stu-id="a664f-125">Office 365 and CSA STAR self-assessment</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="a664f-126">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="a664f-126">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="a664f-127">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="a664f-127">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="a664f-128">使用下表判斷 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="a664f-128">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="a664f-129">**適用性**</span><span class="sxs-lookup"><span data-stu-id="a664f-129">**Applicability**</span></span> | <span data-ttu-id="a664f-130">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="a664f-130">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="a664f-131">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="a664f-131">**Office 365**</span></span> |<span data-ttu-id="a664f-132">Exchange Online、Exchange Online Protection、Office 365 客戶入口網站、Office Online、Office 服務基礎結構、商務用 OneDrive、SharePoint Online、商務用 Skype</span><span class="sxs-lookup"><span data-stu-id="a664f-132">Exchange Online, Exchange Online Protection, Office 365 Customer Portal, Office Online, Office Services Infrastructure, OneDrive for Business,SharePoint Online, Skype for Business</span></span> |

### <a name="frequently-asked-questions"></a><span data-ttu-id="a664f-133">常見問題集</span><span class="sxs-lookup"><span data-stu-id="a664f-133">Frequently asked questions</span></span>

<span data-ttu-id="a664f-134">**CSA CCM 符合哪些產業標準？**</span><span class="sxs-lookup"><span data-stu-id="a664f-134">**Which industry standards does the CSA CCM align with?**</span></span>

<span data-ttu-id="a664f-135">CCM 符合產業公認的安全性標準、規定及控制措施架構，例如：ISO 27001、PCI DSS、HIPAA、AICPA SOC 2、NERC CIP、FedRAMP、NIST 等等。</span><span class="sxs-lookup"><span data-stu-id="a664f-135">The CCM corresponds to industry-accepted security standards, regulations, and control frameworks such as ISO 27001, PCI DSS, HIPAA, AICPA SOC 2, NERC CIP, FedRAMP, NIST, and many more.</span></span> <span data-ttu-id="a664f-136">如需最新清單，請瀏覽 [CSA 網站](https://cloudsecurityalliance.org/)。</span><span class="sxs-lookup"><span data-stu-id="a664f-136">For the most current list, visit the [CSA website](https://cloudsecurityalliance.org/).</span></span>

<span data-ttu-id="a664f-137">**為什麼 CSA STAR 自我評定很重要？**</span><span class="sxs-lookup"><span data-stu-id="a664f-137">**Why is the CSA STAR Self-Assessment important?**</span></span>

<span data-ttu-id="a664f-138">它可讓 CSP 以透明的方式記載對 CSA 發佈的最佳做法的合規性。</span><span class="sxs-lookup"><span data-stu-id="a664f-138">It enables CSPs to document compliance with CSA published best practices in a transparent manner.</span></span> <span data-ttu-id="a664f-139">自我評定報告可公開取得，因此可協助雲端客戶深入了解 CSP 的安全性做法，並使用相同的基準來比較不同的 CSP。</span><span class="sxs-lookup"><span data-stu-id="a664f-139">Self-assessment reports are publicly available, thereby helping cloud customers gain visibility into the security practices of CSPs, and compare various CSPs using the same baseline.</span></span>

<span data-ttu-id="a664f-140">**Office 365 獲得哪些 CSA STAR 保證層級？**</span><span class="sxs-lookup"><span data-stu-id="a664f-140">**Which CSA STAR levels of assurance has Office 365 attained?**</span></span>

- <span data-ttu-id="a664f-141">**層級 1**：**CSA STAR 自我評定**：是雲端服務提供者所提供的免費供應項目，用於記載其安全性控制措施以協助客戶評估服務安全性。</span><span class="sxs-lookup"><span data-stu-id="a664f-141">**Level 1**: **CSA STAR Self-Assessment**: a complimentary offering from cloud service providers to document their security controls to help customers assess the security of the service.</span></span>

### <a name="office-365-resources"></a><span data-ttu-id="a664f-142">Office 365 資源</span><span class="sxs-lookup"><span data-stu-id="a664f-142">Office 365 Resources</span></span>

- [<span data-ttu-id="a664f-143">雲端安全性聯盟</span><span class="sxs-lookup"><span data-stu-id="a664f-143">Cloud Security Alliance</span></span>](https://cloudsecurityalliance.org/)
- [<span data-ttu-id="a664f-144">雲端控制矩陣 (CCM)</span><span class="sxs-lookup"><span data-stu-id="a664f-144">Cloud Controls Matrix (CCM)</span></span>](https://cloudsecurityalliance.org/group/cloud-controls-matrix/)
- [<span data-ttu-id="a664f-145">自我評定問卷 (CAIQ)</span><span class="sxs-lookup"><span data-stu-id="a664f-145">Consensus Assessments Initiative Questionnaire (CAIQ)</span></span>](https://cloudsecurityalliance.org/group/consensus-assessments/)
- [<span data-ttu-id="a664f-146">CSA 安全性、信任與保證註冊 (STAR)</span><span class="sxs-lookup"><span data-stu-id="a664f-146">CSA Security, Trust & Assurance Registry (STAR)</span></span>](https://cloudsecurityalliance.org/star/)
- [<span data-ttu-id="a664f-147">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="a664f-147">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)