---
title: '國防部門 (DoD) 影響等級 2 (IL2) '
description: 深入瞭解 Microsoft 如何滿足國防部門的 (DoD) 影響等級 2 (IL2) 標準。
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
ms.openlocfilehash: 77e8cb50f815c167e50293d495b4a548a73d022e
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385706"
---
# <a name="department-of-defense-dod-impact-level-2-il2"></a><span data-ttu-id="5556e-104">國防部門 (DoD) 影響等級 2 (IL2) </span><span class="sxs-lookup"><span data-stu-id="5556e-104">Department of Defense (DoD) Impact Level 2 (IL2)</span></span>

## <a name="dod-il2-overview"></a><span data-ttu-id="5556e-105">DoD IL2 概述</span><span class="sxs-lookup"><span data-stu-id="5556e-105">DoD IL2 overview</span></span>

<span data-ttu-id="5556e-106">國防 Information Systems 機關 (DISA) 是美國國防部 (DoD) 的代理人，負責開發及維護 DoD 雲端電腦 [安全性需求指南 (SRG) ](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)。</span><span class="sxs-lookup"><span data-stu-id="5556e-106">The Defense Information Systems Agency (DISA) is an agency of the US Department of Defense (DoD) that is responsible for developing and maintaining the DoD Cloud Computing [Security Requirements Guide (SRG)](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html).</span></span> <span data-ttu-id="5556e-107">SRG 會定義 DoD 用以評估雲端服務提供者 (CSP) 的安全性狀態的基準安全性需求，以支援 DoD 臨時授權 (PA) ，允許 CSP 主控 DoD 使命。</span><span class="sxs-lookup"><span data-stu-id="5556e-107">The SRG defines the baseline security requirements used by DoD to assess the security posture of a cloud service provider (CSP), supporting the decision to grant a DoD Provisional Authorization (PA) that allows a CSP to host DoD missions.</span></span> <span data-ttu-id="5556e-108">它包含、取代和 rescinds 先前發佈的 DoD 雲端安全性模型 (CSM) 和對應至 DoD 風險管理架構 (RMF) 。</span><span class="sxs-lookup"><span data-stu-id="5556e-108">It incorporates, supersedes, and rescinds the previously published DoD Cloud Security Model (CSM) and maps to the DoD Risk Management Framework (RMF).</span></span>

<span data-ttu-id="5556e-109">DISA 指南 DoD 以規劃及授權使用 CSP 的機構和部門。</span><span class="sxs-lookup"><span data-stu-id="5556e-109">DISA guides DoD agencies and departments in planning and authorizing the use of a CSP.</span></span> <span data-ttu-id="5556e-110">它也會評估與 SRG 相容性相關的 CSP 服務，這是一種授權程式，其中 Csp 可以提供檔，以概括顯示其與 DoD 標準的相容性。</span><span class="sxs-lookup"><span data-stu-id="5556e-110">It also evaluates CSP offerings for compliance with the SRG, an authorization process whereby CSPs can furnish documentation outlining their compliance with DoD standards.</span></span> <span data-ttu-id="5556e-111">在適當的情況下，它會 (PAs) DoD 臨時授權，因此 DoD 的代理商和支援組織可以使用雲端服務，而不必自行進行完整核准程式，節省時間和精力。</span><span class="sxs-lookup"><span data-stu-id="5556e-111">It issues DoD Provisional Authorizations (PAs) when appropriate, so DoD agencies and supporting organizations can use cloud services without having to go through a full approval process on their own, saving time and effort.</span></span>

<span data-ttu-id="5556e-112">[15 月 2014 DoD 的 CIO 備忘錄](https://www.esi.mil/contentview.aspx?id=585)，針對 *購買和使用商業性雲端計算服務的更新指導* 方針，其「FedRAMP 將充當所有 DoD 雲端服務的最低安全性基準。</span><span class="sxs-lookup"><span data-stu-id="5556e-112">The [15 December 2014 DoD CIO memo](https://www.esi.mil/contentview.aspx?id=585) regarding *Updated Guidance on the Acquisition and Use of Commercial Cloud Computing Services* states that 'FedRAMP will serve as the minimum security baseline for all DoD cloud services'.</span></span> <span data-ttu-id="5556e-113">SRG 會在所有資訊影響層級 (IL) 使用 FedRAMP 適中的基準，並考慮使用高基準。</span><span class="sxs-lookup"><span data-stu-id="5556e-113">The SRG uses the FedRAMP Moderate baseline at all information impact levels (IL) and considers the High Baseline at some.</span></span>

<span data-ttu-id="5556e-114">[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD 使用 FedRAMP 安全性控制* ，表明 IL2 資訊可能會主控于一個 CSP 中，該 CSP 最少保留 FedRAMP 適中的 Pa 及 DoD 層級2的 pa，遵循 Section 5.6.2 中所述的人員安全性需求。</span><span class="sxs-lookup"><span data-stu-id="5556e-114">[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD use of FedRAMP Security Controls* states that IL2 information may be hosted in a CSP that minimally holds a FedRAMP Moderate PA and a DoD Level 2 PA, subject to compliance with the personnel security requirements outlined in Section 5.6.2.</span></span> <span data-ttu-id="5556e-115">不過，此方法不會將 CSP 從其他安全性和整合需求，當作使命擁有者的要求來緩解。</span><span class="sxs-lookup"><span data-stu-id="5556e-115">However, this approach does not alleviate the CSP from meeting other security and integration requirements as required by the Mission Owner.</span></span> <span data-ttu-id="5556e-116">根據 [SRG 區段 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL2 位置和分割性需求*，FedRAMP 適中的 pa 會充分涵蓋 DoD IL2 pa，這樣就不會進一步評估 IL2 PA 的需求。</span><span class="sxs-lookup"><span data-stu-id="5556e-116">According to [SRG Section 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL2 Location and Separation Requirements*, DoD IL2 PA is adequately covered by a FedRAMP Moderate PA such that the requirements will not be additionally assessed for an IL2 PA.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="5556e-117">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="5556e-117">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="5556e-118">Azure</span><span class="sxs-lookup"><span data-stu-id="5556e-118">Azure</span></span>
- <span data-ttu-id="5556e-119">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="5556e-119">Dynamics 365</span></span>
- <span data-ttu-id="5556e-120">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="5556e-120">Microsoft Cloud App Security</span></span>
- <span data-ttu-id="5556e-121">適用於端點的 Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="5556e-121">Microsoft Defender for Endpoint</span></span>
- <span data-ttu-id="5556e-122">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5556e-122">Microsoft Graph</span></span>
- <span data-ttu-id="5556e-123">Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5556e-123">Microsoft Intune</span></span>
- <span data-ttu-id="5556e-124">Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="5556e-124">Microsoft Stream</span></span>
- <span data-ttu-id="5556e-125">Office 365美國政府，Office 365 美國政府-高</span><span class="sxs-lookup"><span data-stu-id="5556e-125">Office 365 U.S. Government, Office 365 U.S. Government - High</span></span>
- <span data-ttu-id="5556e-126">Power Apps</span><span class="sxs-lookup"><span data-stu-id="5556e-126">Power Apps</span></span>
- <span data-ttu-id="5556e-127">電源自動化</span><span class="sxs-lookup"><span data-stu-id="5556e-127">Power Automate</span></span>
- <span data-ttu-id="5556e-128">Power BI</span><span class="sxs-lookup"><span data-stu-id="5556e-128">Power BI</span></span>

## <a name="azure-dynamics-365-and-dod-il2"></a><span data-ttu-id="5556e-129">Azure、Dynamics 365 及 DoD IL2</span><span class="sxs-lookup"><span data-stu-id="5556e-129">Azure, Dynamics 365, and DoD IL2</span></span>

<span data-ttu-id="5556e-130">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [Azure DOD IL2](/azure/compliance/offerings/offering-dod-il2)service。</span><span class="sxs-lookup"><span data-stu-id="5556e-130">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure DoD IL2 offering](/azure/compliance/offerings/offering-dod-il2).</span></span>

## <a name="office-365-and-dod-il2"></a><span data-ttu-id="5556e-131">Office 365 和 DoD IL2</span><span class="sxs-lookup"><span data-stu-id="5556e-131">Office 365 and DoD IL2</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="5556e-132">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="5556e-132">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="5556e-133">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="5556e-133">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="5556e-134">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="5556e-134">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="5556e-135">**適用性**</span><span class="sxs-lookup"><span data-stu-id="5556e-135">**Applicability**</span></span> | <span data-ttu-id="5556e-136">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="5556e-136">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="5556e-137">**GCC**</span><span class="sxs-lookup"><span data-stu-id="5556e-137">**GCC**</span></span> | <span data-ttu-id="5556e-138">活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告，商務用 OneDrive，人員卡片，SharePoint 線上，商務用 Skype，Windows Ink</span><span class="sxs-lookup"><span data-stu-id="5556e-138">Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |
| <span data-ttu-id="5556e-139">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="5556e-139">**GCC High**</span></span> | <span data-ttu-id="5556e-140">活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告，商務用 OneDrive，人員卡片，SharePoint 線上，商務用 Skype，Windows Ink</span><span class="sxs-lookup"><span data-stu-id="5556e-140">Activity Feed Service, Bing Services, Delve, Exchange Online Protection, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="resources"></a><span data-ttu-id="5556e-141">資源</span><span class="sxs-lookup"><span data-stu-id="5556e-141">Resources</span></span>

- [<span data-ttu-id="5556e-142">Microsoft 政府解決方案</span><span class="sxs-lookup"><span data-stu-id="5556e-142">Microsoft government solutions</span></span>](https://www.microsoft.com/enterprise/government)
- [<span data-ttu-id="5556e-143">DoD 雲端電腦安全性性需求手冊</span><span class="sxs-lookup"><span data-stu-id="5556e-143">DoD Cloud Computing Security Requirements Guide</span></span>](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [<span data-ttu-id="5556e-144">FedRAMP 檔</span><span class="sxs-lookup"><span data-stu-id="5556e-144">FedRAMP documents</span></span>](https://www.fedramp.gov/documents/)
- <span data-ttu-id="5556e-145">[NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *風險管理架構：資訊系統和組織：系統安全性和隱私權的系統 Life-Cycle 方式*</span><span class="sxs-lookup"><span data-stu-id="5556e-145">[NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *Risk Management Framework for Information Systems and Organizations: A System Life-Cycle Approach for Security and Privacy*</span></span>
- <span data-ttu-id="5556e-146">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *的安全性和隱私權控制資訊系統和組織*</span><span class="sxs-lookup"><span data-stu-id="5556e-146">[NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *Security and Privacy Controls for Information Systems and Organizations*</span></span>
- <span data-ttu-id="5556e-147">[DoD 指令 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD 風險管理架構 (RMF) DoD 資訊技術* (</span><span class="sxs-lookup"><span data-stu-id="5556e-147">[DoD Instruction 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD Risk Management Framework (RMF) for DoD Information Technology (IT)*</span></span>
