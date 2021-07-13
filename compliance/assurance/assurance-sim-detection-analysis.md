---
title: Microsoft 安全性事件管理：偵測和分析
description: 本文概要說明 Microsoft online services 中的安全性事件管理偵測和分析處理常式。
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
hideEdit: true
ms.openlocfilehash: 445d812b33214a3d2287268b587607004ef96ab7
ms.sourcegitcommit: 8bf2602d56eedee4447ddb374ef95b0587f254e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53377350"
---
# <a name="microsoft-security-incident-management-detection-and-analysis"></a><span data-ttu-id="ac8cf-103">Microsoft 安全性事件管理：偵測和分析</span><span class="sxs-lookup"><span data-stu-id="ac8cf-103">Microsoft security incident management: Detection and analysis</span></span>

<span data-ttu-id="ac8cf-104">為了偵測惡意活動，Microsoft 的每一項線上服務都會集中記錄安全性事件及其他資料，並執行各種分析技術，以找出反常或可疑的活動。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-104">To detect malicious activity, each of Microsoft's online services centrally logs security events and other data and perform various analytical techniques to find anomalous or suspicious activity.</span></span> <span data-ttu-id="ac8cf-105">記錄檔是透過 Microsoft online services 伺服器和基礎結構裝置收集，並儲存在中央和整合資料庫中。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-105">Log files are collected from Microsoft online services servers and infrastructure devices and stored in central and consolidated databases.</span></span>

<span data-ttu-id="ac8cf-106">Microsoft 採取以風險為基礎的方法來偵測惡意活動。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-106">Microsoft takes a risk-based approach to detecting malicious activity.</span></span> <span data-ttu-id="ac8cf-107">我們使用事件資料和威脅情報來定義偵測並設定其優先順序。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-107">We use incident data and threat intelligence to define and prioritize our detections.</span></span>

<span data-ttu-id="ac8cf-108">使用具有極高經驗、熟練、熟練之人員的團隊是偵測和分析階段成功的最重要的分項之一。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-108">Employing a team of highly experienced, proficient, and skilled people is one of the most important pillars to success in the detection and analysis phase.</span></span> <span data-ttu-id="ac8cf-109">Microsoft 使用多個服務小組，其中包含具有所有元件之能力的員工，包括在堆疊內的所有元件上，包括網路、路由器、防火牆、負載平衡器、作業系統和應用程式。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-109">Microsoft employs multiple service teams that include employees with competencies on all components within the stack, including the network, routers, firewalls, load balancers, operating systems, and applications.</span></span>

<span data-ttu-id="ac8cf-110">Microsoft online services 中的安全性偵測機制也包含不同來源所啟動的通知和警示。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-110">The security detection mechanisms in Microsoft online services also include notifications and alerts that are initiated by different sources.</span></span> <span data-ttu-id="ac8cf-111">Microsoft 線上服務安全性回應小組是安全性事件升級程式的主要 orchestrators。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-111">Microsoft online services security response teams are the key orchestrators of the security incident escalation process.</span></span> <span data-ttu-id="ac8cf-112">這些小組會接收所有升級，並負責分析和確認安全性事件的有效性。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-112">These teams receive all escalations and are responsible for analyzing and confirming the validity of the security incident.</span></span>

![安全性事件管理工作流程](../media/assurance-sim-workflow.png)

<span data-ttu-id="ac8cf-114">偵測的其中一個主要主要專案是通知：</span><span class="sxs-lookup"><span data-stu-id="ac8cf-114">One of the primary pillars of detection is notification:</span></span>

- <span data-ttu-id="ac8cf-115">每個服務小組負責根據線上服務安全性小組的需求，記錄服務中的任何動作或事件。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-115">Each service team is responsible to log any action or event inside the service based on the requirements from the online service security team.</span></span> <span data-ttu-id="ac8cf-116">由不同服務小組所建立的所有記錄，都是由安全性資訊和事件管理 (SIEM) 解決方案搭配預先定義的安全性和偵測規則處理。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-116">All logs created by the different service teams are processed by a Security Information and Event Management (SIEM) solution with predefined security and detection rules.</span></span> <span data-ttu-id="ac8cf-117">這些規則會根據安全性小組的建議演變，針對先前的安全性事件所獲知的資訊，判斷是否有任何可疑或惡意的活動。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-117">These rules evolve based on security team recommendations, on information learned from previous security incidents, to determine if there is any suspicious or malicious activity.</span></span>
- <span data-ttu-id="ac8cf-118">如果客戶決定安全性事件正在進行中，則他們可能會開啟 Microsoft 的支援案例，該支援案例會指派給 Microsoft 通訊小組，並將其轉換為所有適當的小組。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-118">If a customer determines that a security incident is underway, they may open a support case with Microsoft, which is assigned to the Microsoft communications team and turned into an escalation to all appropriate teams.</span></span>

<span data-ttu-id="ac8cf-119">Azure、Dynamics 365 及 Microsoft 365 服務小組也會使用透過安全性監控和登入在趨勢分析中取得的情報，以偵測可能表示攻擊或安全性事件的 Microsoft 線上服務資訊系統中的 abnormalities。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-119">Azure, Dynamics 365, and Microsoft 365 service teams also use the intelligence gained in trend analysis through security monitoring and logging to detect abnormalities in Microsoft online services information systems that might indicate an attack or a security incident.</span></span> <span data-ttu-id="ac8cf-120">在實際執行環境中，Microsoft 線上服務系統會將這些記錄的輸出匯總到集中式記錄伺服器。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-120">Microsoft online services systems aggregate output from these logs in the production environment into centralized logging servers.</span></span> <span data-ttu-id="ac8cf-121">在這些集中式記錄伺服器中，會在整個實際執行環境中檢查記錄的位置趨勢。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-121">From these centralized logging servers, logs are examined to spot trends throughout the production environment.</span></span> <span data-ttu-id="ac8cf-122">集中式伺服器中匯總的資料會安全地傳送至記錄服務，以進行高級查詢、儀表板建立及偵測反常和惡意活動。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-122">Data aggregated in the centralized servers are securely transmitted into a logging service for advanced querying, dashboard building and detecting anomalous and malicious activity.</span></span> <span data-ttu-id="ac8cf-123">服務也會使用機器學習來偵測記錄輸出的異常情況。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-123">The service also uses machine learning to detect anomalies with log output.</span></span>

<span data-ttu-id="ac8cf-124">在升級期間內，根據安全性事件的性質，安全性回應小組可能會與 Microsoft 的不同小組的一或多個主題專家打交道：</span><span class="sxs-lookup"><span data-stu-id="ac8cf-124">During the escalation phase and depending on the nature of the security incident, security response teams may engage one or more subject matter experts from various teams at Microsoft:</span></span>

- <span data-ttu-id="ac8cf-125">線上服務安全性與合規性小組</span><span class="sxs-lookup"><span data-stu-id="ac8cf-125">Online Services Security and Compliance team</span></span>
- <span data-ttu-id="ac8cf-126">Microsoft 威脅情報中心 (MSTIC) </span><span class="sxs-lookup"><span data-stu-id="ac8cf-126">Microsoft Threat Intelligence Center (MSTIC)</span></span>
- <span data-ttu-id="ac8cf-127">Microsoft 安全性回應中心 (MSRC) </span><span class="sxs-lookup"><span data-stu-id="ac8cf-127">Microsoft Security Response Center (MSRC)</span></span>
- <span data-ttu-id="ac8cf-128">公司、外部及法律事務 (CELA) </span><span class="sxs-lookup"><span data-stu-id="ac8cf-128">Corporate, External, and Legal Affairs (CELA)</span></span>
- <span data-ttu-id="ac8cf-129">Azure 安全性</span><span class="sxs-lookup"><span data-stu-id="ac8cf-129">Azure Security</span></span>
- <span data-ttu-id="ac8cf-130">Microsoft 365 工程及其他。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-130">Microsoft 365 engineering, and others.</span></span>

<span data-ttu-id="ac8cf-131">在升級任何安全性回應小組之前，服務小組負責根據定義的準則決定及設定安全性事件的嚴重性層級，例如：</span><span class="sxs-lookup"><span data-stu-id="ac8cf-131">Before an escalation to any security response team occurs, the service team is responsible for determining and setting the severity level of the security incident based on defined criteria such as:</span></span>

- <span data-ttu-id="ac8cf-132">隱私權</span><span class="sxs-lookup"><span data-stu-id="ac8cf-132">Privacy</span></span>
- <span data-ttu-id="ac8cf-133">影響</span><span class="sxs-lookup"><span data-stu-id="ac8cf-133">Impact</span></span>
- <span data-ttu-id="ac8cf-134">範圍</span><span class="sxs-lookup"><span data-stu-id="ac8cf-134">Scope</span></span>
- <span data-ttu-id="ac8cf-135">受影響的承租人數目</span><span class="sxs-lookup"><span data-stu-id="ac8cf-135">Number of affected tenants</span></span>
- <span data-ttu-id="ac8cf-136">區域</span><span class="sxs-lookup"><span data-stu-id="ac8cf-136">Region</span></span>
- <span data-ttu-id="ac8cf-137">服務</span><span class="sxs-lookup"><span data-stu-id="ac8cf-137">Service</span></span>
- <span data-ttu-id="ac8cf-138">事件的詳細資料</span><span class="sxs-lookup"><span data-stu-id="ac8cf-138">Details of the incident</span></span>
- <span data-ttu-id="ac8cf-139">特定客戶行業或市場規定。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-139">Specific customer industry or market regulations.</span></span>

<span data-ttu-id="ac8cf-140">事件優先順序取決於使用不同的因素，包括但不限於事件的功能影響、事件的資訊影響，以及事件的可復原性。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-140">Incident prioritization is determined by using distinct factors, including but not limited to the functional impact of the incident, the informational impact of the incident, and the recoverability from the incident.</span></span>

<span data-ttu-id="ac8cf-141">在收到有關安全性事件的上報後，安全性小組會將虛擬小組組織 (v 小組) 由 Microsoft online 服務安全性回應小組、服務小組和事件通訊小組成員組成。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-141">After receiving an escalation about a security incident, the security team organizes a virtual team (v-team) comprised of members from the Microsoft online service security response team, service teams, and the incident communication team.</span></span> <span data-ttu-id="ac8cf-142">然後，v 小組必須確認安全性事件的合法性，並消除任何誤報。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-142">The v-team must then confirm the legitimacy of the security incident and eliminate any false positives.</span></span> <span data-ttu-id="ac8cf-143">在準備階段確定的指示器所提供資訊的準確性是很重要的。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-143">The accuracy of information provided by the indicators determined during the preparation phase is critical.</span></span> <span data-ttu-id="ac8cf-144">透過依向量攻擊類別來分析此資訊，「五團隊」可以判斷安全性事件是否為合理考慮。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-144">By analyzing this information by category of vector attack, the v-team can determine if the security incident is a legitimate concern.</span></span>

<span data-ttu-id="ac8cf-145">在調查開始時，安全性事件回應小組會依照案例管理原則記錄事件的所有相關資訊。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-145">At the beginning of the investigation, the security incident response team records all information about the incident according to our case management policies.</span></span> <span data-ttu-id="ac8cf-146">隨著案例的進展，我們追蹤進行中的動作，並遵循證據處理標準，以在整個事件週期內收集、保留及保護此資料。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-146">As the case progresses, we track ongoing actions and follow evidence handling standards for gathering, retaining, and securing this data throughout the incident lifecycle.</span></span>

<span data-ttu-id="ac8cf-147">這些動作的一些範例包括：</span><span class="sxs-lookup"><span data-stu-id="ac8cf-147">Some examples of these actions would include:</span></span>

- <span data-ttu-id="ac8cf-148">摘要，這是事件及其潛在影響的簡短描述</span><span class="sxs-lookup"><span data-stu-id="ac8cf-148">A summary, which is a brief description of the incident and its potential impact</span></span>
- <span data-ttu-id="ac8cf-149">事件的嚴重性和優先順序，它們是透過評估潛在影響來衍生</span><span class="sxs-lookup"><span data-stu-id="ac8cf-149">The incident's severity and priority, which are derived by assessing the potential impact</span></span>
- <span data-ttu-id="ac8cf-150">所有識別出導致事件發生的標記的清單</span><span class="sxs-lookup"><span data-stu-id="ac8cf-150">A list of all indicators identified which led to detection of the incident</span></span>
- <span data-ttu-id="ac8cf-151">任何相關事件的清單</span><span class="sxs-lookup"><span data-stu-id="ac8cf-151">A list of any related incidents</span></span>
- <span data-ttu-id="ac8cf-152">由 v 小組採取的所有動作清單</span><span class="sxs-lookup"><span data-stu-id="ac8cf-152">A list of all actions taken by the v-team</span></span>
- <span data-ttu-id="ac8cf-153">任何收集的證據，也會保留以供檢討後分析和未來的鑒證調查。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-153">Any gathered evidence, which will also be preserved for post-mortem analysis and future forensic investigations</span></span>
- <span data-ttu-id="ac8cf-154">建議的後續步驟和動作</span><span class="sxs-lookup"><span data-stu-id="ac8cf-154">Recommended next steps and actions</span></span>

<span data-ttu-id="ac8cf-155">在安全性事件確認之後，安全性回應小組和適當服務小組的主要目標是包含攻擊、保護服務 () 受到攻擊，以及避免全域影響較大。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-155">After security incident confirmation, the primary goals of the security response team and the appropriate service team are to contain the attack, to protect the service(s) under attack, and to avoid a greater global impact.</span></span> <span data-ttu-id="ac8cf-156">在同一時間，適當的工程小組會運作，以判斷根本原因，並準備第一個復原計畫。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-156">At the same time, the appropriate engineering teams work to determine the root cause and to prepare the first recovery plan.</span></span>

<span data-ttu-id="ac8cf-157">在下一個階段中，安全性回應小組會識別由安全性事件（如果有的話）所影響的客戶 (s) 。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-157">In the next phase, the security response team identifies the customer(s) affected by the security incident, if any.</span></span> <span data-ttu-id="ac8cf-158">影響範圍可能需要一些時間，以根據地區、資料中心、服務、伺服器陣列、伺服器等來判斷。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-158">The scope of effect can take some time to determine, based on region, datacenter, service, server farm, server, and so forth.</span></span> <span data-ttu-id="ac8cf-159">受影響客戶的清單是由服務小組和對應的 Microsoft 通訊小組所編譯，然後負責處理合約和合規性義務中的客戶通知程式。</span><span class="sxs-lookup"><span data-stu-id="ac8cf-159">The list of affected customers is compiled by the service team and the corresponding Microsoft communications team, who then handle the customer notification process within contractual and compliance obligations.</span></span>

## <a name="related-articles"></a><span data-ttu-id="ac8cf-160">相關文章</span><span class="sxs-lookup"><span data-stu-id="ac8cf-160">Related articles</span></span>

- [<span data-ttu-id="ac8cf-161">Microsoft 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="ac8cf-161">Microsoft security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="ac8cf-162">Microsoft 安全性事件管理：準備</span><span class="sxs-lookup"><span data-stu-id="ac8cf-162">Microsoft security incident management: Preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="ac8cf-163">Microsoft 安全性事件管理：包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="ac8cf-163">Microsoft security incident management: Containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
- [<span data-ttu-id="ac8cf-164">Microsoft 安全性事件管理：事件後活動</span><span class="sxs-lookup"><span data-stu-id="ac8cf-164">Microsoft security incident management: Post-incident activity</span></span>](assurance-sim-post-incident-activity.md)
- [<span data-ttu-id="ac8cf-165">如何記錄安全性事件支援票證</span><span class="sxs-lookup"><span data-stu-id="ac8cf-165">How to Log a Security Event Support Ticket</span></span>](/azure/security/fundamentals/event-support-ticket)
- [<span data-ttu-id="ac8cf-166">GDPR 規定的 Azure 和 Dynamics 365 外洩通知</span><span class="sxs-lookup"><span data-stu-id="ac8cf-166">Azure and Dynamics 365 breach notification under the GDPR</span></span>](/compliance/regulatory/gdpr-breach-azure-dynamics)
