---
title: 保護 Microsoft 365 基礎結構
description: 深入瞭解 Microsoft 如何保護 Microsoft 365 基礎結構。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 224900bd60f2fd5637e7264f1aed98d5ff878b20
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089616"
---
# <a name="securing-the-microsoft-365-infrastructure"></a><span data-ttu-id="b2f58-103">保護 Microsoft 365 基礎結構</span><span class="sxs-lookup"><span data-stu-id="b2f58-103">Securing the Microsoft 365 infrastructure</span></span>

<span data-ttu-id="b2f58-104">Microsoft 365 是世界上最大的企業和消費型雲端服務之一，而且會在客戶基礎、產品及功能方面，繼續迅速成長。</span><span class="sxs-lookup"><span data-stu-id="b2f58-104">Microsoft 365 is one of the largest enterprise and consumer cloud services in the world and continues to grow rapidly, both in customer base, products, and features.</span></span> <span data-ttu-id="b2f58-105">客戶 Microsoft 365 不僅適用于世界一流的生產力解決方案，還能協助保護其最機密的資訊，避免不斷演變的網路威脅環境。</span><span class="sxs-lookup"><span data-stu-id="b2f58-105">Customers turn to Microsoft 365 not only for its world-class productivity solutions, but to help protect their most sensitive information from the constantly evolving cyber threat landscape.</span></span> <span data-ttu-id="b2f58-106">這是 Microsoft 最重要的頭等大事，可讓客戶資料安全，並維護客戶信任。</span><span class="sxs-lookup"><span data-stu-id="b2f58-106">It is Microsoft's top priority to keep customer data secure and maintain customer trust.</span></span>

<span data-ttu-id="b2f58-107">保護此規模和複雜性的系統是不可能的，如果安全性是事後的，則只有在初始設計程式內整合安全性時，才會有效。</span><span class="sxs-lookup"><span data-stu-id="b2f58-107">Securing a system of this scale and complexity is not possible if security is an afterthought, it is only effective if security is integrated during the initial design process.</span></span> <span data-ttu-id="b2f58-108">它需要可靠的威脅偵測系統，並提供來自自動化系統和高素質工程師的提示回應。</span><span class="sxs-lookup"><span data-stu-id="b2f58-108">It requires a robust threat detection system with prompt responses from both automated systems and highly skilled engineers.</span></span> <span data-ttu-id="b2f58-109">連續評估和驗證這些系統是非常重要的，可確保安全設定保持不變，且會識別先前未知的漏洞。</span><span class="sxs-lookup"><span data-stu-id="b2f58-109">Continuous assessment and validation of these systems is essential to ensure secure configurations remain intact and previously unknown vulnerabilities are identified.</span></span>

## <a name="core-security-principles"></a><span data-ttu-id="b2f58-110">核心安全性原則</span><span class="sxs-lookup"><span data-stu-id="b2f58-110">Core security principles</span></span>

<span data-ttu-id="b2f58-111">七項安全性原則為我們的架構奠定了基礎，以 Microsoft 365 *防禦* 威脅、偵測 *和回應* 任何威脅，以及根據評估的結果不斷 *評估* 安全性狀況及改善服務。</span><span class="sxs-lookup"><span data-stu-id="b2f58-111">Seven security principles lay the foundation for our framework of *protecting* the Microsoft 365 services from threats, *detecting and responding* to any threats, and continuously *assessing* the security posture and improving services based on the results of those assessments.</span></span>

- <span data-ttu-id="b2f58-112">**資料隱私權**：客戶擁有其資料，而 Microsoft 是保管人。</span><span class="sxs-lookup"><span data-stu-id="b2f58-112">**Data privacy**: Customers own their data and Microsoft is the custodian.</span></span> <span data-ttu-id="b2f58-113">Microsoft 365 服務，除非客戶明確要求和核准，否則設計為無需使用工程師存取客戶資料。</span><span class="sxs-lookup"><span data-stu-id="b2f58-113">Microsoft 365 services are designed to operate without engineers accessing customer data, unless explicitly requested and approved by the customer.</span></span>
- <span data-ttu-id="b2f58-114">**假設** 損等：會以實際的方式處理個人和服務。</span><span class="sxs-lookup"><span data-stu-id="b2f58-114">**Assume breach**: Personnel and services are treated as though compromise is a real possibility.</span></span>
- <span data-ttu-id="b2f58-115">**最低許可權**：對資源的存取權和許可權，只限于執行必要工作所需的工作。</span><span class="sxs-lookup"><span data-stu-id="b2f58-115">**Least privilege**: Access and permissions to resources are limited to only what is necessary to perform needed tasks.</span></span>
- <span data-ttu-id="b2f58-116">**違反界限**：一個界限內的身分識別和基礎結構，會與其他界限中的資源隔離。</span><span class="sxs-lookup"><span data-stu-id="b2f58-116">**Breach boundaries**: Identities and infrastructure in one boundary are isolated from resources in other boundaries.</span></span> <span data-ttu-id="b2f58-117">損迭一個界限不應導致遭到其他威脅。</span><span class="sxs-lookup"><span data-stu-id="b2f58-117">Compromise of one boundary should not lead to compromise of another.</span></span>
- <span data-ttu-id="b2f58-118">**Service fabric 整合安全性**：安全優先級和需求已內置於新功能與功能的設計中，確保強大的安全性狀況可隨每個服務一起縮放。</span><span class="sxs-lookup"><span data-stu-id="b2f58-118">**Service fabric integrated security**: Security priorities and requirements are built into the design of new features and capabilities, ensuring that a strong security posture scales with each service.</span></span>
- <span data-ttu-id="b2f58-119">**自動化和自動**： Microsoft 著重于開發耐用的產品和架構，可讓您智慧化及自動強制執行服務安全性，同時讓 Microsoft 工程師能夠以規模的方式安全地管理回應安全性威脅。</span><span class="sxs-lookup"><span data-stu-id="b2f58-119">**Automated and automatic**: Microsoft focuses on developing durable products and architectures that can intelligently and automatically enforce service security, while giving Microsoft engineers the ability to safely manage responses to security threats at scale.</span></span>
- <span data-ttu-id="b2f58-120">**自我調整安全性**： Microsoft 的安全性功能可透過機器教學模型、常式滲透測試及自動化評估加以增強。</span><span class="sxs-lookup"><span data-stu-id="b2f58-120">**Adaptive security**: Microsoft security capabilities adapt to and are enhanced by machine learning models, routine penetration testing, and automated assessments.</span></span>

## <a name="protection"></a><span data-ttu-id="b2f58-121">保護</span><span class="sxs-lookup"><span data-stu-id="b2f58-121">Protection</span></span>

### <a name="access-control"></a><span data-ttu-id="b2f58-122">存取控制</span><span class="sxs-lookup"><span data-stu-id="b2f58-122">Access control</span></span>

<span data-ttu-id="b2f58-123">根據預設，負責開發及維護 Microsoft 365 服務的人員，在服務基礎結構中 (ZSA) 具有零的存取權。</span><span class="sxs-lookup"><span data-stu-id="b2f58-123">By default, personnel responsible for developing and maintaining Microsoft 365 services have Zero Standing Access (ZSA) to the service infrastructure.</span></span> <span data-ttu-id="b2f58-124">Microsoft 致力於只雇用最佳的工程師和嚴格的背景檢查，但 Microsoft 不會假設在運作服務中預設受信任。</span><span class="sxs-lookup"><span data-stu-id="b2f58-124">While Microsoft strives to hire only the best engineers and rigorous background checks are required, Microsoft does not assume that they are trusted by default in operating services.</span></span> <span data-ttu-id="b2f58-125">此外，當核准人員進行特殊許可權存取時，他們只會獲得有限期限的存取權，只會對特定範圍的服務基礎結構執行必要的動作。</span><span class="sxs-lookup"><span data-stu-id="b2f58-125">Additionally, when engineers are approved for privileged access, they are only granted access for a limited duration to perform only the actions needed for a specific scope of the service infrastructure.</span></span> <span data-ttu-id="b2f58-126">Microsoft 會將這些原則視為即時 (JIT) 和足夠的存取 (JEA) ，該是透過一名為密碼箱的系統來執行。</span><span class="sxs-lookup"><span data-stu-id="b2f58-126">Microsoft refers to these policies as Just-in-Time (JIT) and Just-Enough-Access (JEA) which are implemented through a system called Lockbox.</span></span>

<span data-ttu-id="b2f58-127">若要取得更高的許可權，Microsoft 工程師會送出特定任務的要求，並指定執行它的時間範圍。</span><span class="sxs-lookup"><span data-stu-id="b2f58-127">To acquire elevated privileges, Microsoft engineers submit a request for the specific task and specify the time frame to perform it.</span></span> <span data-ttu-id="b2f58-128">一旦核准，密碼箱便會產生專用的 JIT 帳戶，只具備執行所要求之工作的能力。</span><span class="sxs-lookup"><span data-stu-id="b2f58-128">Once approved, Lockbox generates a specialized JIT account with the ability to perform only the requested task.</span></span> <span data-ttu-id="b2f58-129">動作通常採取自動化工作流程的形式，以安全地執行所需的任何疑難排解或復原。</span><span class="sxs-lookup"><span data-stu-id="b2f58-129">Actions usually take the form of automated workflows that securely perform any troubleshooting or recovery required.</span></span> <span data-ttu-id="b2f58-130">在極少數的情況下，必須直接存取基礎結構時，嚴格監控的特殊許可權存取工作站 (PAWs) 是必要的。</span><span class="sxs-lookup"><span data-stu-id="b2f58-130">In rare instances when direct access to the infrastructure is necessary, strictly monitored Privileged Access Workstations (PAWs) are required.</span></span>

<span data-ttu-id="b2f58-131">惡意使用者和遭破壞的帳戶在任何組織中都有實際的可能性，而且我們的存取控制系統是為了防範這些威脅而設計的。</span><span class="sxs-lookup"><span data-stu-id="b2f58-131">Rogue users and compromised accounts are a real possibility in any organization, and our access control system are designed to protect against these threats.</span></span>

<span data-ttu-id="b2f58-132">如需存取控制的詳細資訊，請參閱 [Identity and access management 一覽](assurance-identity-and-access-management.md)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-132">For more information about access control, see [Identity and access management overview](assurance-identity-and-access-management.md).</span></span>

### <a name="encryption"></a><span data-ttu-id="b2f58-133">加密</span><span class="sxs-lookup"><span data-stu-id="b2f58-133">Encryption</span></span>

<span data-ttu-id="b2f58-134">雖然存取控制在防護 Microsoft 365 服務中提供重要的角色，但整個資料生命週期都使用加密，以進一步保護 Microsoft 客戶的機密性和隱私權。</span><span class="sxs-lookup"><span data-stu-id="b2f58-134">While access controls provide a vital role in defending Microsoft 365 services, encryption is used throughout the data lifecycle to further protect confidentiality and privacy for Microsoft customers.</span></span>

<span data-ttu-id="b2f58-135">用戶端電腦、Microsoft 365 伺服器和非 Microsoft 365 伺服器之間傳輸的資料會使用 TLS 1.2 加密。</span><span class="sxs-lookup"><span data-stu-id="b2f58-135">Data in transit between client machines, Microsoft 365 servers, and non-Microsoft 365 servers is encrypted using TLS 1.2.</span></span> <span data-ttu-id="b2f58-136">我們會定期查看使用中的密碼和通訊協定，並在必要時新增已改進的通訊協定，並移除較弱的通訊協定。</span><span class="sxs-lookup"><span data-stu-id="b2f58-136">We regularly review the ciphers and protocols in use, adding improved protocols when available and removing weaker ones as needed.</span></span>

<span data-ttu-id="b2f58-137">Microsoft server 上的客戶內容會在大量使用 BitLocker 的磁片區層級加密。</span><span class="sxs-lookup"><span data-stu-id="b2f58-137">Customer content at rest on Microsoft servers is encrypted at the volume-level using BitLocker.</span></span> <span data-ttu-id="b2f58-138">另外，您也可以使用由 Microsoft 或客戶管理的金鑰來套用應用層級加密。</span><span class="sxs-lookup"><span data-stu-id="b2f58-138">Application-level encryption can additionally be applied using keys managed by either Microsoft or the customer.</span></span> <span data-ttu-id="b2f58-139">只有透過 JIT 和 JEA 處理常式授權和核准時，才可以存取 Microsoft 受管理的金鑰。</span><span class="sxs-lookup"><span data-stu-id="b2f58-139">Access to Microsoft-managed keys is only possible when authorized and approved through the JIT and JEA process.</span></span>

<span data-ttu-id="b2f58-140">如需 Microsoft 365 中加密的相關資訊，請參閱[encryption and key management 概述](assurance-encryption.md)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-140">For more information about encryption in Microsoft 365, see [Encryption and key management overview](assurance-encryption.md).</span></span>

### <a name="network-isolation"></a><span data-ttu-id="b2f58-141">網路隔離</span><span class="sxs-lookup"><span data-stu-id="b2f58-141">Network isolation</span></span>

<span data-ttu-id="b2f58-142">根據最低許可權的原則，Microsoft 365 會限制服務基礎結構不同部分之間的通訊，只會限制運作的必要部分。</span><span class="sxs-lookup"><span data-stu-id="b2f58-142">In line with the principle of least privilege, Microsoft 365 restricts communication between different parts of the service infrastructure to only what is necessary to operate.</span></span> <span data-ttu-id="b2f58-143">根據預設，會拒絕所有網路流量，但只會明確定義所允許的通訊。</span><span class="sxs-lookup"><span data-stu-id="b2f58-143">All network traffic is denied by default, with only explicitly defined communication being allowed.</span></span> <span data-ttu-id="b2f58-144">這種限制會在整個基礎結構中建立違規界限。</span><span class="sxs-lookup"><span data-stu-id="b2f58-144">This restriction establishes breach boundaries throughout the infrastructure.</span></span> <span data-ttu-id="b2f58-145">若要將新的網路路徑新增至其服務以容納新功能的 Teams，必須先評估並核准要求，才能開啟此要求。</span><span class="sxs-lookup"><span data-stu-id="b2f58-145">Teams that would like to add new network paths to accommodate a new feature to their service must have the request evaluated and approved before it can be opened.</span></span>

<span data-ttu-id="b2f58-146">如需 Microsoft 365 中的網路隔離的詳細資訊，請參閱[Microsoft 365 隔離控制項](/microsoft-365/enterprise/microsoft-365-isolation-controls)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-146">For more information about network isolation in Microsoft 365, see [Microsoft 365 isolation controls](/microsoft-365/enterprise/microsoft-365-isolation-controls).</span></span>

## <a name="detection--response"></a><span data-ttu-id="b2f58-147">偵測 & 回應</span><span class="sxs-lookup"><span data-stu-id="b2f58-147">Detection & Response</span></span>

### <a name="security-monitoring"></a><span data-ttu-id="b2f58-148">安全性監視</span><span class="sxs-lookup"><span data-stu-id="b2f58-148">Security monitoring</span></span>

<span data-ttu-id="b2f58-149">Microsoft 大規模的安全性監控只有透過使用自動雲端式解決方案產生高準確性的警示時，才有可能。</span><span class="sxs-lookup"><span data-stu-id="b2f58-149">Security monitoring at Microsoft's massive scale is only possible by generating highly accurate alerts using automated cloud-based solutions.</span></span> <span data-ttu-id="b2f58-150">從整個核心基礎結構收集的每一個服務和遙測資料中的審計記錄會傳送至專屬的「集中近即時處理及警示」解決方案。</span><span class="sxs-lookup"><span data-stu-id="b2f58-150">Audit logs from each service and telemetry data gathered from throughout the core infrastructure is sent to a proprietary centralized near-real-time processing and alerting solution.</span></span>

<span data-ttu-id="b2f58-151">盡可能使用自動觸發的動作修正偵測到的威脅。</span><span class="sxs-lookup"><span data-stu-id="b2f58-151">Detected threats are remediated using automatically triggered actions when possible.</span></span> <span data-ttu-id="b2f58-152">當自動方案未成功或無法解決問題時，Microsoft 工程師會立即採取行動來緩解威脅。</span><span class="sxs-lookup"><span data-stu-id="b2f58-152">When automated solutions are unsuccessful or incapable of resolving the issue, on-call Microsoft engineers immediately take action to mitigate the threat.</span></span>

<span data-ttu-id="b2f58-153">如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[安全性監視概述](assurance-security-monitoring.md)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-153">For more information about security monitoring in Microsoft 365, see [Security monitoring overview](assurance-security-monitoring.md).</span></span>

## <a name="assessment"></a><span data-ttu-id="b2f58-154">評估</span><span class="sxs-lookup"><span data-stu-id="b2f58-154">Assessment</span></span>

### <a name="automated-assessments"></a><span data-ttu-id="b2f58-155">自動評估</span><span class="sxs-lookup"><span data-stu-id="b2f58-155">Automated assessments</span></span>

<span data-ttu-id="b2f58-156">不論系統的設計方式為何，安全性狀況都會因故意和無意間的設定偏差隨著時間而降低。</span><span class="sxs-lookup"><span data-stu-id="b2f58-156">Regardless of how a system is designed, the security posture can degrade due to intentional and unintentional configuration drift over time.</span></span> <span data-ttu-id="b2f58-157">自動工具會持續評估尋找未修補及配置錯誤之服務的 Microsoft 365 系統。</span><span class="sxs-lookup"><span data-stu-id="b2f58-157">Automated tools constantly assess Microsoft 365 systems that look for unpatched and misconfigured services.</span></span> <span data-ttu-id="b2f58-158">這種評估通常稱為「修補」、「反病毒」、「弱點」和「設定掃描」 (PAVC) 。</span><span class="sxs-lookup"><span data-stu-id="b2f58-158">This assessment is often referred to as patching, anti-virus, vulnerability, and configuration scanning (PAVC).</span></span>

<span data-ttu-id="b2f58-159">我們也會經常驗證我們的架構，以找出未使用的開啟埠和具有管理存取權的帳戶等實例。</span><span class="sxs-lookup"><span data-stu-id="b2f58-159">Our architecture is also frequently validated, identifying instances such as unused open ports and accounts with standing administrative access.</span></span> <span data-ttu-id="b2f58-160">任何從預先定義的所需狀態偏差的服務都會自動重新排列成對齊。</span><span class="sxs-lookup"><span data-stu-id="b2f58-160">Any services that drift from a pre-defined desired state are automatically brought back into alignment.</span></span>

<span data-ttu-id="b2f58-161">如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[弱點管理概述](assurance-vulnerability-management.md)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-161">For more information about security monitoring in Microsoft 365, see [Vulnerability management overview](assurance-vulnerability-management.md).</span></span>

### <a name="attack-simulation-and-penetration-testing"></a><span data-ttu-id="b2f58-162">攻擊模擬和滲透測試</span><span class="sxs-lookup"><span data-stu-id="b2f58-162">Attack simulation and penetration testing</span></span>

<span data-ttu-id="b2f58-163">Microsoft 365 的最大優先順序是防止攻擊 infiltrating 防禦。</span><span class="sxs-lookup"><span data-stu-id="b2f58-163">Microsoft 365's top priority is to prevent attacks from infiltrating defenses.</span></span> <span data-ttu-id="b2f58-164">Microsoft 365 擁有一支專門的安全性專家小組，這些專家會持續進行模擬攻擊，識別先前未知的漏洞，並提供大量資料流程，以改善安全性監控功能。</span><span class="sxs-lookup"><span data-stu-id="b2f58-164">Microsoft 365 has a dedicated team of security experts who are constantly conducting simulated attacks to identify previously unknown vulnerabilities and to provide a constant stream of rich data to improve security monitoring capabilities.</span></span> <span data-ttu-id="b2f58-165">這些模擬型攻擊採用一種頻繁的自動小型攻擊和專家導向的深度 dives。</span><span class="sxs-lookup"><span data-stu-id="b2f58-165">These simulated attacks take the form of frequent automated small-scale attacks and expert-driven deep dives.</span></span> <span data-ttu-id="b2f58-166">在這些活動中，Microsoft 會評估偵測、回應及逐出攻擊者的能力。</span><span class="sxs-lookup"><span data-stu-id="b2f58-166">From these activities, Microsoft evaluates the ability to detect, respond, and evict attackers.</span></span>

<span data-ttu-id="b2f58-167">如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[Microsoft 365 中的攻擊模擬](assurance-monitoring-and-testing.md)。</span><span class="sxs-lookup"><span data-stu-id="b2f58-167">For more information about security monitoring in Microsoft 365, see [Attack simulation in Microsoft 365](assurance-monitoring-and-testing.md).</span></span>

## <a name="resources"></a><span data-ttu-id="b2f58-168">資源</span><span class="sxs-lookup"><span data-stu-id="b2f58-168">Resources</span></span>

[<span data-ttu-id="b2f58-169">在幕後：保護 Microsoft 365 服務電源的基礎結構</span><span class="sxs-lookup"><span data-stu-id="b2f58-169">Behind the Scenes: Securing the Infrastructure Powering the Microsoft 365 Service</span></span>](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
