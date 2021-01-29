---
title: Microsoft 365 安全性事件管理：事件後活動
description: 本文概要說明 Microsoft 365 中的安全性事件管理後續事件處理常式。
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
ms.openlocfilehash: 66c25503ac574de512f5201981112a0e54714968
ms.sourcegitcommit: 2973d25e9e0185b84d281f963553a332eac1c1a3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50040346"
---
# <a name="microsoft-365-security-incident-management-post-incident-activity"></a><span data-ttu-id="a07e1-103">Microsoft 365 安全性事件管理：事件後活動</span><span class="sxs-lookup"><span data-stu-id="a07e1-103">Microsoft 365 security incident management: Post-incident activity</span></span>

## <a name="postmortem"></a><span data-ttu-id="a07e1-104">死後</span><span class="sxs-lookup"><span data-stu-id="a07e1-104">Postmortem</span></span>

<span data-ttu-id="a07e1-105">有些安全性事件，尤其是客戶影響或導致資料破壞的事件，會發生完整的事件總結。</span><span class="sxs-lookup"><span data-stu-id="a07e1-105">Some security incidents, especially those incidents that are customer impacting or result in a data breach, are subject to a full incident postmortem.</span></span> <span data-ttu-id="a07e1-106">Microsoft 365 安全性回應小組會針對安全性事件回應中的所有協力廠商，進行詳細總結：</span><span class="sxs-lookup"><span data-stu-id="a07e1-106">The Microsoft 365 Security Response team conducts a detailed postmortem with all the parties involved in security incident response to:</span></span>

- <span data-ttu-id="a07e1-107">記錄導致事件發生的事件順序</span><span class="sxs-lookup"><span data-stu-id="a07e1-107">Document the sequence of events that caused the incident</span></span>
- <span data-ttu-id="a07e1-108">如已知) 所述，以包含違反違犯 (的演員所支援的證據，建立事件的技術摘要。</span><span class="sxs-lookup"><span data-stu-id="a07e1-108">Create a technical summary of the incident as supported by the evidence that includes the actors involved in the breach (if known).</span></span> <span data-ttu-id="a07e1-109">這項摘要會包含回應的執行方式和其他重要優點。</span><span class="sxs-lookup"><span data-stu-id="a07e1-109">This summary will include how the response was executed and other key takeaways.</span></span>
- <span data-ttu-id="a07e1-110">識別在安全性事件回應期間識別的技術停機、程式失敗、手動錯誤、程式缺陷和通訊不足，以及/或任何先前未知的攻擊媒介。</span><span class="sxs-lookup"><span data-stu-id="a07e1-110">Identify technical lapses, procedural failures, manual errors, process flaws, and communication glitches, and/or any previously unknown attack vectors that were identified during the security incident response.</span></span>

<span data-ttu-id="a07e1-111">事後，您可以在 Microsoft 365 工程開發週期中設定新的優先順序，以直接影響 Microsoft 365 服務的改進、操作程式及檔。</span><span class="sxs-lookup"><span data-stu-id="a07e1-111">The postmortem will directly influence Microsoft 365 service improvement, operational processes, and documentation by setting new priorities in the Microsoft 365 engineering development cycle.</span></span>

## <a name="documentation"></a><span data-ttu-id="a07e1-112">文件</span><span class="sxs-lookup"><span data-stu-id="a07e1-112">Documentation</span></span>

<span data-ttu-id="a07e1-113">事後過程中的所有重要技術調查都會以錯誤或開發變更要求的形式，于報表和服務投資或修復中取得。</span><span class="sxs-lookup"><span data-stu-id="a07e1-113">All key technical findings in the postmortem process are captured in a report and service investments or fixes in the form of bugs or development change requests.</span></span> <span data-ttu-id="a07e1-114">這些結果會遵循適當的工程團隊。</span><span class="sxs-lookup"><span data-stu-id="a07e1-114">These findings are followed-up with the appropriate engineering teams.</span></span> <span data-ttu-id="a07e1-115">針對流程失敗及跨組織的問題，問題會記錄在 Microsoft 365 安全性回應小組的資料庫中，並遵循適當的群組來處理這些問題。</span><span class="sxs-lookup"><span data-stu-id="a07e1-115">For process failures and cross-organizational issues, issues are documented in the Microsoft 365 Security Response team's database and followed-up with the appropriate groups to address them.</span></span>

## <a name="process-improvement"></a><span data-ttu-id="a07e1-116">進程改進</span><span class="sxs-lookup"><span data-stu-id="a07e1-116">Process improvement</span></span>

<span data-ttu-id="a07e1-117">回應 Microsoft 365 中的安全性事件，涉及與跨 Microsoft 不同組織的多個群組進行協調，以及可能的適當外部組織，例如法律強制執行。</span><span class="sxs-lookup"><span data-stu-id="a07e1-117">Responding to a security incident in Microsoft 365 involves coordination with multiple groups spread across different organizations within Microsoft, and potentially even appropriate external organizations such as law enforcement.</span></span> <span data-ttu-id="a07e1-118">我們知道，在每個安全性事件（sufficiency 及完整性）之後，評估我們的回應是很重要的。</span><span class="sxs-lookup"><span data-stu-id="a07e1-118">We know that it is critical to evaluate our responses after every security incident for both sufficiency and completeness.</span></span> <span data-ttu-id="a07e1-119">針對任何已識別的改善或變更，Microsoft 365 安全性回應小組會評估與適當小組和專案關係人進行諮詢的建議，並在適當的情況下將其融入標準運作程式中。</span><span class="sxs-lookup"><span data-stu-id="a07e1-119">For any identified improvements or changes, the Microsoft 365 Security Response team evaluates the suggestions in consultation with the appropriate teams and stakeholders, and where appropriate incorporates them into standard operating procedures.</span></span> <span data-ttu-id="a07e1-120">在安全事件回應或事後活動中所識別的所有必要變更、bug 或服務改進都會在內部 Microsoft 365 工程資料庫中記錄及追蹤。</span><span class="sxs-lookup"><span data-stu-id="a07e1-120">All required changes, bugs, or service improvements identified during the security incident response or postmortem activity are logged and tracked in an internal Microsoft 365 engineering database.</span></span> <span data-ttu-id="a07e1-121">所有潛在的錯誤或功能會指派給適當的擁有者。</span><span class="sxs-lookup"><span data-stu-id="a07e1-121">All potential bugs or features are assigned to the appropriate owner.</span></span> <span data-ttu-id="a07e1-122">Microsoft 365 安全性回應小組會檢查所有專案，直到問題解決為止。</span><span class="sxs-lookup"><span data-stu-id="a07e1-122">The Microsoft 365 Security Response team reviews all entries until the issue is resolved.</span></span>

## <a name="related-articles"></a><span data-ttu-id="a07e1-123">相關文章</span><span class="sxs-lookup"><span data-stu-id="a07e1-123">Related articles</span></span>

- [<span data-ttu-id="a07e1-124">Microsoft 365 安全性事件管理</span><span class="sxs-lookup"><span data-stu-id="a07e1-124">Microsoft 365 security incident management</span></span>](assurance-security-incident-management.md)
- [<span data-ttu-id="a07e1-125">Microsoft 365 的安全性事件管理準備</span><span class="sxs-lookup"><span data-stu-id="a07e1-125">Microsoft 365 security incident management preparation</span></span>](assurance-sim-preparation.md)
- [<span data-ttu-id="a07e1-126">Microsoft 365 安全性事件管理偵測和分析</span><span class="sxs-lookup"><span data-stu-id="a07e1-126">Microsoft 365 security incident management detection and analysis</span></span>](assurance-sim-detection-analysis.md)
- [<span data-ttu-id="a07e1-127">Microsoft 365 的安全性事件管理包容、eradication 及恢復</span><span class="sxs-lookup"><span data-stu-id="a07e1-127">Microsoft 365 security incident management containment, eradication, and recovery</span></span>](assurance-sim-containment-eradication-recovery.md)
