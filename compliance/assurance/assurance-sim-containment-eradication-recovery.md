---
title: Microsoft 365 安全性事件管理：包容、eradication 及恢復
description: 本文概要說明 Microsoft 365 中的安全性事件管理包容、eradication 及復原程式。
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
ms.openlocfilehash: 702735ed2ba35a4f3b0a02123f0c58b5fb4d397e
ms.sourcegitcommit: d67e4d4fdc664f1da450c8ef2f6732e19bdd403a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037586"
---
# <a name="microsoft-365-security-incident-management-containment-eradication-and-recovery"></a><span data-ttu-id="46732-103">Microsoft 365 安全性事件管理：包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="46732-103">Microsoft 365 security incident management: Containment, eradication, and recovery</span></span>

<span data-ttu-id="46732-104">根據 Microsoft 365 安全性回應小組、服務小組和其他人員所執行的分析，開發適當的包容和復原計畫，以盡可能降低安全性事件的影響。</span><span class="sxs-lookup"><span data-stu-id="46732-104">Based on the analysis performed by the Microsoft 365 Security Response team, the service team, and others, an appropriate containment and recovery plan is developed to minimize the effect of the security incident.</span></span> <span data-ttu-id="46732-105">適當的服務小組接著會從 Microsoft 365 安全回應小組的支援，套用生產方案。</span><span class="sxs-lookup"><span data-stu-id="46732-105">The appropriate service teams then apply that plan in production with support from the Microsoft 365 Security Response team.</span></span>

## <a name="containment"></a><span data-ttu-id="46732-106">遏制</span><span class="sxs-lookup"><span data-stu-id="46732-106">Containment</span></span>

<span data-ttu-id="46732-107">在偵測到安全性事件後，必須先包含入侵，才可存取更多資源或造成更大的損毀。</span><span class="sxs-lookup"><span data-stu-id="46732-107">After detecting a security incident, it is important to contain the intrusion before the adversary can access more resources or cause more damage.</span></span> <span data-ttu-id="46732-108">我們的安全性事件回應程式的主要目標是限制對客戶或其資料的影響，或是對 Microsoft 系統、服務和應用程式的影響。</span><span class="sxs-lookup"><span data-stu-id="46732-108">The primary goal of our security incident response procedures is to limit impact to customers or their data, or to Microsoft systems, services, and applications.</span></span>

## <a name="eradication"></a><span data-ttu-id="46732-109">根除</span><span class="sxs-lookup"><span data-stu-id="46732-109">Eradication</span></span>

<span data-ttu-id="46732-110">Eradication 是以高信心程度消除安全性事件根本原因的處理常式。</span><span class="sxs-lookup"><span data-stu-id="46732-110">Eradication is the process of eliminating the root cause of the security incident with a high degree of confidence.</span></span> <span data-ttu-id="46732-111">目標是兩折的：</span><span class="sxs-lookup"><span data-stu-id="46732-111">The goal is two-fold:</span></span>

- <span data-ttu-id="46732-112">完全從環境逐出對手</span><span class="sxs-lookup"><span data-stu-id="46732-112">to evict the adversary completely from the environment</span></span>
- <span data-ttu-id="46732-113">若要緩解此弱點 (請注意，) 如果已啟用或可能讓敵人重新輸入環境。</span><span class="sxs-lookup"><span data-stu-id="46732-113">to mitigate the vulnerability (if known) that enabled or could enable the adversary to reenter the environment.</span></span>

<span data-ttu-id="46732-114">根據事件性質、安全性事件範圍、滲透程度與可能影響程度的深度，Microsoft 365 安全性回應小組會建議服務小組採用 eradication 技巧。</span><span class="sxs-lookup"><span data-stu-id="46732-114">Depending on the nature of the incident, the scope of the security incident, the depth of the penetration and possible repercussions, the Microsoft 365 Security Response team will recommend that service teams adopt eradication techniques.</span></span> <span data-ttu-id="46732-115">考慮到可能由這些 eradication 步驟造成的潛在業務影響，當必要時) ，服務小組和 Microsoft 365 安全性回應小組會進行必要的分析和核准，以 (必要事項。</span><span class="sxs-lookup"><span data-stu-id="46732-115">Considering the potential business impact that may be caused by these eradication steps, these decisions will be made by service teams and the Microsoft 365 Security Response team after a detailed analysis and approval from the Executive Incident Manager (if necessary).</span></span>

## <a name="recovery"></a><span data-ttu-id="46732-116">恢復</span><span class="sxs-lookup"><span data-stu-id="46732-116">Recovery</span></span>

<span data-ttu-id="46732-117">隨著回應小組獲得合理的信賴程度，讓敵人從環境逐出，而且已消除所有已知可靠的路徑，個別的服務小組會啟動還原步驟，以將服務帶入已知且良好的設定。</span><span class="sxs-lookup"><span data-stu-id="46732-117">As the response team gains a reasonable level of confidence that the adversary has been evicted from the environment and all known vulnerable paths have been eliminated, the individual service teams, will initiate restoration steps to bring the service to a known and good configuration.</span></span> <span data-ttu-id="46732-118">這些還原步驟將會與 Microsoft 365 安全性回應小組進行諮詢。</span><span class="sxs-lookup"><span data-stu-id="46732-118">These restoration steps will be in consultation with the Microsoft 365 Security Response team.</span></span> <span data-ttu-id="46732-119">此活動包含識別服務的最後一個已知良好狀態，從備份還原至此狀態，檢查還原的狀態中有漏洞的攻擊路徑等等。Microsoft 365 安全性回應小組（諮詢服務小組）將會決定環境可能的最佳復原計畫。</span><span class="sxs-lookup"><span data-stu-id="46732-119">This activity includes identifying the last known good state of the service, restoring from backups to this state, inspecting vulnerable attack paths in the restored state, etc. The Microsoft 365 Security Response team, in consultation with the service teams, will determine the best possible recovery plan for the environment.</span></span>

<span data-ttu-id="46732-120">復原的一個重要方面是要有增強的 vigilance 和控制措施，以驗證復原計畫是否已順利執行，且環境中不存在遭到破壞的跡象。</span><span class="sxs-lookup"><span data-stu-id="46732-120">A key aspect to the recovery is to have enhanced vigilance and controls in place to validate that the recovery plan has been successfully executed, and that no signs of breach exist in the environment.</span></span>

## <a name="customer-notification-of-security-incident"></a><span data-ttu-id="46732-121">客戶安全性事件的通知</span><span class="sxs-lookup"><span data-stu-id="46732-121">Customer notification of security incident</span></span>

<span data-ttu-id="46732-122">如果 Microsoft 決定發生安全性事件，我們會以不需要的延遲，以及我們同意的合約和規範中的規定來通知您。</span><span class="sxs-lookup"><span data-stu-id="46732-122">If Microsoft determines that a security incident has occurred, we will notify you with undue delay, and within contractual and compliance requirements we have agreed to.</span></span> <span data-ttu-id="46732-123">在識別所有受影響的承租人之後，Microsoft 365 客戶經驗 (CxP) 通訊小組會運作，識別可能適用于受影響承租人的任何相關規章。</span><span class="sxs-lookup"><span data-stu-id="46732-123">After identifying all affected tenants, the Microsoft 365 Customer Experience (CxP) Communications team works to identify any relevant regulations that might apply to affected tenants.</span></span> <span data-ttu-id="46732-124">Microsoft 365 CxP 通訊小組使用適用的規章中所定義的適當通訊通道，以通知適當的承租人連絡人。</span><span class="sxs-lookup"><span data-stu-id="46732-124">The Microsoft 365 CxP Communications team uses the appropriate communication channel defined in applicable regulations to notify the appropriate tenant contact.</span></span>

<span data-ttu-id="46732-125">通知會包含有關該事件的詳細資訊，例如事件的描述、對客戶資料的影響、Microsoft 採取的動作，以及/或建議的動作，以供客戶用以解決問題並避免週期。</span><span class="sxs-lookup"><span data-stu-id="46732-125">Notification will include detailed information about the incident, such as a description of the incident, the effect on customer data, if any, actions taken by Microsoft, and/or suggested actions for customers to take to resolve the issue and prevent recurrence.</span></span> <span data-ttu-id="46732-126">通知將會傳遞給 Microsoft 365 租使用者的指定系統管理員 (s) 。</span><span class="sxs-lookup"><span data-stu-id="46732-126">Notification will be delivered to the designated administrator(s) of the Microsoft 365 tenant.</span></span> <span data-ttu-id="46732-127">為了確保收到通知，您應該確保您的系統管理員在其租使用者設定檔中提供及維護準確的連絡人資訊。</span><span class="sxs-lookup"><span data-stu-id="46732-127">To ensure notifications are received, you should ensure that your administrators provide and maintain accurate contact information in their tenant profiles.</span></span> <span data-ttu-id="46732-128">此外，視事件性質而定，客戶也可以透過 Microsoft 365 服務健康情況儀表板獲得通知[。](http://status.yammer.com/)</span><span class="sxs-lookup"><span data-stu-id="46732-128">In addition, depending on the nature of the incident, customers can also be notified via the Microsoft 365 Service Health Dashboard[.](http://status.yammer.com/)</span></span>

## <a name="related-articles"></a><span data-ttu-id="46732-129">相關文章</span><span class="sxs-lookup"><span data-stu-id="46732-129">Related articles</span></span>

- [<span data-ttu-id="46732-130">Microsoft 365 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="46732-130">Microsoft 365 security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="46732-131">Microsoft 365 的安全性事件管理準備</span><span class="sxs-lookup"><span data-stu-id="46732-131">Microsoft 365 security incident management preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="46732-132">Microsoft 365 安全性事件管理偵測和分析</span><span class="sxs-lookup"><span data-stu-id="46732-132">Microsoft 365 security incident management detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="46732-133">Microsoft 365 安全性事件管理後置事件活動</span><span class="sxs-lookup"><span data-stu-id="46732-133">Microsoft 365 security incident management post-incident activity</span></span>](assurance-sim-post-incident-activity.md)
