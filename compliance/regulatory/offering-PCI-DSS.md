---
title: 支付卡行業 (PCI) 資料安全標準 (DSS)
description: Azure、SharePoint Online 和商務用 OneDrive 符合支付卡行業資料安全標準第 1 級 3.2 版。
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
ms.openlocfilehash: ab92c2d12477e0e7fa1890ae25e06d264305e95c
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384383"
---
# <a name="payment-card-industry-pci-data-security-standard-dss"></a><span data-ttu-id="2e8bb-104">支付卡行業 (PCI) 資料安全標準 (DSS)</span><span class="sxs-lookup"><span data-stu-id="2e8bb-104">Payment Card Industry (PCI) Data Security Standard (DSS)</span></span>

## <a name="pci-dss-overview"></a><span data-ttu-id="2e8bb-105">PCI DSS 概觀</span><span class="sxs-lookup"><span data-stu-id="2e8bb-105">PCI DSS overview</span></span>

<span data-ttu-id="2e8bb-106">支付卡行業 (PCI) 資料安全標準 (DSS) 是一個全球資訊安全性標準，旨在透過進一步控制信用卡資料來防止詐欺行為。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-106">The Payment Card Industry (PCI) Data Security Standards (DSS) is a global information security standard designed to prevent fraud through increased control of credit card data.</span></span> <span data-ttu-id="2e8bb-107">任何規模的組織在接受來自五大信用卡品牌 (Visa、MasterCard、American Express、Discover 及 Japan Credit Bureau (JCB)) 的付款卡時，都必須遵循 PCI DSS 標準。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-107">Organizations of all sizes must follow PCI DSS standards if they accept payment cards from the five major credit card brands, Visa, MasterCard, American Express, Discover, and the Japan Credit Bureau (JCB).</span></span> <span data-ttu-id="2e8bb-108">任何儲存、處理或傳輸付款和持卡人資料的組織皆需符合 PCI DSS 規範。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-108">Compliance with PCI DSS is required for any organization that stores, processes, or transmits payment and cardholder data.</span></span>

## <a name="microsoft-and-pci-dss"></a><span data-ttu-id="2e8bb-109">Microsoft 和 PCI DSS</span><span class="sxs-lookup"><span data-stu-id="2e8bb-109">Microsoft and PCI DSS</span></span>

<span data-ttu-id="2e8bb-110">Microsoft 已透過經核准的合格資安評估商 (QSA) 完成年度 PCI DSS 評估。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-110">Microsoft completed an annual PCI DSS assessment using an approved Qualified Security Assessor (QSA).</span></span> <span data-ttu-id="2e8bb-111">審查員已審查 Microsoft Azure、Microsoft 商務用 OneDrive 和 Microsoft SharePoint Online 環境，其中包括驗證基礎結構、開發、作業、管理、支援和範圍內服務。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-111">The auditors reviewed Microsoft Azure, Microsoft OneDrive for Business, and Microsoft SharePoint Online  environments, which include validating the infrastructure, development, operations, management, support, and in-scope services.</span></span> <span data-ttu-id="2e8bb-112">PCI DSS 根據交易量指定 4 個合規性等級。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-112">The PCI DSS designates four levels of compliance based on transaction volume.</span></span> <span data-ttu-id="2e8bb-113">Azure、商務用 OneDrive 和 SharePoint Online 通過服務提供者第 1 級 PCI DSS 3.2 版認證 (最高交易量，一年超過 600 萬)。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-113">Azure, OneDrive for Business, and SharePoint Online are certified as compliant under PCI DSS version 3.2 at Service Provider Level 1 (the highest volume of transactions, more than 6 million a year).</span></span>

<span data-ttu-id="2e8bb-114">評估會提供合規性證明 (AoC) 供客戶使用，以及 QSA 發出的合規性報告 (RoC)。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-114">The assessment results in an Attestation of Compliance (AoC), which is available to customers and Report on Compliance (RoC) issued by the QSA.</span></span> <span data-ttu-id="2e8bb-115">合規性的有效期從通過審核及收到評估商提供的 AoC 開始，並在 AoC 簽署日一年後結束。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-115">The effective period for compliance begins upon passing the audit and receiving the AoC from the assessor and ends one year from the date the AoC is signed.</span></span> 

<span data-ttu-id="2e8bb-116">想要開發持卡人環境或支付卡處理服務的客戶可在許多基礎部分使用這些驗證，從而降低自行取得 PCI DSS 認證的相關工作量和成本。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-116">Customers who want to develop a cardholder environment or card processing service can use these validations in many of the underlying portions, thereby reducing the associated effort and costs of getting their own PCI DSS certification.</span></span>

<span data-ttu-id="2e8bb-117">請注意，Azure、商務用 OneDrive 和 SharePoint Online 的 PCI DSS 合規性狀態不會自動轉換成客戶在這些平台上建立或託管的服務的 PCI DSS 認證。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-117">It is important to understand that PCI DSS compliance status for Azure, OneDrive for Business, and SharePoint Online not automatically translate to PCI DSS certification for the services that customers build or host on these platforms.</span></span> <span data-ttu-id="2e8bb-118">客戶需負責確保符合 PCI DSS 要求。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-118">Customers are responsible for ensuring that they achieve compliance with PCI DSS requirements.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="2e8bb-119">Microsoft 範圍內雲端平台與服務</span><span class="sxs-lookup"><span data-stu-id="2e8bb-119">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="2e8bb-120">Azure 和 Azure Government</span><span class="sxs-lookup"><span data-stu-id="2e8bb-120">Azure and Azure Government</span></span>
- <span data-ttu-id="2e8bb-121">Intune</span><span class="sxs-lookup"><span data-stu-id="2e8bb-121">Intune</span></span>
- <span data-ttu-id="2e8bb-122">Microsoft 雲端應用程式安全性</span><span class="sxs-lookup"><span data-stu-id="2e8bb-122">Microsoft Cloud App Security</span></span>
- [<span data-ttu-id="2e8bb-123">適用於端點的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="2e8bb-123">Microsoft Defender for Endpoint</span></span>](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)
- <span data-ttu-id="2e8bb-124">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e8bb-124">Microsoft Graph</span></span>
- <span data-ttu-id="2e8bb-125">Office 365</span><span class="sxs-lookup"><span data-stu-id="2e8bb-125">Office 365</span></span>
- <span data-ttu-id="2e8bb-126">商務用 OneDrive 和 SharePoint Online (僅限美國)</span><span class="sxs-lookup"><span data-stu-id="2e8bb-126">OneDrive for Business and SharePoint Online (United States only)</span></span>
- <span data-ttu-id="2e8bb-127">PPowerApps 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="2e8bb-127">PowerApps cloud service either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite</span></span>
- <span data-ttu-id="2e8bb-128">電源自動化 (可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中)</span><span class="sxs-lookup"><span data-stu-id="2e8bb-128">Power Automate (either as a standalone service or as included in an Office 365 or Dynamics 365 branded plan or suite)</span></span>
- <span data-ttu-id="2e8bb-129">Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="2e8bb-129">Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite</span></span>

## <a name="azure-dynamics-365-and-pci-dss"></a><span data-ttu-id="2e8bb-130">Azure、Dynamics 365 和 PCI DSS</span><span class="sxs-lookup"><span data-stu-id="2e8bb-130">Azure, Dynamics 365, and PCI DSS</span></span>

<span data-ttu-id="2e8bb-131">如需 Azure、Dynamics 365 及其他線上服務合規性的詳細資訊，請參閱 [Azure PCI DSS 供應項目](/azure/compliance/offerings/offering-pci-dss)。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-131">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure PCI DSS offering](/azure/compliance/offerings/offering-pci-dss).</span></span>

## <a name="office-365-and-pci-dss"></a><span data-ttu-id="2e8bb-132">Office 365 和 PCI DSS</span><span class="sxs-lookup"><span data-stu-id="2e8bb-132">Office 365 and PCI DSS</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="2e8bb-133">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="2e8bb-133">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="2e8bb-134">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="2e8bb-134">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="2e8bb-135">使用下表判斷 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="2e8bb-135">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="2e8bb-136">**適用性**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-136">**Applicability**</span></span> | <span data-ttu-id="2e8bb-137">**範圍內服務**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-137">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="2e8bb-138">**Office 365**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-138">**Office 365**</span></span> | <span data-ttu-id="2e8bb-139">商務用 OneDrive (美國)、SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2e8bb-139">OneDrive for Business (United States), SharePoint Online</span></span> |

### <a name="office-365-audit-reports-and-certificates"></a><span data-ttu-id="2e8bb-140">Office 365 稽核、報告和認證</span><span class="sxs-lookup"><span data-stu-id="2e8bb-140">Office 365 audit, reports, and certificates</span></span>

- [<span data-ttu-id="2e8bb-141">商務用 OneDrive 和 SharePoint Online PCI DSS 合規性證明 (AoC)</span><span class="sxs-lookup"><span data-stu-id="2e8bb-141">OneDrive for Business and SharePoint Online PCI DSS Attestation of Compliance (AoC)</span></span>](https://aka.ms/spo-pci)

### <a name="frequently-asked-questions"></a><span data-ttu-id="2e8bb-142">常見問題集</span><span class="sxs-lookup"><span data-stu-id="2e8bb-142">Frequently asked questions</span></span>

<span data-ttu-id="2e8bb-143">**為什麼合規性證明 (AoC) 封面頁顯示「2018 年 6 月」？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-143">**Why does the Attestation of Compliance (AoC) cover page say 'June 2018'?**</span></span>

<span data-ttu-id="2e8bb-144">封面頁上的 2018 年 6 月日期是發佈 AoC 範本的時間。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-144">The June 2018 date on the cover page is when the AoC template was published.</span></span> <span data-ttu-id="2e8bb-145">如需評估的日期，請參閱第 2 節。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-145">Refer to Section 2 for the date of the assessment.</span></span> 

<span data-ttu-id="2e8bb-146">**PA DSS 和 PCI DSS 之間的關聯是什麼？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-146">**What is the relationship between the PA DSS and PCI DSS?**</span></span>

<span data-ttu-id="2e8bb-147">支付應用程式資料安全標準 (PA DSS) 是符合 PCI DSS 的一組要求，且取代 Visa 的支付應用程式最佳實務，並合併其他主要發卡機構的合規性要求。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-147">The Payment Application Data Security Standard (PA DSS) is a set of requirements that comply with the PCI DSS, and replaces Visa's Payment Application Best Practices, and consolidates the compliance requirements of the other primary card issuers.</span></span> <span data-ttu-id="2e8bb-148">PA DSS 可協助軟體廠商開發協力廠商應用程式，在卡片授權或結算程序中儲存、處理或傳輸持卡人付款資料。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-148">The PA DSS helps software vendors develop third-party applications that store, process, or transmit cardholder payment data as part of a card authorization or settlement process.</span></span> <span data-ttu-id="2e8bb-149">零售商必須使用 PA DSS 認證應用程式以有效地達到其 PCI DSS 合規性。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-149">Retailers must use PA DSS certified applications to efficiently achieve their PCI DSS compliance.</span></span> <span data-ttu-id="2e8bb-150">PA DSS 不適用於 Azure。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-150">The PA DSS does not apply to Azure.</span></span>

<span data-ttu-id="2e8bb-151">**什麼是收單行？Azure 使用收單行嗎？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-151">**What is an acquirer and does Azure use one?**</span></span>

<span data-ttu-id="2e8bb-152">收單行是處理支付卡交易的銀行或其他實體。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-152">An acquirer is a bank or other entity that processes payment card transactions.</span></span> <span data-ttu-id="2e8bb-153">Azure 不會以服務提供支付卡處理，因此不會使用收單行。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-153">Azure does not offer payment card processing as a service and thus does not use an acquirer.</span></span>

<span data-ttu-id="2e8bb-154">**PCI DSS 適用於哪些組織和商家？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-154">**To what organizations and merchants does the PCI DSS apply?**</span></span>

<span data-ttu-id="2e8bb-155">PCI DSS 適用於任何接受、傳輸或儲存持卡人資料的公司，無論規模或交易次數。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-155">PCI DSS applies to any company, no matter the size, or number of transactions, that accepts, transmits, or stores cardholder data.</span></span> <span data-ttu-id="2e8bb-156">也就是說，如果任何客戶使用信用卡或轉帳卡付款給某公司，便適用 PCI DSS 要求。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-156">That is, if any customer ever pays a company using a credit or debit card, then the PCI DSS requirements apply.</span></span> <span data-ttu-id="2e8bb-157">系統會根據 12 個月內的總交易量，以四個層級中的其中一個層級驗證公司。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-157">Companies are validated at one of four levels based on the total transaction volume over a 12-month period.</span></span> <span data-ttu-id="2e8bb-158">第 1 級適用於每年處理超過 600 萬筆交易的公司；第 2 級適用於 100 萬至 600 萬筆交易；第 3 級適用於 20,000 至 1 百萬筆交易；而第 4 級則適用於少於 20,000 筆交易。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-158">Level 1 is for companies that process over 6 million transactions a year; Level 2 for 1 million to 6 million transactions; Level 3 is for 20,000 to 1 million transactions; and Level 4 is for fewer than 20,000 transactions.</span></span>

<span data-ttu-id="2e8bb-159">**美國以外的國家/地區是否有符合 PCI DSS 規範的商務用 OneDrive 和 SharePoint Online 方案？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-159">**Are there plans for OneDrive for Business and SharePoint Online to be PCI DSS-compliant outside of the United States?**</span></span>

<span data-ttu-id="2e8bb-160">目前符合 PCI DSS 規範的商務用 OneDrive 和 SharePoint Online 僅限美國。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-160">Currently OneDrive for Business and SharePoint Online is PCI-DSS compliant only in the United States (US).</span></span> <span data-ttu-id="2e8bb-161">Microsoft 會評估美國以外地區的需求和時間表，並在其他地區新增至藍圖時提供更新。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-161">Microsoft will evaluate the requirements and timelines for regions outside of US and provide updates when and if other regions are added to the roadmap.</span></span>

<span data-ttu-id="2e8bb-162">**[商務用 OneDrive] 和 [SharePoint Online] 的適用範圍為何？**</span><span class="sxs-lookup"><span data-stu-id="2e8bb-162">**What is in-scope for OneDrive for Business and SharePoint Online?**</span></span>

<span data-ttu-id="2e8bb-163">目前，只有上傳至 [商務用 OneDrive] 和 [SharePoint Online] 的檔案和文件符合 PCI DSS 的要求。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-163">Currently, only files and documents uploaded to OneDrive for Business and SharePoint Online will be compliant with PCI DSS.</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="2e8bb-164">使用 Microsoft 合規性管理員來評定風險</span><span class="sxs-lookup"><span data-stu-id="2e8bb-164">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="2e8bb-165">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-165">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="2e8bb-166">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-166">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="2e8bb-167">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-167">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="2e8bb-168">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="2e8bb-168">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="2e8bb-169">資源</span><span class="sxs-lookup"><span data-stu-id="2e8bb-169">Resources</span></span>

- [<span data-ttu-id="2e8bb-170">PCI 安全標準協會</span><span class="sxs-lookup"><span data-stu-id="2e8bb-170">PCI Security Standards Council</span></span>](https://www.pcisecuritystandards.org/)
- [<span data-ttu-id="2e8bb-171">PCI 資料安全性標準</span><span class="sxs-lookup"><span data-stu-id="2e8bb-171">PCI Data Security Standard</span></span>](https://www.pcisecuritystandards.org/documents/PCI_DSS_v3-1.pdf)
- [<span data-ttu-id="2e8bb-172">PCI DSS 快速參考指南</span><span class="sxs-lookup"><span data-stu-id="2e8bb-172">PCI DSS Quick Reference Guide</span></span>](https://www.pcisecuritystandards.org/documents/PCISSC%20QRG%20August%202014%20-print.pdf)
- [<span data-ttu-id="2e8bb-173">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="2e8bb-173">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
