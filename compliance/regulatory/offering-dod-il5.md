---
title: '國防部門 (DoD) 影響層級 5 (IL5) '
description: 深入瞭解 Microsoft 如何滿足國防部門 (DoD) 影響等級 5 (IL5) 標準。
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
ms.openlocfilehash: 9f92ed19a22b7eff8a7e9988e66c51aea90d42ab
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385707"
---
# <a name="department-of-defense-dod-impact-level-5-il5"></a><span data-ttu-id="6bfc9-104">國防部門 (DoD) 影響層級 5 (IL5) </span><span class="sxs-lookup"><span data-stu-id="6bfc9-104">Department of Defense (DoD) Impact Level 5 (IL5)</span></span>

## <a name="dod-il5-overview"></a><span data-ttu-id="6bfc9-105">DoD IL5 概述</span><span class="sxs-lookup"><span data-stu-id="6bfc9-105">DoD IL5 overview</span></span>

<span data-ttu-id="6bfc9-106">國防 Information Systems 機關 (DISA) 是美國國防部 (DoD) 的代理人，負責開發及維護 DoD 雲端電腦 [安全性需求指南 (SRG) ](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-106">The Defense Information Systems Agency (DISA) is an agency of the US Department of Defense (DoD) that is responsible for developing and maintaining the DoD Cloud Computing [Security Requirements Guide (SRG)](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html).</span></span> <span data-ttu-id="6bfc9-107">SRG 會定義 DoD 用以評估雲端服務提供者 (CSP) 的安全性狀態的基準安全性需求，以支援 DoD 臨時授權 (PA) ，允許 CSP 主控 DoD 使命。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-107">The SRG defines the baseline security requirements used by DoD to assess the security posture of a cloud service provider (CSP), supporting the decision to grant a DoD Provisional Authorization (PA) that allows a CSP to host DoD missions.</span></span> <span data-ttu-id="6bfc9-108">它包含、取代和 rescinds 先前發佈的 DoD 雲端安全性模型 (CSM) 和對應至 DoD 風險管理架構 (RMF) 。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-108">It incorporates, supersedes, and rescinds the previously published DoD Cloud Security Model (CSM) and maps to the DoD Risk Management Framework (RMF).</span></span>

<span data-ttu-id="6bfc9-109">DISA 指南 DoD 以規劃及授權使用 CSP 的機構和部門。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-109">DISA guides DoD agencies and departments in planning and authorizing the use of a CSP.</span></span> <span data-ttu-id="6bfc9-110">它也會評估與 SRG 相容性相關的 CSP 服務，這是一種授權程式，其中 Csp 可以提供檔，以概括顯示其與 DoD 標準的相容性。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-110">It also evaluates CSP offerings for compliance with the SRG, an authorization process whereby CSPs can furnish documentation outlining their compliance with DoD standards.</span></span> <span data-ttu-id="6bfc9-111">在適當的情況下，它會 (PAs) DoD 臨時授權，因此 DoD 的代理商和支援組織可以使用雲端服務，而不必自行進行完整核准程式，節省時間和精力。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-111">It issues DoD Provisional Authorizations (PAs) when appropriate, so DoD agencies and supporting organizations can use cloud services without having to go through a full approval process on their own, saving time and effort.</span></span>

<span data-ttu-id="6bfc9-112">根據 [SRG Section 3.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#3.2InformationImpactLevels) *資訊影響層級*，IL5 資訊涵蓋：</span><span class="sxs-lookup"><span data-stu-id="6bfc9-112">According to [SRG Section 3.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#3.2InformationImpactLevels) *Information Impact Levels*, IL5 information covers:</span></span>

- <span data-ttu-id="6bfc9-113">受管理的未分類資訊 (CUI) 需要更高的保護層級，而不是 IL4 所具備的保護</span><span class="sxs-lookup"><span data-stu-id="6bfc9-113">Controlled Unclassified Information (CUI) that requires higher level of protection than that afforded by IL4</span></span>
    - <span data-ttu-id="6bfc9-114">[CUI](https://www.archives.gov/cui)登錄會提供由執行的分支所保護的特定資訊類別，例如， [CUI 類別清單](https://www.archives.gov/cui/registry/category-list)中包含超過20個類別群組。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-114">The [CUI Registry](https://www.archives.gov/cui) provides specific categories of information that is under protection by the Executive branch, for example, more than 20 category groupings are included in the [CUI category list](https://www.archives.gov/cui/registry/category-list).</span></span>
    - <span data-ttu-id="6bfc9-115">[NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *保護 Nonfederal 系統和組織中受控的未分類資訊* ，供聯邦代理商用於合約或與非聯邦組織建立的其他合約。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-115">[NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations* is intended for use by federal agencies in contracts or other agreements established with non-federal organizations.</span></span>

- <span data-ttu-id="6bfc9-116">本國安全系統 (NSS) </span><span class="sxs-lookup"><span data-stu-id="6bfc9-116">National Security Systems (NSS)</span></span>
    - <span data-ttu-id="6bfc9-117">[NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) ， *識別區域安全性系統的資訊系統* 提供 NSS 的定義。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-117">[NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) *Guideline for Identifying an Information System as a National Security System* provides definitions of NSS.</span></span>
    - <span data-ttu-id="6bfc9-118">[CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security 分類和 Control Selection 針對全國的安全性系統，針對* 聯邦機關應套用來分類全國安全性資訊的安全性標準提供指導方針。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-118">[CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security Categorization and Control Selection for National Security Systems* provides guidance on the security standards that federal agencies should apply to categorize national security information.</span></span>

<span data-ttu-id="6bfc9-119">[15 月 2014 DoD 的 CIO 備忘錄](https://www.esi.mil/contentview.aspx?id=585)，針對 *購買和使用商業性雲端計算服務的更新指導* 方針，其「FedRAMP 將充當所有 DoD 雲端服務的最低安全性基準。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-119">The [15 December 2014 DoD CIO memo](https://www.esi.mil/contentview.aspx?id=585) regarding *Updated Guidance on the Acquisition and Use of Commercial Cloud Computing Services* states that 'FedRAMP will serve as the minimum security baseline for all DoD cloud services'.</span></span> <span data-ttu-id="6bfc9-120">SRG 會在所有資訊影響層級 (IL) 使用 FedRAMP 適中的基準，並考慮使用高基準。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-120">The SRG uses the FedRAMP Moderate baseline at all information impact levels (IL) and considers the High Baseline at some.</span></span>

<span data-ttu-id="6bfc9-121">[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD 使用 FedRAMP 安全性控制* ，說明 FedRAMP 的高 PA （結合 DoD 的 FedRAMP + 控制項和控制項增強功能） (C/CEs) 和 SRG 中的需求，是用來評估 awarding a IL5 的 a DoD PA。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-121">[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD use of FedRAMP Security Controls* states that a FedRAMP High PA, supplemented with DoD FedRAMP+ controls and control enhancements (C/CEs) and requirements in the SRG, are used to assess CSPs toward awarding a DoD PA at IL5.</span></span> <span data-ttu-id="6bfc9-122">不論使用何種 C/CE 基準做為 FedRAMP 高 PA 的基礎，在 IL5 中取得 DoD PA 之前，必須先評估並核准其他考慮和/或需求。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-122">No matter what C/CE baseline is used as the basis for a FedRAMP High PA, additional considerations and/or requirements will need to be assessed and approved before a DoD PA can be awarded at IL5.</span></span> <span data-ttu-id="6bfc9-123">具體說來， [SRG Section 5.1.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD FedRAMP + Security Controls/強化* 狀態在表2中，除了 FedRAMP 的高基線之外，還需要10個其他 C/CES，DoD IL5 PA。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-123">Specifically, [SRG Section 5.1.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD FedRAMP+ Security Controls/Enhancements* states in Table 2 that 10 additional C/CEs beyond the FedRAMP High baseline are required for a DoD IL5 PA.</span></span>

<span data-ttu-id="6bfc9-124">此外，根據 [SRG 區段 5.2.2.3](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL5 位置和分割性需求*，下列需求 (彼此之間的需求) 必須針對第5級的 PA 進行：</span><span class="sxs-lookup"><span data-stu-id="6bfc9-124">Moreover, according to [SRG Section 5.2.2.3](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL5 Location and Separation Requirements*, the following requirements (among others) must be in place for a Level 5 PA:</span></span>

- <span data-ttu-id="6bfc9-125">DoD 和聯邦政府承租人/使命之間的虛/邏輯分隔性已足夠。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-125">Virtual/logical separation between DoD and Federal Government tenants / missions is sufficient.</span></span> <span data-ttu-id="6bfc9-126">需要租使用者/使命系統之間的虛擬/邏輯分隔。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-126">Virtual/logical separation between tenant/mission systems is required.</span></span>
- <span data-ttu-id="6bfc9-127">從非 DoD/非聯邦政府租使用者實際的隔離 (（也就是「公用」、「州政府租使用者) ）。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-127">Physical separation from non-DoD/non-Federal Government tenants (that is, public, local/state government tenants) is required.</span></span>
- <span data-ttu-id="6bfc9-128">CSP 會限制對美國公民的 CSP 員工，對 DoD 和社區資訊的潛在存取權。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-128">The CSP restricts potential access to DoD's and the community's information to CSP employees that are U.S. Citizens.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="6bfc9-129">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="6bfc9-129">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="6bfc9-130">Azure</span><span class="sxs-lookup"><span data-stu-id="6bfc9-130">Azure</span></span>
- <span data-ttu-id="6bfc9-131">Dynamics 365 客戶服務</span><span class="sxs-lookup"><span data-stu-id="6bfc9-131">Dynamics 365 Customer Service</span></span>
- <span data-ttu-id="6bfc9-132">Microsoft Defender for Endpoint (以前是 Microsoft Defender 高級威脅防護) </span><span class="sxs-lookup"><span data-stu-id="6bfc9-132">Microsoft Defender for Endpoint (formerly Microsoft Defender Advanced Threat Protection)</span></span>
- <span data-ttu-id="6bfc9-133">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6bfc9-133">Microsoft Graph</span></span>
- <span data-ttu-id="6bfc9-134">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="6bfc9-134">Microsoft Stream</span></span>
- <span data-ttu-id="6bfc9-135">Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="6bfc9-135">Office 365 U.S. Government Defense</span></span>
- <span data-ttu-id="6bfc9-136">Power Automate (之前稱為 Microsoft Flow)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-136">Power Automate (formerly Microsoft Flow)</span></span>
- <span data-ttu-id="6bfc9-137">Power BI</span><span class="sxs-lookup"><span data-stu-id="6bfc9-137">Power BI</span></span>

## <a name="azure-dynamics-365-and-dod-il5"></a><span data-ttu-id="6bfc9-138">Azure、Dynamics 365 及 DoD IL5</span><span class="sxs-lookup"><span data-stu-id="6bfc9-138">Azure, Dynamics 365, and DoD IL5</span></span>

<span data-ttu-id="6bfc9-139">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [Azure DOD IL5](/azure/compliance/offerings/offering-dod-il5)service。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-139">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure DoD IL5 offering](/azure/compliance/offerings/offering-dod-il5).</span></span>

## <a name="office-365-and-dod-il5"></a><span data-ttu-id="6bfc9-140">Office 365 和 DoD IL5</span><span class="sxs-lookup"><span data-stu-id="6bfc9-140">Office 365 and DoD IL5</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="6bfc9-141">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="6bfc9-141">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="6bfc9-142">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="6bfc9-142">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="6bfc9-143">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="6bfc9-143">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="6bfc9-144">**適用性**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-144">**Applicability**</span></span> | <span data-ttu-id="6bfc9-145">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-145">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="6bfc9-146">**DoD**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-146">**DoD**</span></span> | <span data-ttu-id="6bfc9-147">活動摘要服務，Bing 服務，Exchange Online，Exchange Online Protection，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="6bfc9-147">Activity Feed Service, Bing Services, Exchange Online, Exchange Online Protection, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="attestation-documents"></a><span data-ttu-id="6bfc9-148">證明檔</span><span class="sxs-lookup"><span data-stu-id="6bfc9-148">Attestation documents</span></span>

<span data-ttu-id="6bfc9-149">我們的政府客戶可以提交套件存取要求表單，直接從[FedRAMP 的 Marketplace](https://marketplace.fedramp.gov/#!/products?sort=productName&productNameSearch=azure) Office 365 美國政府國防 FedRAMP 檔。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-149">US government customers can request Office 365 U.S. Government Defense FedRAMP documentation directly from the [FedRAMP Marketplace](https://marketplace.fedramp.gov/#!/products?sort=productName&productNameSearch=azure) by submitting a package access request form.</span></span> <span data-ttu-id="6bfc9-150">您必須具有 .gov 或 mil 的電子郵件地址，才能直接從 FedRAMP 存取 FedRAMP 的安全性套件。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-150">You must have a .gov or .mil email address to access a FedRAMP security package directly from FedRAMP.</span></span>

<span data-ttu-id="6bfc9-151">選取 [FedRAMP 和 DoD 檔，包括系統安全性計畫 (SSP) 、連續監控報告、動作和里程碑的計畫， (POA \& M) （如果有的話），您可以從「服務信任入口網站 [審核報告-FedRAMP 報表](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3) 」區段中的 [保密協定和暫止的存取授權] 中取得客戶。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-151">Select FedRAMP and DoD documentation, including System Security Plan (SSP), continuous monitoring reports, Plan of Action and Milestones (POA\&M), etc., is available to customers under NDA and pending access authorization from the Service Trust Portal [Audit Reports - FedRAMP Reports](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3) section.</span></span> <span data-ttu-id="6bfc9-152">請與您的 Microsoft 客戶代表聯繫以取得協助。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-152">Contact your Microsoft account representative for assistance.</span></span>

### <a name="resources"></a><span data-ttu-id="6bfc9-153">資源</span><span class="sxs-lookup"><span data-stu-id="6bfc9-153">Resources</span></span>

- [<span data-ttu-id="6bfc9-154">Microsoft 政府解決方案</span><span class="sxs-lookup"><span data-stu-id="6bfc9-154">Microsoft government solutions</span></span>](https://www.microsoft.com/enterprise/government)
- [<span data-ttu-id="6bfc9-155">DoD 雲端電腦安全性性需求手冊</span><span class="sxs-lookup"><span data-stu-id="6bfc9-155">DoD Cloud Computing Security Requirements Guide</span></span>](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [<span data-ttu-id="6bfc9-156">FedRAMP 檔</span><span class="sxs-lookup"><span data-stu-id="6bfc9-156">FedRAMP documents</span></span>](https://www.fedramp.gov/documents/)
- <span data-ttu-id="6bfc9-157">[DoD 指令 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD 風險管理架構 (RMF) DoD 資訊技術* (</span><span class="sxs-lookup"><span data-stu-id="6bfc9-157">[DoD Instruction 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF) for DoD Information Technology (IT)*</span></span>
- <span data-ttu-id="6bfc9-158">[NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *風險管理架構：資訊系統和組織：系統安全性和隱私權的系統 Life-Cycle 方式*</span><span class="sxs-lookup"><span data-stu-id="6bfc9-158">[NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *Risk Management Framework for Information Systems and Organizations: A System Life-Cycle Approach for Security and Privacy*</span></span>
- <span data-ttu-id="6bfc9-159">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *的安全性和隱私權控制資訊系統和組織*</span><span class="sxs-lookup"><span data-stu-id="6bfc9-159">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *Security and Privacy Controls for Information Systems and Organizations*</span></span>
- <span data-ttu-id="6bfc9-160">*將資訊系統識別為全國安全性系統的* [NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf)指導方針</span><span class="sxs-lookup"><span data-stu-id="6bfc9-160">[NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) *Guideline for Identifying an Information System as a National Security System*</span></span>
- <span data-ttu-id="6bfc9-161">[](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *適用于全國安全性系統的 CNSSI 1253 安全性分類和控制選項*</span><span class="sxs-lookup"><span data-stu-id="6bfc9-161">[CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security Categorization and Control Selection for National Security Systems*</span></span>
- <span data-ttu-id="6bfc9-162">[NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *保護 Nonfederal 系統和組織中受控未分類的資訊*</span><span class="sxs-lookup"><span data-stu-id="6bfc9-162">[NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations*</span></span>
- <span data-ttu-id="6bfc9-163">受管理的未分類資訊 (CUI) [Registry](https://www.archives.gov/cui) 和 CUI [類別清單](https://www.archives.gov/cui/registry/category-list)。</span><span class="sxs-lookup"><span data-stu-id="6bfc9-163">Controlled Unclassified Information (CUI) [Registry](https://www.archives.gov/cui) and CUI [category list](https://www.archives.gov/cui/registry/category-list).</span></span>
