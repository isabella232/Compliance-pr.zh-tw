---
title: Microsoft 365 安全性事件管理：偵測和分析
description: 本文概要說明 Microsoft 365 中的安全性事件管理偵測和分析處理常式。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
f1.keywords:
- NOCSH
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 1fbdca0c0b08c793732ba31414bedd943d4dc115
ms.sourcegitcommit: d67e4d4fdc664f1da450c8ef2f6732e19bdd403a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037585"
---
# <a name="microsoft-365-security-incident-management-detection-and-analysis"></a><span data-ttu-id="0f881-103">Microsoft 365 安全性事件管理：偵測和分析</span><span class="sxs-lookup"><span data-stu-id="0f881-103">Microsoft 365 security incident management: Detection and analysis</span></span>

<span data-ttu-id="0f881-104">為了偵測惡意活動，Microsoft 365 會集中記錄安全性事件及其他資料，並執行各種分析技術，以找出反常或可疑的活動。</span><span class="sxs-lookup"><span data-stu-id="0f881-104">To detect malicious activity, Microsoft 365 centrally logs security events and other data and performs various analytical techniques to find anomalous or suspicious activity.</span></span> <span data-ttu-id="0f881-105">記錄檔是從 Microsoft 365 伺服器和基礎結構裝置收集，並儲存在中央和整合資料庫中。</span><span class="sxs-lookup"><span data-stu-id="0f881-105">Log files are collected from Microsoft 365 servers and infrastructure devices and stored in a central and consolidated database.</span></span>

<span data-ttu-id="0f881-106">Microsoft 採取以風險為基礎的方法來偵測惡意活動。</span><span class="sxs-lookup"><span data-stu-id="0f881-106">Microsoft takes a risk-based approach to detecting malicious activity.</span></span> <span data-ttu-id="0f881-107">我們使用事件資料和威脅情報來定義偵測並設定其優先順序。</span><span class="sxs-lookup"><span data-stu-id="0f881-107">We use incident data and threat intelligence to define and prioritize our detections.</span></span>

<span data-ttu-id="0f881-108">使用具有極高經驗、熟練、熟練之人員的團隊是偵測和分析階段成功的最重要的分項之一。</span><span class="sxs-lookup"><span data-stu-id="0f881-108">Employing a team of highly experienced, proficient, and skilled people is one of the most important pillars to success in the detection and analysis phase.</span></span> <span data-ttu-id="0f881-109">Microsoft 365 使用多個服務小組，而這些小組的員工在堆疊內的所有元件上都有其能力，包括網路、路由器、防火牆、負載平衡器、作業系統和應用程式。</span><span class="sxs-lookup"><span data-stu-id="0f881-109">Microsoft 365 employs multiple service teams, and those teams include employees with competencies on all components within the stack, including the network, routers, firewalls, load balancers, operating systems, and applications.</span></span>

<span data-ttu-id="0f881-110">Microsoft 365 中的安全性偵測機制也包含不同來源所啟動的通知及警示。</span><span class="sxs-lookup"><span data-stu-id="0f881-110">The security detection mechanisms in Microsoft 365 also include notification and alerts that are initiated by different sources.</span></span> <span data-ttu-id="0f881-111">Microsoft 365 安全性回應小組是安全性事件升級程式的重要 orchestrator。</span><span class="sxs-lookup"><span data-stu-id="0f881-111">The Microsoft 365 Security Response team is the key orchestrator of the security incident escalation process.</span></span> <span data-ttu-id="0f881-112">此小組接收所有升級，並負責分析和確認安全性事件的有效性。</span><span class="sxs-lookup"><span data-stu-id="0f881-112">This team receives all escalations and is responsible for analyzing and confirming the validity of the security incident.</span></span>

<span data-ttu-id="0f881-113">偵測的其中一個主要主要專案是通知：</span><span class="sxs-lookup"><span data-stu-id="0f881-113">One of the primary pillars of detection is notification:</span></span>

- <span data-ttu-id="0f881-114">每個服務小組負責根據 Microsoft 365 安全小組的需求，記錄服務中的任何動作或事件。</span><span class="sxs-lookup"><span data-stu-id="0f881-114">Each service team is responsible to log any action or event inside the service based on the requirements from the Microsoft 365 Security team.</span></span> <span data-ttu-id="0f881-115">由不同服務小組所建立的所有記錄，都是由安全性資訊和事件管理 (SIEM) 解決方案搭配預先定義的安全性和偵測規則處理。</span><span class="sxs-lookup"><span data-stu-id="0f881-115">All logs created by the different service teams are processed by a Security Information and Event Management (SIEM) solution with predefined security and detection rules.</span></span> <span data-ttu-id="0f881-116">這些規則會根據 Microsoft 365 安全小組的建議演變，以瞭解先前安全性事件的資訊，判斷是否有任何可疑或惡意的活動。</span><span class="sxs-lookup"><span data-stu-id="0f881-116">These rules evolve based on the Microsoft 365 Security team’s recommendation, on information learned from previous security incidents, to determine if there is any suspicious or malicious activity.</span></span>
- <span data-ttu-id="0f881-117">如果客戶決定安全性事件正在進行中，則他們可能會開啟 Microsoft 的支援案例，它會指派給 microsoft 365 客戶經驗 (CxP) 通訊小組，並將其轉換為所有適當的團隊。</span><span class="sxs-lookup"><span data-stu-id="0f881-117">If a customer determines that a security incident is underway, they may open a support case with Microsoft, which is assigned to the Microsoft 365 Customer Experience (CxP) Communications team and turned into an escalation to all appropriate teams.</span></span>

<span data-ttu-id="0f881-118">Microsoft 365 服務小組也會使用透過安全性監控和登入在趨勢分析中取得的情報，以偵測可能表示攻擊或安全性事件的 Microsoft 365 資訊系統中的 abnormalities。</span><span class="sxs-lookup"><span data-stu-id="0f881-118">Microsoft 365 service teams also use the intelligence gained in trend analysis through security monitoring and logging to detect abnormalities in Microsoft 365 information systems that might indicate an attack or a security incident.</span></span> <span data-ttu-id="0f881-119">Microsoft 365 伺服器會將來自實際執行環境中這些記錄的輸出匯總到集中式記錄伺服器。</span><span class="sxs-lookup"><span data-stu-id="0f881-119">Microsoft 365 servers aggregate output from these logs in the production environment into a centralized logging server.</span></span> <span data-ttu-id="0f881-120">在此集中式記錄伺服器中，會在整個實際執行環境中檢查記錄的位置趨勢。</span><span class="sxs-lookup"><span data-stu-id="0f881-120">From this centralized logging server, logs are examined to spot trends throughout the production environment.</span></span> <span data-ttu-id="0f881-121">集中式伺服器中匯總的資料會安全地傳送至記錄服務，以進行高級查詢、儀表板建立及偵測反常和惡意活動。</span><span class="sxs-lookup"><span data-stu-id="0f881-121">Data aggregated in the centralized server is securely transmitted into a logging service for advanced querying, dashboard building and detecting anomalous and malicious activity.</span></span> <span data-ttu-id="0f881-122">服務也會使用機器學習來偵測記錄輸出的異常情況。</span><span class="sxs-lookup"><span data-stu-id="0f881-122">The service also uses machine learning to detect anomalies with log output.</span></span>

<span data-ttu-id="0f881-123">在升級期間（取決於安全性事件的性質），Microsoft 365 的安全性回應小組可能會從 Microsoft 的各個小組吸引一或多個主題專家：</span><span class="sxs-lookup"><span data-stu-id="0f881-123">During the escalation phase and depending on the nature of the security incident, the Microsoft 365 Security Response team may engage one or more subject matter experts from various teams at Microsoft:</span></span>

- <span data-ttu-id="0f881-124">線上服務安全性與合規性小組</span><span class="sxs-lookup"><span data-stu-id="0f881-124">Online Services Security and Compliance team</span></span>
- <span data-ttu-id="0f881-125">Microsoft 威脅情報中心 (MSTIC) </span><span class="sxs-lookup"><span data-stu-id="0f881-125">Microsoft Threat Intelligence Center (MSTIC)</span></span>
- <span data-ttu-id="0f881-126">Microsoft 安全性回應中心 (MSRC) </span><span class="sxs-lookup"><span data-stu-id="0f881-126">Microsoft Security Response Center (MSRC)</span></span>
- <span data-ttu-id="0f881-127">公司、外部及法律事務 (CELA) </span><span class="sxs-lookup"><span data-stu-id="0f881-127">Corporate, External, and Legal Affairs (CELA)</span></span>
- <span data-ttu-id="0f881-128">Azure 安全性</span><span class="sxs-lookup"><span data-stu-id="0f881-128">Azure Security</span></span>
- <span data-ttu-id="0f881-129">Microsoft 365 工程及其他。</span><span class="sxs-lookup"><span data-stu-id="0f881-129">Microsoft 365 engineering, and others.</span></span>

<span data-ttu-id="0f881-130">在升級至 Microsoft 365 安全性回應小組之前，服務小組負責根據定義的準則決定及設定安全性事件的嚴重性層級，例如：</span><span class="sxs-lookup"><span data-stu-id="0f881-130">Before any escalation to the Microsoft 365 Security Response team occurs, the service team is responsible for determining and setting the severity level of the security incident based on defined criteria such as:</span></span>

- <span data-ttu-id="0f881-131">隱私權</span><span class="sxs-lookup"><span data-stu-id="0f881-131">Privacy</span></span>
- <span data-ttu-id="0f881-132">影響</span><span class="sxs-lookup"><span data-stu-id="0f881-132">Impact</span></span>
- <span data-ttu-id="0f881-133">範圍</span><span class="sxs-lookup"><span data-stu-id="0f881-133">Scope</span></span>
- <span data-ttu-id="0f881-134">受影響的承租人數目</span><span class="sxs-lookup"><span data-stu-id="0f881-134">Number of affected tenants</span></span>
- <span data-ttu-id="0f881-135">地區</span><span class="sxs-lookup"><span data-stu-id="0f881-135">Region</span></span>
- <span data-ttu-id="0f881-136">服務</span><span class="sxs-lookup"><span data-stu-id="0f881-136">Service</span></span>
- <span data-ttu-id="0f881-137">事件的詳細資料</span><span class="sxs-lookup"><span data-stu-id="0f881-137">Details of the incident</span></span>
- <span data-ttu-id="0f881-138">特定客戶行業或市場規定。</span><span class="sxs-lookup"><span data-stu-id="0f881-138">Specific customer industry or market regulations.</span></span>

<span data-ttu-id="0f881-139">事件優先順序取決於使用不同的因素，包括但不限於事件的功能影響、事件的資訊影響，以及事件的可復原性。</span><span class="sxs-lookup"><span data-stu-id="0f881-139">Incident prioritization is determined by using distinct factors, including but not limited to the functional impact of the incident, the informational impact of the incident, and the recoverability from the incident.</span></span>

<span data-ttu-id="0f881-140">收到有關安全性事件的上報之後，Microsoft 365 安全小組會將虛擬小組組織 (v 小組) 由 Microsoft 365 安全性回應小組、服務小組和 Microsoft 365 事件通訊小組組成的成員組成。</span><span class="sxs-lookup"><span data-stu-id="0f881-140">After receiving an escalation about a security incident, the Microsoft 365 Security team organizes a virtual team (v-team) comprised of members from Microsoft 365 Security Response team, service teams, and the Microsoft 365 Incident Communication team.</span></span> <span data-ttu-id="0f881-141">此 v 小組活動的較複雜部分是確認安全性事件，並消除任何誤報。</span><span class="sxs-lookup"><span data-stu-id="0f881-141">The more complex part of activities of this v-team is to confirm the security incident and to eliminate any false positives.</span></span> <span data-ttu-id="0f881-142">準備階段中所確定的指示器所提供資訊的準確性很重要。</span><span class="sxs-lookup"><span data-stu-id="0f881-142">The accuracy of information provided by the indicators determined in the preparation phase is critical.</span></span> <span data-ttu-id="0f881-143">透過依向量攻擊類別來分析此資訊，「五團隊」可以判斷安全性事件是否為合理考慮。</span><span class="sxs-lookup"><span data-stu-id="0f881-143">By analyzing this information by category of vector attack, the v-team can determine if the security incident is a legitimate concern.</span></span>

<span data-ttu-id="0f881-144">在調查開始時，Office 安全性事件回應小組會依照案例管理原則記錄事件的所有相關資訊。</span><span class="sxs-lookup"><span data-stu-id="0f881-144">At the beginning of the investigation, the Office Security Incident Response team records all information about the incident according to our case management policies.</span></span> <span data-ttu-id="0f881-145">隨著案例的進展，我們追蹤進行中的動作，並遵循證據處理標準，以在整個事件週期內收集、保留及保護此資料。</span><span class="sxs-lookup"><span data-stu-id="0f881-145">As the case progresses, we track ongoing actions and follow evidence handling standards for gathering, retaining, and securing this data throughout the incident lifecycle.</span></span>

<span data-ttu-id="0f881-146">這些動作的一些範例包括：</span><span class="sxs-lookup"><span data-stu-id="0f881-146">Some examples of these actions would include:</span></span>

- <span data-ttu-id="0f881-147">摘要，這是事件及其潛在影響的簡短描述</span><span class="sxs-lookup"><span data-stu-id="0f881-147">A summary, which is a brief description of the incident and its potential impact</span></span>
- <span data-ttu-id="0f881-148">事件的嚴重性和優先順序，它們是透過評估潛在影響來衍生</span><span class="sxs-lookup"><span data-stu-id="0f881-148">The incident's severity and priority, which are derived by assessing the potential impact</span></span>
- <span data-ttu-id="0f881-149">所有識別出導致事件發生的標記的清單</span><span class="sxs-lookup"><span data-stu-id="0f881-149">A list of all indicators identified which led to detection of the incident</span></span>
- <span data-ttu-id="0f881-150">任何相關事件的清單</span><span class="sxs-lookup"><span data-stu-id="0f881-150">A list of any related incidents</span></span>
- <span data-ttu-id="0f881-151">由 v 小組採取的所有動作清單</span><span class="sxs-lookup"><span data-stu-id="0f881-151">A list of all actions taken by the v-team</span></span>
- <span data-ttu-id="0f881-152">任何收集的證據，也會保留以供檢討後分析和未來的鑒證調查。</span><span class="sxs-lookup"><span data-stu-id="0f881-152">Any gathered evidence, which will also be preserved for post-mortem analysis and future forensic investigations</span></span>
- <span data-ttu-id="0f881-153">建議的後續步驟和動作</span><span class="sxs-lookup"><span data-stu-id="0f881-153">Recommended next steps and actions</span></span>

<span data-ttu-id="0f881-154">在安全性事件確認之後，Microsoft 365 安全回應小組和適當的服務小組主要目標是包含攻擊、保護服務 () 受到攻擊，以及避免全域影響較大。</span><span class="sxs-lookup"><span data-stu-id="0f881-154">After security incident confirmation, the primary goals of the Microsoft 365 Security Response team and the appropriate service team are to contain the attack, to protect the service(s) under attack, and to avoid a greater global impact.</span></span> <span data-ttu-id="0f881-155">在同一時間，適當的工程小組會運作，以判斷根本原因，並準備第一個復原計畫。</span><span class="sxs-lookup"><span data-stu-id="0f881-155">At the same time, the appropriate engineering teams work to determine the root cause and to prepare the first recovery plan.</span></span>

<span data-ttu-id="0f881-156">在下一個階段中，Microsoft 365 安全性回應小組會識別由安全性事件（如果有的話）所影響的客戶 () 。</span><span class="sxs-lookup"><span data-stu-id="0f881-156">In the next phase, the Microsoft 365 Security Response team identifies the customer(s) affected by the security incident, if any.</span></span> <span data-ttu-id="0f881-157">影響範圍可能需要一些時間，以根據地區、資料中心、服務、伺服器陣列、伺服器等來判斷。</span><span class="sxs-lookup"><span data-stu-id="0f881-157">The scope of effect can take some time to determine, based on region, datacenter, service, server farm, server, and so forth.</span></span> <span data-ttu-id="0f881-158">受影響客戶的清單是由服務小組和 Microsoft 365 CxP 通訊小組所編譯，然後負責處理合約和合規性義務中的客戶通知程式。</span><span class="sxs-lookup"><span data-stu-id="0f881-158">The list of affected customers is compiled by the service team and the Microsoft 365 CxP Communications team, who then handle the customer notification process within contractual and compliance obligations.</span></span>

## <a name="related-articles"></a><span data-ttu-id="0f881-159">相關文章</span><span class="sxs-lookup"><span data-stu-id="0f881-159">Related articles</span></span>

- [<span data-ttu-id="0f881-160">Microsoft 365 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="0f881-160">Microsoft 365 security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="0f881-161">Microsoft 365 的安全性事件管理準備</span><span class="sxs-lookup"><span data-stu-id="0f881-161">Microsoft 365 security incident management preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="0f881-162">Microsoft 365 的安全性事件管理包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="0f881-162">Microsoft 365 security incident management containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
- [<span data-ttu-id="0f881-163">Microsoft 365 安全性事件管理後置事件活動</span><span class="sxs-lookup"><span data-stu-id="0f881-163">Microsoft 365 security incident management post-incident activity</span></span>](assurance-sim-post-incident-activity.md)
