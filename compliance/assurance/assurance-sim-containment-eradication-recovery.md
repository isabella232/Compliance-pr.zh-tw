---
title: Microsoft 安全性事件管理：包容、eradication 及恢復
description: 本文概要說明 Microsoft online services 中的安全性事件管理包容、eradication 及復原程式。
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
ms.openlocfilehash: 95e52107df2f3e745d393c62929f7c169bcf9a33
ms.sourcegitcommit: 8bf2602d56eedee4447ddb374ef95b0587f254e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53377550"
---
# <a name="microsoft-security-incident-management-containment-eradication-and-recovery"></a><span data-ttu-id="48dce-103">Microsoft 安全性事件管理：包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="48dce-103">Microsoft security incident management: Containment, eradication, and recovery</span></span>

<span data-ttu-id="48dce-104">根據安全性回應小組、服務小組和其他人員所執行的分析，開發適當的包容和復原計畫，以盡可能降低安全性事件的影響。</span><span class="sxs-lookup"><span data-stu-id="48dce-104">Based on the analysis performed by the security response team, the service team, and others, an appropriate containment and recovery plan is developed to minimize the effect of the security incident.</span></span> <span data-ttu-id="48dce-105">然後，適當的服務小組會在生產環境中套用此方案，並提供來自安全性回應小組的支援。</span><span class="sxs-lookup"><span data-stu-id="48dce-105">The appropriate service teams then apply that plan in production with support from the security response team.</span></span>

## <a name="containment"></a><span data-ttu-id="48dce-106">遏制</span><span class="sxs-lookup"><span data-stu-id="48dce-106">Containment</span></span>

<span data-ttu-id="48dce-107">在偵測到安全性事件後，必須先包含入侵，才可存取更多資源或造成更大的損毀。</span><span class="sxs-lookup"><span data-stu-id="48dce-107">After detecting a security incident, it is important to contain the intrusion before the adversary can access more resources or cause more damage.</span></span> <span data-ttu-id="48dce-108">我們的安全性事件回應程式的主要目標是限制對客戶或其資料的影響，或是對 Microsoft 系統、服務和應用程式的影響。</span><span class="sxs-lookup"><span data-stu-id="48dce-108">The primary goal of our security incident response procedures is to limit impact to customers or their data, or to Microsoft systems, services, and applications.</span></span>

## <a name="eradication"></a><span data-ttu-id="48dce-109">根除</span><span class="sxs-lookup"><span data-stu-id="48dce-109">Eradication</span></span>

<span data-ttu-id="48dce-110">Eradication 是以高信心程度消除安全性事件根本原因的處理常式。</span><span class="sxs-lookup"><span data-stu-id="48dce-110">Eradication is the process of eliminating the root cause of the security incident with a high degree of confidence.</span></span> <span data-ttu-id="48dce-111">目標是兩折的：</span><span class="sxs-lookup"><span data-stu-id="48dce-111">The goal is two-fold:</span></span>

- <span data-ttu-id="48dce-112">完全從環境逐出對手</span><span class="sxs-lookup"><span data-stu-id="48dce-112">to evict the adversary completely from the environment</span></span>
- <span data-ttu-id="48dce-113">若要緩解此弱點 (請注意，) 如果已啟用或可能讓敵人重新輸入環境。</span><span class="sxs-lookup"><span data-stu-id="48dce-113">to mitigate the vulnerability (if known) that enabled or could enable the adversary to reenter the environment.</span></span>

<span data-ttu-id="48dce-114">根據事件性質、安全性事件範圍、滲透程度與可能影響程度的深度，安全性回應小組會建議服務小組採用 eradication 技巧。</span><span class="sxs-lookup"><span data-stu-id="48dce-114">Depending on the nature of the incident, the scope of the security incident, the depth of the penetration and possible repercussions, the security response team will recommend that service teams adopt eradication techniques.</span></span> <span data-ttu-id="48dce-115">考慮到此 eradication 步驟可能導致的潛在業務影響，當必要時) ，服務小組和安全性回應小組會進行必要的分析和核准，以 (。</span><span class="sxs-lookup"><span data-stu-id="48dce-115">Considering the potential business impact that may be caused by these eradication steps, these decisions will be made by service teams and the security response team after a detailed analysis and approval from the Executive Incident Manager (if necessary).</span></span>

## <a name="recovery"></a><span data-ttu-id="48dce-116">恢復</span><span class="sxs-lookup"><span data-stu-id="48dce-116">Recovery</span></span>

<span data-ttu-id="48dce-117">隨著回應小組獲得合理的信賴程度，讓敵人從環境逐出，而且已消除所有已知可靠的路徑，個別的服務小組會啟動還原步驟，以將服務帶入已知且良好的設定。</span><span class="sxs-lookup"><span data-stu-id="48dce-117">As the response team gains a reasonable level of confidence that the adversary has been evicted from the environment and all known vulnerable paths have been eliminated, the individual service teams, will initiate restoration steps to bring the service to a known and good configuration.</span></span> <span data-ttu-id="48dce-118">這些還原步驟將會與安全性回應小組進行諮詢。</span><span class="sxs-lookup"><span data-stu-id="48dce-118">These restoration steps will be in consultation with the security response team.</span></span> <span data-ttu-id="48dce-119">此活動包含識別服務的最後一個已知良好狀態，從備份還原至此狀態，檢查還原的狀態中有漏洞的攻擊路徑等等。與服務小組互動的安全性回應小組會決定環境可能的最佳復原計畫。</span><span class="sxs-lookup"><span data-stu-id="48dce-119">This activity includes identifying the last known good state of the service, restoring from backups to this state, inspecting vulnerable attack paths in the restored state, etc. The security response team, in consultation with the service teams, will determine the best possible recovery plan for the environment.</span></span>

<span data-ttu-id="48dce-120">復原的一個重要方面是要有增強的 vigilance 和控制措施，以驗證復原計畫是否已順利執行，且環境中不存在遭到破壞的跡象。</span><span class="sxs-lookup"><span data-stu-id="48dce-120">A key aspect to the recovery is to have enhanced vigilance and controls in place to validate that the recovery plan has been successfully executed, and that no signs of breach exist in the environment.</span></span>

## <a name="customer-notification-of-security-incident"></a><span data-ttu-id="48dce-121">客戶安全性事件的通知</span><span class="sxs-lookup"><span data-stu-id="48dce-121">Customer notification of security incident</span></span>

<span data-ttu-id="48dce-122">如果 Microsoft 決定發生安全性事件，我們會以不需要的延遲，以及我們同意的合約和規範中的規定來通知您。</span><span class="sxs-lookup"><span data-stu-id="48dce-122">If Microsoft determines that a security incident has occurred, we will notify you with undue delay, and within contractual and compliance requirements we have agreed to.</span></span> <span data-ttu-id="48dce-123">在識別所有受影響的承租人之後，對應的通訊小組會運作，識別可能適用于受影響承租人的任何相關規章。</span><span class="sxs-lookup"><span data-stu-id="48dce-123">After identifying all affected tenants, the corresponding communications team works to identify any relevant regulations that might apply to affected tenants.</span></span> <span data-ttu-id="48dce-124">通訊小組使用適用的規章中所定義的適當通訊通道，以通知適當的承租人連絡人。</span><span class="sxs-lookup"><span data-stu-id="48dce-124">The communications team uses the appropriate communication channel defined in applicable regulations to notify the appropriate tenant contact.</span></span>

<span data-ttu-id="48dce-125">通知會包含有關該事件的詳細資訊，例如事件的描述、對客戶資料的影響、Microsoft 採取的動作，以及/或建議的動作，以供客戶用以解決問題並避免週期。</span><span class="sxs-lookup"><span data-stu-id="48dce-125">Notification will include detailed information about the incident, such as a description of the incident, the effect on customer data, if any, actions taken by Microsoft, and/or suggested actions for customers to take to resolve the issue and prevent recurrence.</span></span> <span data-ttu-id="48dce-126">通知將會傳送至 Microsoft online services 租使用者的指定系統管理員 (s) 。</span><span class="sxs-lookup"><span data-stu-id="48dce-126">Notification will be delivered to the designated administrator(s) of the Microsoft online services tenant.</span></span> <span data-ttu-id="48dce-127">為了確保收到通知，您應該確保您的系統管理員在其租使用者設定檔中提供及維護準確的連絡人資訊。</span><span class="sxs-lookup"><span data-stu-id="48dce-127">To ensure notifications are received, you should ensure that your administrators provide and maintain accurate contact information in their tenant profiles.</span></span> <span data-ttu-id="48dce-128">此外，視事件性質而定，也可以透過[Microsoft 365 服務健康情況儀表板](http://status.yammer.com/)通知 Microsoft 365 的客戶。</span><span class="sxs-lookup"><span data-stu-id="48dce-128">In addition, depending on the nature of the incident, Microsoft 365 customers can also be notified via the [Microsoft 365 Service Health Dashboard](http://status.yammer.com/).</span></span>

## <a name="related-articles"></a><span data-ttu-id="48dce-129">相關文章</span><span class="sxs-lookup"><span data-stu-id="48dce-129">Related articles</span></span>

- [<span data-ttu-id="48dce-130">Microsoft 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="48dce-130">Microsoft security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="48dce-131">Microsoft 安全性事件管理：準備</span><span class="sxs-lookup"><span data-stu-id="48dce-131">Microsoft security incident management: Preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="48dce-132">Microsoft 安全性事件管理：偵測和分析</span><span class="sxs-lookup"><span data-stu-id="48dce-132">Microsoft security incident management: Detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="48dce-133">Microsoft 安全性事件管理：事件後活動</span><span class="sxs-lookup"><span data-stu-id="48dce-133">Microsoft security incident management: Post-incident activity</span></span>](assurance-sim-post-incident-activity.md)
- [<span data-ttu-id="48dce-134">如何記錄安全性事件支援票證</span><span class="sxs-lookup"><span data-stu-id="48dce-134">How to Log a Security Event Support Ticket</span></span>](/azure/security/fundamentals/event-support-ticket)
- [<span data-ttu-id="48dce-135">GDPR 規定的 Azure 和 Dynamics 365 外洩通知</span><span class="sxs-lookup"><span data-stu-id="48dce-135">Azure and Dynamics 365 breach notification under the GDPR</span></span>](/compliance/regulatory/gdpr-breach-azure-dynamics)
