---
title: Microsoft 員工轉接及終止
description: 深入瞭解 Microsoft 員工的轉接與終止程式 Microsoft 365
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
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: b31dd13f4a6209712a9cc212ab3bcd9c5addf6b7
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089609"
---
# <a name="microsoft-employee-transfer-and-termination"></a><span data-ttu-id="caae3-103">Microsoft 員工轉接及終止</span><span class="sxs-lookup"><span data-stu-id="caae3-103">Microsoft employee transfer and termination</span></span>

<span data-ttu-id="caae3-104">「員工轉接」和「終止」是每家組織一般商務運作的一部分。</span><span class="sxs-lookup"><span data-stu-id="caae3-104">Employee transfers and terminations are a part of every organization's normal business operations.</span></span> <span data-ttu-id="caae3-105">當員工變更職位或離開公司時，請務必及時撤銷不適當的存取。</span><span class="sxs-lookup"><span data-stu-id="caae3-105">When an employee changes positions or leaves the company, it is essential to revoke inappropriate access in a timely manner.</span></span> <span data-ttu-id="caae3-106">為了有利於有效的存取變更和存取 revocations，Microsoft 365 使用標準化的程式和自動化程式，協調人力資源資訊系統 (HRIS) 與身分識別管理 (IDM) System。</span><span class="sxs-lookup"><span data-stu-id="caae3-106">To facilitate efficient access changes and access revocations, Microsoft 365 uses standardized procedures and automated processes to coordinate the Human Resources Information System (HRIS) with the Identity Management (IDM) system.</span></span> <span data-ttu-id="caae3-107">這兩個系統之間的自動化業務流程對於維護運作一致性、保護 Microsoft 365 的服務和資料、避免特權蔓延，以及減少與內幕威脅相關的風險而言，都是必要的。</span><span class="sxs-lookup"><span data-stu-id="caae3-107">Automated orchestration between these two systems is essential to maintaining operational consistency, safeguarding Microsoft 365's services and data, preventing privilege creep, and reducing risks related to insider threats.</span></span>

<span data-ttu-id="caae3-108">Microsoft 365 的系統設計為可運作，而不需對我們的工程師進行實際執行環境的系統管理存取。</span><span class="sxs-lookup"><span data-stu-id="caae3-108">Microsoft 365 systems are designed to operate without standing administrative access to production environments for our engineers.</span></span> <span data-ttu-id="caae3-109">Microsoft 會使用即時 (JIT) ，只需足夠存取 (JEA) 模型，以在必要時為工程師提供必要的臨時存取，以支援其服務。</span><span class="sxs-lookup"><span data-stu-id="caae3-109">Microsoft uses a Just-In-Time (JIT), Just-Enough-Access (JEA) model to provide engineers with the temporary access needed to support their service when required.</span></span> <span data-ttu-id="caae3-110">若要要求和使用服務小群組帳戶進行 JIT 存取，工程師必須透過 IDM 工具要求及維護 eligibilities。</span><span class="sxs-lookup"><span data-stu-id="caae3-110">To request and use a service team account for JIT access, engineers must request and maintain eligibilities through the IDM tool.</span></span> <span data-ttu-id="caae3-111">當員工轉移或終止時，系統會自動修改其服務小群組帳戶和相關的 eligibilities，以防止不適當的存取。</span><span class="sxs-lookup"><span data-stu-id="caae3-111">When employees are transferred or terminated, their service team account and related eligibilities are automatically modified to prevent inappropriate access.</span></span>

## <a name="transfer-and-reassignment"></a><span data-ttu-id="caae3-112">轉移和重新指派</span><span class="sxs-lookup"><span data-stu-id="caae3-112">Transfer and reassignment</span></span>

<span data-ttu-id="caae3-113">員工轉帳是透過員工主管的轉移交易要求來啟動。</span><span class="sxs-lookup"><span data-stu-id="caae3-113">Employee transfers are initiated through a transfer transaction request by the employee's manager.</span></span> <span data-ttu-id="caae3-114">管理員會建立一項申請，並與全球人才購置提供的信件流程。</span><span class="sxs-lookup"><span data-stu-id="caae3-114">The manager creates a requisition and engages with Global Talent Acquisition for the offer letter process.</span></span> <span data-ttu-id="caae3-115">一旦員工接受新角色的提供，HR 服務便會在人力資源核心工具中完成傳輸，觸發 IDM 以設定所有員工 eligibilities 的到期日。</span><span class="sxs-lookup"><span data-stu-id="caae3-115">Once the employee accepts the offer for the new role, HR services completes the transfer in the HR core tools, triggering IDM to set an expiration date for all the employee's eligibilities.</span></span> <span data-ttu-id="caae3-116">員工必須送出要求並收到其新管理員的核准，以保留其 eligibilities。</span><span class="sxs-lookup"><span data-stu-id="caae3-116">The employee must submit a request and receive approval from their new manager to retain their eligibilities.</span></span> <span data-ttu-id="caae3-117">無法提交要求或接收管理員核准會導致已轉移員工的 eligibilities 撤銷。</span><span class="sxs-lookup"><span data-stu-id="caae3-117">Failure to submit a request or receive manager approval results in the revocation of the transferred employee's eligibilities.</span></span> <span data-ttu-id="caae3-118">針對包含特定安全性含義的傳輸，系統存取和安全性群組成員資格會立即重新評估，以反映其新角色。</span><span class="sxs-lookup"><span data-stu-id="caae3-118">For transfers that include specific security implications, system accesses and security group memberships are reevaluated immediately to reflect their new role.</span></span>

## <a name="termination"></a><span data-ttu-id="caae3-119">終止</span><span class="sxs-lookup"><span data-stu-id="caae3-119">Termination</span></span>

<span data-ttu-id="caae3-120">Microsoft 使用明確定義的原則和程式，在員工終止時立即撤銷對 Microsoft 系統和資源的實體和邏輯存取。</span><span class="sxs-lookup"><span data-stu-id="caae3-120">Microsoft uses clearly defined policies and procedures to promptly revoke physical and logical access to Microsoft systems and resources when an employee is terminated.</span></span> <span data-ttu-id="caae3-121">當員工提供通知時，該員工的主管會將終止日期輸入 HRIS。</span><span class="sxs-lookup"><span data-stu-id="caae3-121">When an employee gives their notice, the employee's manager enters the termination date into the HRIS.</span></span> <span data-ttu-id="caae3-122">在員工的最後一天之後，HRIS 會將該員工標示為已終止，並將該資訊共用給 IDM，這會自動移除所有的服務小群組帳戶和 eligibilities。</span><span class="sxs-lookup"><span data-stu-id="caae3-122">Following the employee's last working day, the HRIS marks the employee as terminated and shares the information to IDM, which removes all service team accounts and eligibilities automatically.</span></span>

<span data-ttu-id="caae3-123">針對 involuntary 終止，HR 與員工的主管合作，遵循適當的步驟來終止和下架員工。</span><span class="sxs-lookup"><span data-stu-id="caae3-123">For involuntary terminations, HR works with the employee's manager to follow the appropriate steps to terminate and offboard the employee.</span></span> <span data-ttu-id="caae3-124">與自願終止類似，終止資訊會輸入 HRIS，以及任何必要的步驟，例如有效的日期協調、存取權移除。</span><span class="sxs-lookup"><span data-stu-id="caae3-124">Similar to a voluntary termination, the termination information is entered into the HRIS along with any necessary steps such as effective date coordination, access removal.</span></span> <span data-ttu-id="caae3-125">和任何其他與角色轉換相關的步驟。</span><span class="sxs-lookup"><span data-stu-id="caae3-125">and any other steps relative to transitioning out of role.</span></span>
