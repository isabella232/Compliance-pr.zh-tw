---
title: Microsoft 安全性事件管理：事件後活動
description: 本文提供 Microsoft online services 中的安全性事件管理後續事件處理常式的概述。
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
ms.openlocfilehash: 965c7d6d0d469b9eea981252805bda598c92a4c8
ms.sourcegitcommit: 8bf2602d56eedee4447ddb374ef95b0587f254e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53377530"
---
# <a name="microsoft-security-incident-management-post-incident-activity"></a><span data-ttu-id="3e4be-103">Microsoft 安全性事件管理：事件後活動</span><span class="sxs-lookup"><span data-stu-id="3e4be-103">Microsoft security incident management: Post-incident activity</span></span>

## <a name="postmortem"></a><span data-ttu-id="3e4be-104">死後</span><span class="sxs-lookup"><span data-stu-id="3e4be-104">Postmortem</span></span>

<span data-ttu-id="3e4be-105">有些安全性事件，尤其是客戶影響或導致資料破壞的事件，會發生完整的事件總結。</span><span class="sxs-lookup"><span data-stu-id="3e4be-105">Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem.</span></span> <span data-ttu-id="3e4be-106">安全性回應小組會針對安全性事件回應中的所有協力廠商，進行詳細總結：</span><span class="sxs-lookup"><span data-stu-id="3e4be-106">The security response team conducts a detailed postmortem with all the parties involved in security incident response to:</span></span>

- <span data-ttu-id="3e4be-107">記錄導致事件發生的事件順序。</span><span class="sxs-lookup"><span data-stu-id="3e4be-107">Document the sequence of events that caused the incident.</span></span>
- <span data-ttu-id="3e4be-108">如已知) 所述，以包含違反違犯 (的演員所支援的證據，建立事件的技術摘要。</span><span class="sxs-lookup"><span data-stu-id="3e4be-108">Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known).</span></span> <span data-ttu-id="3e4be-109">這項摘要會包含回應的執行方式和其他重要優點。</span><span class="sxs-lookup"><span data-stu-id="3e4be-109">This summary will include how the response was executed and other key takeaways.</span></span>
- <span data-ttu-id="3e4be-110">識別在安全性事件回應期間識別的技術停機、程式失敗、手動錯誤、程式缺陷和通訊不足，以及/或任何先前未知的攻擊媒介。</span><span class="sxs-lookup"><span data-stu-id="3e4be-110">Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.</span></span>

<span data-ttu-id="3e4be-111">事後，您可以在 Microsoft online services 工程開發週期中設定新的優先順序，以直接影響 Microsoft 線上服務的改進、操作過程及檔。</span><span class="sxs-lookup"><span data-stu-id="3e4be-111">The postmortem will directly influence Microsoft online service improvement, operational processes, and documentation by setting new priorities in the Microsoft online services engineering development cycle.</span></span>

## <a name="documentation"></a><span data-ttu-id="3e4be-112">文件</span><span class="sxs-lookup"><span data-stu-id="3e4be-112">Documentation</span></span>

<span data-ttu-id="3e4be-113">事後過程中的所有重要技術調查都會以錯誤或開發變更要求的形式，于報表和服務投資或修復中取得。</span><span class="sxs-lookup"><span data-stu-id="3e4be-113">All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests.</span></span> <span data-ttu-id="3e4be-114">這些結果會遵循適當的工程團隊。</span><span class="sxs-lookup"><span data-stu-id="3e4be-114">These findings are followed-up with the appropriate engineering teams.</span></span> <span data-ttu-id="3e4be-115">針對流程失敗及跨組織的問題，問題會記錄在安全性回應小組的資料庫中，並遵循適當的群組來處理這些問題。</span><span class="sxs-lookup"><span data-stu-id="3e4be-115">For process failures and cross-organizational issues, issues are documented in the security response team's database and followed-up with the appropriate groups to address them.</span></span>

## <a name="process-improvement"></a><span data-ttu-id="3e4be-116">進程改進</span><span class="sxs-lookup"><span data-stu-id="3e4be-116">Process improvement</span></span>

<span data-ttu-id="3e4be-117">在 Microsoft online services 中回應安全性事件，涉及與跨 Microsoft 不同組織的多個群組進行協調，以及可能的適當外部組織，例如法律強制執行。</span><span class="sxs-lookup"><span data-stu-id="3e4be-117">Responding to a security incident in Microsoft online services involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement.</span></span> <span data-ttu-id="3e4be-118">我們知道，在每個安全性事件（sufficiency 及完整性）之後，評估我們的回應是很重要的。</span><span class="sxs-lookup"><span data-stu-id="3e4be-118">We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness.</span></span> <span data-ttu-id="3e4be-119">針對任何已識別的改善或變更，安全性回應小組會評估與適當小組和專案關係人進行諮詢的建議，並在適當的情況下將其融入標準運作程式中。</span><span class="sxs-lookup"><span data-stu-id="3e4be-119">For any identified improvements or changes, the security response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures.</span></span> <span data-ttu-id="3e4be-120">在安全性事件回應或事後活動中所識別的所有必要變更、缺陷或服務改進都會在內部的 Microsoft 工程資料庫中記錄及追蹤。</span><span class="sxs-lookup"><span data-stu-id="3e4be-120">All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft engineering database.</span></span> <span data-ttu-id="3e4be-121">所有潛在的錯誤或功能會指派給適當的擁有者。</span><span class="sxs-lookup"><span data-stu-id="3e4be-121">All potential bugs or features are assigned to the appropriate owner.</span></span> <span data-ttu-id="3e4be-122">Microsoft 安全性回應小組會檢查所有專案，直到問題解決為止。</span><span class="sxs-lookup"><span data-stu-id="3e4be-122">The Microsoft security response team reviews all entries until the issue is resolved.</span></span>

## <a name="related-articles"></a><span data-ttu-id="3e4be-123">相關文章</span><span class="sxs-lookup"><span data-stu-id="3e4be-123">Related articles</span></span>

- [<span data-ttu-id="3e4be-124">Microsoft 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="3e4be-124">Microsoft security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="3e4be-125">Microsoft 安全性事件管理：準備</span><span class="sxs-lookup"><span data-stu-id="3e4be-125">Microsoft security incident management: Preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="3e4be-126">Microsoft 安全性事件管理：偵測和分析</span><span class="sxs-lookup"><span data-stu-id="3e4be-126">Microsoft security incident management: Detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="3e4be-127">Microsoft 安全性事件管理：包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="3e4be-127">Microsoft security incident management: Containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
- [<span data-ttu-id="3e4be-128">如何記錄安全性事件支援票證</span><span class="sxs-lookup"><span data-stu-id="3e4be-128">How to Log a Security Event Support Ticket</span></span>](/azure/security/fundamentals/event-support-ticket)
- [<span data-ttu-id="3e4be-129">GDPR 規定的 Azure 和 Dynamics 365 外洩通知</span><span class="sxs-lookup"><span data-stu-id="3e4be-129">Azure and Dynamics 365 breach notification under the GDPR</span></span>](/compliance/regulatory/gdpr-breach-azure-dynamics)
