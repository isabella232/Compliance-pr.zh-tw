---
title: 使用安全性與合規性中心的 DSR 案例工具來管理 GDPR 資料主體要求
description: 了解如何使用 DSR 案例工具管理歐盟一般資料保護規定 （GDPR） 資料主體要求。
f1.keywords:
- NOCSH
ms.author: markjjo
author: markjjo
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
localization_priority: Priority
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- SPO_Content
- MS-Compliance
ms.assetid: ce9eb942-3589-42cb-88fd-1576ecb09c5c
ms.custom: seo-marvel-apr2020
hideEdit: true
ms.openlocfilehash: 8448d9a77352491ce0066dbf74ed5aea0e8f7a29
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089576"
---
# <a name="manage-gdpr-data-subject-requests-with-the-dsr-case-tool-in-the-security--compliance-center"></a><span data-ttu-id="d3ce0-103">使用安全性與合規性中心的 DSR 案例工具來管理 GDPR 資料主體要求</span><span class="sxs-lookup"><span data-stu-id="d3ce0-103">Manage GDPR data subject requests with the DSR case tool in the Security & Compliance Center</span></span>

<span data-ttu-id="d3ce0-104">歐盟一般資料保護規定 (GDPR) 專為保護和賦予歐盟 (EU) 內部個人隱私權而設計。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-104">The EU General Data Protection Regulation (GDPR) is about protecting and enabling individuals' privacy rights inside the European Union (EU).</span></span> <span data-ttu-id="d3ce0-105">GDPR 賦予歐盟的個人 (稱為資料主體) 存取、擷取、更正、清除及限制其個人資料處理的權利。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-105">The GDPR gives individuals in the European Union (known as data subjects) the right to access, retrieve, correct, erase, and restrict processing of their personal data.</span></span> <span data-ttu-id="d3ce0-106">根據 GDPR，個人資料意指與已識別或可識別自然人相關的任何資訊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-106">Under the GDPR, personal data means any information relating to an identified or identifiable natural person.</span></span> <span data-ttu-id="d3ce0-107">由個人向其組織提出以對其個人資料採取動作的正式要求，稱為資料主體要求或 DSR。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-107">A formal request by a person to their organization to take an action on their personal data is called a Data Subject Request or DSR.</span></span> <span data-ttu-id="d3ce0-108">如需有關回應 Office 365 中資料的 DSR 的詳細資訊，請參閱 [Office 365 資料主體要求指南](https://go.microsoft.com/fwlink/?linkid=871169 )。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-108">For detailed information about responding to DSRs for data in Office 365, see [Office 365 Data Subject Request Guide](https://go.microsoft.com/fwlink/?linkid=871169 ).</span></span>
  
<span data-ttu-id="d3ce0-109">若要管理調查以回應貴組織中人員提交的 DSR，您可以使用安全性與合規性中心的 DSR 案例工具尋找儲存在下列位置的內容：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-109">To manage investigations in response to a DSR submitted by a person in your organization, you can use the DSR case tool in the Security & Compliance Center to find content stored in:</span></span>
  
- <span data-ttu-id="d3ce0-110">組織中的任何使用者信箱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-110">Any user mailbox in your organization.</span></span> <span data-ttu-id="d3ce0-111">這包括 Microsoft Teams 中的商務用 Skype 交談和一對一聊天</span><span class="sxs-lookup"><span data-stu-id="d3ce0-111">This includes Skype for Business conversations and one-to-one chats in Microsoft Teams</span></span>
    
- <span data-ttu-id="d3ce0-112">與 Microsoft 365 群組相關聯的所有信箱，以及 Microsoft Teams 中的所有小組信箱</span><span class="sxs-lookup"><span data-stu-id="d3ce0-112">All mailboxes associated with an Microsoft 365 Group and all team mailboxes in Microsoft Teams</span></span>
    
- <span data-ttu-id="d3ce0-113">貴組織中所有的 SharePoint Online 網站和商務用 OneDrive 帳戶</span><span class="sxs-lookup"><span data-stu-id="d3ce0-113">All SharePoint Online sites and OneDrive for Business accounts in your organization</span></span>
    
- <span data-ttu-id="d3ce0-114">貴組織中所有的 Teams 網站和 Microsoft 365 群組網站</span><span class="sxs-lookup"><span data-stu-id="d3ce0-114">All Teams sites and Microsoft 365 Group sites in your organization</span></span>
    
- <span data-ttu-id="d3ce0-115">Exchange Online 中的所有公用資料夾</span><span class="sxs-lookup"><span data-stu-id="d3ce0-115">All public folders in Exchange Online</span></span>
    
<span data-ttu-id="d3ce0-116">使用 DSR 案例工具，您可以：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-116">Using the DSR case tool you can:</span></span>
  
- <span data-ttu-id="d3ce0-117">針對每一個 DSR 調查建立個別案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-117">Create a separate case for each DSR investigation.</span></span>
    
- <span data-ttu-id="d3ce0-118">藉由將人員新增為案例成員，來控制誰可以存取此案例；只有成員才能存取案例，而且在安全性與合規性中心內的 **[DSR 案例]** 頁面上，他們只能在案例清單上看到自己的案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-118">Control who has access to the DSR case by adding people as members of the case; only members can access the case and can only see their cases in the list of cases on the **DSR cases** page in the Security & Compliance Center.</span></span> <span data-ttu-id="d3ce0-119">此外，您也可以將不同的權限指派給相同案例的不同成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-119">Also, you can assign different permissions to different members of the same case.</span></span> <span data-ttu-id="d3ce0-120">例如，您可以允許某些成員只能檢視案例和搜尋結果，而允許其他成員建立搜尋並匯出搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-120">For example, you can allow some members to only view the case and search results and allow other members to create searches and export search results.</span></span> 
    
- <span data-ttu-id="d3ce0-121">使用內建搜尋搜尋特定資料主體建立或更新的所有內容。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-121">Use the built-in search to search for all content created or uploaded by a specific data subject.</span></span>
    
- <span data-ttu-id="d3ce0-122">選擇性地修改內建搜尋查詢，然後重新執行搜尋以縮小搜尋結果範圍。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-122">Optionally revise the built-in search query and rerun the search to narrow the search results.</span></span>
    
- <span data-ttu-id="d3ce0-123">新增與 DSR 案例相關聯的其他內容搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-123">Add other content searches associated with the DSR case.</span></span> <span data-ttu-id="d3ce0-124">這包括建立可從 Office 漫遊服務傳回部分編製索引的項目和系統產生的記錄的搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-124">This includes creating searches that return partially indexed items and system-generated logs from the Office Roaming Service.</span></span>
    
- <span data-ttu-id="d3ce0-125">匯出資料以回應 DSR 存取或匯出要求。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-125">Export data in response to a DSR access or export request.</span></span>
    
- <span data-ttu-id="d3ce0-p105">DSR 調查程序完成時，請刪除案例。這會移除與案例相關聯的所有搜尋和匯出工作。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-p105">Delete cases when the DSR investigation process is complete. This removes all searches and export jobs associated with the case.</span></span>
    
<span data-ttu-id="d3ce0-128">以下是使用 DSR 案例工具管理 DSR 調查的高層級程序：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-128">Here's the high-level process for using the DSR case tool to manage DSR investigations:</span></span>
  
[<span data-ttu-id="d3ce0-129">步驟 1：將電子文件探索權限指派給潛在的案例成員</span><span class="sxs-lookup"><span data-stu-id="d3ce0-129">Step 1: Assign eDiscovery permissions to potential case members</span></span>](#step-1-assign-ediscovery-permissions-to-potential-case-members)

[<span data-ttu-id="d3ce0-130">步驟 2：建立 DSR 案例並新增成員</span><span class="sxs-lookup"><span data-stu-id="d3ce0-130">Step 2: Create a DSR case and add members</span></span>](#step-2-create-a-dsr-case-and-add-members)

[<span data-ttu-id="d3ce0-131">步驟 3：執行搜尋查詢</span><span class="sxs-lookup"><span data-stu-id="d3ce0-131">Step 3: Run the search query</span></span>](#step-3-run-the-search-query)

[<span data-ttu-id="d3ce0-132">步驟 4：匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-132">Step 4: Export the data</span></span>](#step-4-export-the-data)

[<span data-ttu-id="d3ce0-133">(選擇性) 步驟 5：修改內建搜尋查詢</span><span class="sxs-lookup"><span data-stu-id="d3ce0-133">(Optional) Step 5: Revise the built-in search query</span></span>](#optional-step-5-revise-the-built-in-search-query)

[<span data-ttu-id="d3ce0-134">關於使用 DSR 案例工具的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="d3ce0-134">More information about using the DSR case tool</span></span>](#more-information-about-using-the-dsr-case-tool)
  
> [!IMPORTANT]
> <span data-ttu-id="d3ce0-135">我們的工具可讓系統管理員利用 DSR 案例工具中找到的內建搜尋和匯出功能，協助他們執行 DSR 存取或匯出要求。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-135">Our tools can help admins perform DSR access or export requests by enabling them to utilize the built-in search and export functionality found in the DSR case tool.</span></span> <span data-ttu-id="d3ce0-136">此工具有助於採用最佳方法，匯出與資料主體所提交之 DSR 要求相關的資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-136">The tool helps to facilitate a best-effort method to export data that's relevant to a DSR request submitted by a data subject.</span></span> <span data-ttu-id="d3ce0-137">但是請注意，搜尋結果可能會因為資料主體或系統管理動作而異，這可能會基於匯出用途，影響是否將項目視為「個人資料」。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-137">However, it's important to note that search results can vary based on the data subject or the admin actions taken that may impact whether or not an item would be deemed as "personal data" for export purposes.</span></span> <span data-ttu-id="d3ce0-138">例如，如果資料主體是檔案建立者以外的最後一個檔案修改者，則可能不會在搜尋結果中傳回該檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-138">For example, if the data subject was the last person to modify a file they didn't create, the file might not be returned in the search results.</span></span> <span data-ttu-id="d3ce0-139">同樣地，系統管理員可以匯出資料，但不包含部分編製索引的項目或所有版本的 SharePoint 文件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-139">Similarly, an admin could export data without including partially indexed items or all versions of SharePoint documents.</span></span> <span data-ttu-id="d3ce0-140">因此，提供的工具有助於存取和匯出資料要求，不過，結果會受特定系統管理員和資料主體使用案例所限制。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-140">Therefore, the tools provided can help facilitate accessing and exporting data requests; however, the results are subject to specific admin and data subject usage scenarios.</span></span> 
  
## <a name="step-1-assign-ediscovery-permissions-to-potential-case-members"></a><span data-ttu-id="d3ce0-141">步驟 1：將電子文件探索權限指派給潛在的案例成員</span><span class="sxs-lookup"><span data-stu-id="d3ce0-141">Step 1: Assign eDiscovery permissions to potential case members</span></span>

<span data-ttu-id="d3ce0-142">根據預設，全域系統管理員可以存取安全性與合規性中心的 DSR 案例工具。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-142">By default, a global administrator can access the DSR case tool in the Security & Compliance Center.</span></span> <span data-ttu-id="d3ce0-143">根據設計，其他使用者 (例如資料隱私權主管、人力資源經理或涉及 DSR 調查的其他人員) 無法存取 DSR 案例工具，而且必須獲指派適當的權限，才能存取此工具。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-143">By design, other users such as a data privacy officer, a human resources manager, or other people involved in DSR investigations don't have access to the DSR case tool and will have to be assigned the appropriate permissions to access the tool.</span></span> <span data-ttu-id="d3ce0-144">若要指派權限，最簡單的方法是前往安全性與合規性中心內的 **[權限]** 頁面，然後將使用者新增到 [電子文件探索管理員] 角色群組。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-144">The easiest way to do this is to go to the **Permissions** page in the Security & Compliance Center and add users to the eDiscovery Manager role group.</span></span> <span data-ttu-id="d3ce0-145">您還必須指派這些權限，才能將其新增為步驟 2 中建立之 DSR 案例的成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-145">You also have to assign these permissions so you can add them as members of the DSR case that you create in Step 2.</span></span> 
  
<span data-ttu-id="d3ce0-146">如需逐步指示，請參閱[在 Office 365 安全性與合規性中心中指派電子文件探索權限](/microsoft-365/compliance/assign-ediscovery-permissions)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-146">For step-by-step instructions, see [Assign eDiscovery permissions in the Office‍ 365 Security & Compliance Center](/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>
  
> [!NOTE]
> <span data-ttu-id="d3ce0-147">根據預設，全域系統管理員 (或安全性與合規性中心中 [組織管理] 角色群組的其他成員) 沒有匯出內容搜尋結果所需的權限 (請參閱本文中的步驟 4)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-147">By default, a global administrator (or other members of the Organization Management role group in the Security & Compliance Center don't have the necessary permissions to export Content Search results (see Step 4 in this article).</span></span> <span data-ttu-id="d3ce0-148">若要解決這個問題，系統管理員可以將自己新增為 [電子郵件探索管理員] 角色群組的成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-148">To address this, an admin can add themselves as a member of the eDiscovery Manager role group.</span></span> 
  
## <a name="step-2-create-a-dsr-case-and-add-members"></a><span data-ttu-id="d3ce0-149">步驟 2：建立 DSR 案例並新增成員</span><span class="sxs-lookup"><span data-stu-id="d3ce0-149">Step 2: Create a DSR case and add members</span></span>

<span data-ttu-id="d3ce0-150">下一個步驟是建立 DSR 案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-150">The next step is to create a DSR case.</span></span> <span data-ttu-id="d3ce0-151">建立案例時，您可以選擇啟動內建搜尋，也可以建立案例但不啟動搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-151">When you create a case, you can choose to start the built-in search or you can create the case without starting the search.</span></span> <span data-ttu-id="d3ce0-152">下列程序會指示您建立案例但不啟動搜尋，然後示範如何將成員新增到案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-152">The following procedure instructs you to create the case without starting the search and then show you how to add members to the case.</span></span>
  
1. <span data-ttu-id="d3ce0-153">前往 [https://protection.office.com](https://protection.office.com)，然後使用您的公司或學校帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-153">Go to [https://protection.office.com](https://protection.office.com) and sign in using your work or school account.</span></span> 
    
2. <span data-ttu-id="d3ce0-154">在安全性與合規性中心，按一下 **[資料隱私權]** \> **[資料主體要求]**，然後按一下 ![[新增圖示]](../media/ITPro-EAC-AddIcon.gif) **[新增 DSR 案例]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-154">In the Security & Compliance Center, click **Data privacy** \> **Data subject requests**, and then click ![Add Icon](../media/ITPro-EAC-AddIcon.gif) **New DSR case**.</span></span>
    
3. <span data-ttu-id="d3ce0-155">在 **[新增 DSR 案例]** 飛出視窗頁面上，為案例命名、輸入選擇性描述，然後按一下 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-155">On the **New DSR case** flyout page, give the case a name, type an optional description, and then click **Next**.</span></span> <span data-ttu-id="d3ce0-156">案例名稱在組織中必須是唯一的。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-156">The name of the case must be unique in your organization.</span></span>
    
    > [!TIP]
    > <span data-ttu-id="d3ce0-157">請考慮在新案例的名稱和/或描述中，新增提交您調查之 DSR 要求之人員的名稱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-157">Consider adding the name of the person who submitted the DSR request that you're investigating in the name and/or description of the new case.</span></span> <span data-ttu-id="d3ce0-158">請注意，只有此案例的成員 (以及電子文件探索系統管理員) 才能在 **[資料主體要求]** 頁面的案例清單中看到此案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-158">Note that only members of this case (and eDiscovery Administrators) will be able to see the case in the list of cases on the **Data subject requests** page.</span></span> 
  
4. <span data-ttu-id="d3ce0-159">在 **[要求詳細資料]** 頁面的 **[資料主體 (提出此要求的人員)]** 下，選取要尋找並匯出資料的人員，然後按一下 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-159">On the **Request details** page, under **Data subject (the person who filed this request)**, select the person that you want to find and export data for and then click **Next**.</span></span>
    
5. <span data-ttu-id="d3ce0-160">在 **[確認您的案例設定]** 頁面上，您可以變更案例名稱和描述，以及選取不同的資料主體。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-160">On the **Confirm your case settings** page, you can change the case name and description, and select a different data subject.</span></span> <span data-ttu-id="d3ce0-161">否則，按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-161">Otherwise, click **Save**.</span></span>
    
    <span data-ttu-id="d3ce0-162">系統會顯示一個頁面，確認已建立新的 DSR 案例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-162">A page is displayed that confirms the new DSR case has been created.</span></span>
    
    ![開始搜尋或關閉 [新增 DSR 案例] 頁面](../media/b5e62c2c-cafe-4a8d-a38c-789ed9f9ccbd.png)
  
    <span data-ttu-id="d3ce0-164">此時，您可以執行下列其中一項操作：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-164">At this point, you can do one of two things:</span></span>
    
    <span data-ttu-id="d3ce0-165">a.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-165">a.</span></span> <span data-ttu-id="d3ce0-166">按一下 **[顯示搜尋結果]** 開始搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-166">Clicking **Show me search results** starts the search.</span></span> <span data-ttu-id="d3ce0-167">這是預設選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-167">This is the default selection.</span></span> <span data-ttu-id="d3ce0-168">您選取此選項時所執行的內建搜尋以及所傳回的結果將會在步驟 3 討論。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-168">The built-in search that's run when you select this option and the results that are returned are discussed in Step 3.</span></span>
    
    <span data-ttu-id="d3ce0-169">b.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-169">b.</span></span> <span data-ttu-id="d3ce0-170">按一下 **[完成]** 關閉新的 DSR 案例，而不啟動內建搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-170">Clicking **Finish** closes the new DSR case without starting the built-in search.</span></span> <span data-ttu-id="d3ce0-171">當您選取此選項時，新的 DSR 案例會顯示在 **[資料主體要求]** 頁面上。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-171">When you select this option, the new DSR case is displayed on the **Data subject requests** page.</span></span>
    
6. <span data-ttu-id="d3ce0-172">按一下 **[完成]**，讓您可以進入新的 DSR 案例，並在其中新增成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-172">Click **Finish** so that you can go in to the new DSR case and add members to it.</span></span> 
    
7. <span data-ttu-id="d3ce0-173">在 **[資料主體要求]** 頁面上，按一下您所建立之 DSR 案例的名稱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-173">On the **Data subject requests** page, click the name of the DSR case that you created.</span></span> 
    
8. <span data-ttu-id="d3ce0-174">在 **[管理此案例]** 飛出視窗頁面的 **[管理成員]** 下，按一下 **[新增]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-174">On the **Manage this case** flyout page, under **Manage members**, click **Add**.</span></span> 
    
    <span data-ttu-id="d3ce0-175">在 **[使用者]** 下，會顯示獲指派適當電子文件探索權限的人員的清單。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-175">Under **Users**, a list of people that are assigned the appropriate eDiscovery permissions is displayed.</span></span> <span data-ttu-id="d3ce0-176">您在步驟 1 中為其指派電子文件探索權限的人員將會顯示在此清單中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-176">The people you assigned eDiscovery permissions to in Step 1 will be displayed in this list.</span></span> 
    
9. <span data-ttu-id="d3ce0-177">選取要新增為 DSR 案例成員的人員、按一下 **[新增]**，然後儲存您的變更。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-177">Select the people to add as members of the DSR case, click **Add**, and then save your changes.</span></span>
    
    <span data-ttu-id="d3ce0-178">您也可以按一下 **[管理角色群組]** 底下的 **[新增]**，將角色群組新增為 DSR 案例的成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-178">You can also add role groups as members of DSR case by clicking **Add** under **Manage role groups**.</span></span> 
    
## <a name="step-3-run-the-search-query"></a><span data-ttu-id="d3ce0-179">步驟 3：執行搜尋查詢</span><span class="sxs-lookup"><span data-stu-id="d3ce0-179">Step 3: Run the search query</span></span>

<span data-ttu-id="d3ce0-180">建立 DSR 案例並新增成員之後，下一步是執行與案例相關聯的內建搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-180">After you create a DSR case and add members, the next step is to run the built-in search that's associated with the case.</span></span> <span data-ttu-id="d3ce0-181">此預設搜尋查詢會執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-181">This default search query does the following things:</span></span>
  
- <span data-ttu-id="d3ce0-182">搜尋貴組織中的所有信箱，以尋找資料主體所傳送或接收的所有電子郵件項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-182">Searches all mailboxes in your organization for all email items that were sent or received by the data subject.</span></span> <span data-ttu-id="d3ce0-183">您可以使用 *[參與者]* 電子郵件屬性，在電子郵件訊息的所有人員欄位中搜尋資料主體，以完成此操作。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-183">This is accomplished by using the  *Participants*  email property, which searches for the data subject in all the people fields in an email message.</span></span> <span data-ttu-id="d3ce0-184">此屬性會傳回資料主體位於 **[寄件者]**、**[收件者]**、**[副本]** 和 **[密件副本]** 欄位中的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-184">This property returns items in which the data subject is in the **From**, **To**, **CC**, and **BCC** fields.</span></span> <span data-ttu-id="d3ce0-185">系統也會搜尋 Exchange Online 的公用資料夾中，資料主體所傳送或接收的郵件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-185">Public folders in Exchange Online are also searched for messages sent or received by the data subject.</span></span> 
    
- <span data-ttu-id="d3ce0-186">搜尋貴組織的所有網站，尋找資料主體建立或上傳的文件和項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-186">Searches all sites in your organization for documents and items created or uploaded by the data subject.</span></span> <span data-ttu-id="d3ce0-187">您可以使用下列網站屬性，完成此操作：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-187">This is accomplished by using the following site properties:</span></span>
    
  - <span data-ttu-id="d3ce0-188">*Author* 屬性會傳回資料主體列在 Office 文件的作者欄位中的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-188">The  *Author*  property returns items where the data subject is listed in the author field in Office documents.</span></span> <span data-ttu-id="d3ce0-189">即使文件是由其他人複製和上傳，此值仍然存在。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-189">This value persists, even if the document is copied and uploaded by someone else.</span></span> 
    
  - <span data-ttu-id="d3ce0-190">*CreatedBy* 屬性會傳回資料主體所建立或上傳的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-190">The  *CreatedBy*  property returns items that were created or uploaded by the data subject.</span></span> 
    
<span data-ttu-id="d3ce0-191">以下是在您建立 DSR 案例時自動建立之內建搜尋的關鍵字查詢外觀。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-191">Here's what the keyword query looks like for the built-in search that gets automatically created when you create a DSR case.</span></span>
  
```powershell
participants:"<email address>" OR author:"<display name>" OR createdby:"<display name>"
```

<span data-ttu-id="d3ce0-192">例如，如果資料主體的名稱是 Ina Leonte，關鍵字查詢看起來會像這樣：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-192">For example, if the name of the data subject is Ina Leonte, the keyword query would look like this:</span></span>
  
```powershell
participants:"ina@contoso.com" OR author:"Ina Leonte" OR createdby:"Ina Leonte"
```

 <span data-ttu-id="d3ce0-193">**若要執行 DSR 案例的內建搜尋：**</span><span class="sxs-lookup"><span data-stu-id="d3ce0-193">**To run the built-in search for a DSR case:**</span></span>
  
1. <span data-ttu-id="d3ce0-194">在安全性與合規性中心，按一下 **[資料隱私權]** \> **[資料主體要求]**，然後按一下您在步驟 2 中建立的 DSR 案例旁的 **[開啟]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-194">In the Security & Compliance Center, click **Data privacy** \> **Data subject requests**, and then click **Open** next to the DSR case that you created in Step 2.</span></span> 
    
    <span data-ttu-id="d3ce0-195">按一下頁面頂端的 **[搜尋]** 索引標籤，然後按一下建立 DSR 案例時所建立之內建搜尋旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-195">Click the **Search** tab at the top of the page, and then click the checkbox next to the built-in search that was created when you created the DSR case.</span></span> <span data-ttu-id="d3ce0-196">搜尋與 DSR 案例的名稱相同。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-196">The search has the same name as the DSR case.</span></span> 
    
2. <span data-ttu-id="d3ce0-197">在 [搜尋] 飛出視窗頁面上，按一下 **[開啟查詢]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-197">In the search flyout page, click **Open query**.</span></span>
    
    <span data-ttu-id="d3ce0-198">當您開啟查詢時，搜尋隨即啟動，並將於幾分鐘後完成。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-198">When you open the query, the search is started and will complete in a few moments.</span></span> 
    
3. <span data-ttu-id="d3ce0-199">搜尋完成後，按一下 **[預覽結果]** 可預覽搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-199">When the search is complete, click **Preview results** to preview the search results.</span></span> <span data-ttu-id="d3ce0-200">如需詳細資訊，請參閱[預覽搜尋結果](/microsoft-365/compliance/content-search#preview-search-results)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-200">For more information, see [Preview search results](/microsoft-365/compliance/content-search#preview-search-results).</span></span>
    
    > [!TIP]
    > <span data-ttu-id="d3ce0-201">您也可以檢視搜尋查詢統計資料，以查看搜尋所傳回的信箱和網站項目數目，以及包含符合搜尋查詢之項目的熱門內容位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-201">You can also view the search query statistics to see the number of mailbox and site items that are returned by the search, and the top content locations that contain items that match the search query.</span></span> <span data-ttu-id="d3ce0-202">如需詳細資訊，請參閱[檢視有關搜尋的資訊和統計資料](/microsoft-365/compliance/content-search#view-information-and-statistics-about-a-search)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-202">For more information, see [View information and statistics about a search](/microsoft-365/compliance/content-search#view-information-and-statistics-about-a-search).</span></span> 
  
<span data-ttu-id="d3ce0-203">您可以編輯內建搜尋查詢、變更搜尋的內容位置，然後重新執行搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-203">You can edit the built-in search query, change the content locations that are searched, and then rerun the search.</span></span> <span data-ttu-id="d3ce0-204">如需詳細資訊，請參閱[步驟 5](#optional-step-5-revise-the-built-in-search-query)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-204">See [Step 5](#optional-step-5-revise-the-built-in-search-query) for more information.</span></span> 
  
## <a name="step-4-export-the-data"></a><span data-ttu-id="d3ce0-205">步驟 4：匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-205">Step 4: Export the data</span></span>

<span data-ttu-id="d3ce0-206">執行內建搜尋之後，您可以匯出搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-206">After you run the built-in search, you can export the search results.</span></span> <span data-ttu-id="d3ce0-207">或者，在匯出資料之前，您可能會想要修改查詢以減少搜尋結果的數量。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-207">Alternatively, before you export the data, you may want to revise the query to reduce the number of search results.</span></span> <span data-ttu-id="d3ce0-208">如需有關縮小搜尋結果範圍的詳細資訊，請參閱步驟 5。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-208">See Step 5 for more information about narrowing the search results.</span></span>
  
<span data-ttu-id="d3ce0-209">當您匯出搜尋結果時，可以將信箱項目下載為 PST 檔案或個別郵件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-209">When you export search results, mailbox items can be downloaded in PST files or as individual messages.</span></span> <span data-ttu-id="d3ce0-210">從 SharePoint 和 OneDrive 帳戶匯出內容時，會匯出原生 Office 文件和其他文件的副本。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-210">When you export content from SharePoint and OneDrive accounts, copies of native Office documents and other documents are exported.</span></span> <span data-ttu-id="d3ce0-211">包含每個匯出項目相關資訊的結果檔案會包含在搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-211">A results file that contains information about every exported item is included with the search results.</span></span> <span data-ttu-id="d3ce0-212">如需有關匯出的詳細資訊，請參閱[匯出內容搜尋結果](/microsoft-365/compliance/export-search-results)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-212">For more detailed information about exporting, see [Export Content Search results](/microsoft-365/compliance/export-search-results).</span></span>
  
> [!NOTE]
> <span data-ttu-id="d3ce0-213">根據預設，全域系統管理員 (或安全性與合規性中心中 [組織管理] 角色群組的其他成員) 沒有匯出內容搜尋結果所需的權限。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-213">By default, a global administrator (or other members of the Organization Management role group in the Security & Compliance Center) don't have the necessary permissions to export Content Search results.</span></span> <span data-ttu-id="d3ce0-214">若要解決這個問題，系統管理員可以將自己新增為 [電子郵件探索管理員] 角色群組的成員。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-214">To address this, an admin can add themselves as a member of the eDiscovery Manager role group.</span></span> 
  
<span data-ttu-id="d3ce0-215">您用來匯出內容的電腦必須符合下列系統需求︰</span><span class="sxs-lookup"><span data-stu-id="d3ce0-215">The computer you use to export data has to meet the following system requirements:</span></span>
  
- <span data-ttu-id="d3ce0-216">Windows 7 和更新版本的 32 為原或 64 位元版本</span><span class="sxs-lookup"><span data-stu-id="d3ce0-216">32-bit or 64-bit versions of Windows 7 and later versions</span></span>
    
- <span data-ttu-id="d3ce0-217">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="d3ce0-217">Microsoft .NET Framework 4.7</span></span>
    
- <span data-ttu-id="d3ce0-218">支援的瀏覽器：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-218">A supported browser:</span></span>
    
  - <span data-ttu-id="d3ce0-219">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d3ce0-219">Microsoft Edge</span></span>
    
    <span data-ttu-id="d3ce0-220">或者</span><span class="sxs-lookup"><span data-stu-id="d3ce0-220">Or</span></span>
    
  - <span data-ttu-id="d3ce0-221">Microsoft Internet Explorer 10 和更新版本</span><span class="sxs-lookup"><span data-stu-id="d3ce0-221">Microsoft Internet Explorer 10 and later versions</span></span>
    
    > [!NOTE]
    > <span data-ttu-id="d3ce0-222">Microsoft 不會為 ClickOnce 應用程式製作協力廠商擴充功能或附加元件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-222">Microsoft doesn't manufacture third-party extensions or add-ons for ClickOnce applications.</span></span> <span data-ttu-id="d3ce0-223">不支援使用具有協力廠商擴充功能或附加元件的不支援瀏覽器匯出資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-223">Exporting data using an unsupported browser with third-party extensions or add-ons isn't supported.</span></span> 
  
 <span data-ttu-id="d3ce0-224">**若要從 DSR 案例中的內建搜尋匯出資料：**</span><span class="sxs-lookup"><span data-stu-id="d3ce0-224">**To export data from the built-in search in a DSR case:**</span></span>
  
1. <span data-ttu-id="d3ce0-225">在安全性與合規性中心，按一下 **[資料隱私權]** \> **[資料主體要求]**，然後按一下您要從中匯出資料的 DSR 案例旁的 **[開啟]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-225">In the Security & Compliance Center, click **Data privacy** \> **Data subject requests**, and then click **Open** next to the DSR case that you want to export data from.</span></span> 
    
2. <span data-ttu-id="d3ce0-226">按一下頁面頂端的 **[搜尋]** 索引標籤，然後按一下建立 DSR 案例時所建立之內建搜尋旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-226">Click the **Search** tab at the top of the page, and then click the checkbox next to the built-in search that was created when you created the DSR case.</span></span> <span data-ttu-id="d3ce0-227">或者，按一下其他搜尋，以便從該搜尋匯出資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-227">Or click another search to export data from that search.</span></span> 
    
3. <span data-ttu-id="d3ce0-228">在 [搜尋] 飛出視窗頁面上，按一下 ![[匯出搜尋結果圖示]](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **[其他]**，然後從下拉式清單選取 **[匯出結果]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-228">On the search flyout page, click ![Export search results icon](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **More**, and then select **Export results** from the drop-down list.</span></span> 
    
4. <span data-ttu-id="d3ce0-229">在 **[匯出結果]** 頁面上，選取下列 DSR 匯出要求的建議選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-229">On the **Export results** page, select the following recommended options for DSR export requests.</span></span> 
    
    ![設定匯出設定](../media/25416b79-57da-46a1-ae07-e640602a8fa4.png)
  
    <span data-ttu-id="d3ce0-231">a.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-231">a.</span></span> <span data-ttu-id="d3ce0-232">在 **[輸出選項]** 下，選取第一個選項 (**[所有項目，但不包含格式無法辨識的項目、已加密或因其他原因而未編製索引的項目]**)，以便僅匯出已編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-232">Under **Output options**, select the first option (**All items, excluding ones that have ones that have an unrecognized format, are encrypted, or weren't indexed for other reasons**) to export indexed items only.</span></span> <span data-ttu-id="d3ce0-233">您不想從內建搜尋匯出部分編製索引的項目的原因是，也會匯出其他使用者部分編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-233">The reason you don't want to export partially indexed items from the built-in search is because partially indexed items from other users will also be exported.</span></span> <span data-ttu-id="d3ce0-234">若要只匯出資料主體部分編製索引的項目，建議您建立個別的搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-234">To export only the partially indexed items for the data subject, we recommend that you create a separate search.</span></span> <span data-ttu-id="d3ce0-235">如需詳細資訊，請參閱「關於使用 DSR 案例工具的詳細資訊」一節中的[匯出部分編製索引的項目](#exporting-partially-indexed-items)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-235">For more information, see [Exporting partially indexed items](#exporting-partially-indexed-items) in the "More information about using the DSR case tool" section.</span></span>
    
    <span data-ttu-id="d3ce0-236">b.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-236">b.</span></span> <span data-ttu-id="d3ce0-237">在 **[將 Exchange 內容匯出為]** 下，選取第三個選項，亦即 **[一個包含單一資料夾中所有郵件的 PST 檔案]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-237">Under **Export Exchange content as**, select the third option, **One PST file containing all messages in a single folder**.</span></span> <span data-ttu-id="d3ce0-238">部分結果可能是針對源自另一個使用者信箱的項目，因此此選項只會列出單一資料夾中的項目，而不會指出實際信箱，而且將是您按照下一個項目中的建議，對結果進行重複資料刪除時的最佳選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-238">Because some of the results may be for items that originated in another user's mailbox, this option just lists the item in a single folder without indicating the actual mailbox and is the best option to use when you de-duplicate the results as recommended in the next item.</span></span> <span data-ttu-id="d3ce0-239">此選項也可讓資料主體按時間順序 (項目會依傳送日期排序) 檢閱項目，而不需要瀏覽每個項目的原始信箱資料夾結構。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-239">This option also lets the data subject review items in chronological order (items are sorted by sent date) without having to navigate the original mailbox folder structure for each item.</span></span>
    
    <span data-ttu-id="d3ce0-240">c.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-240">c.</span></span> <span data-ttu-id="d3ce0-241">選取 **[啟用重復資料刪除]** 選項，以排除重複的電子郵件訊息。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-241">Select **Enable de-duplication** option to excludes duplicate email messages.</span></span> <span data-ttu-id="d3ce0-242">建議您使用此選項，因為內建搜尋會搜尋您組織中的所有信箱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-242">We recommend this option because the built-in search searches all mailboxes in your organization.</span></span> <span data-ttu-id="d3ce0-243">因此，如果在搜尋的信箱中找到同一封郵件的多個複本，則此選項表示只會匯出一封郵件的一個複本。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-243">So if multiple copies of the same message are found in the mailboxes that were searched, this option means that only one copy of a message will be exported.</span></span> <span data-ttu-id="d3ce0-244">此選項會一起匯出單一資料夾中一個 PST 檔案中的郵件，為 DSR 匯出要求提供最佳使用者體驗。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-244">This option, together will exporting messages in one PST file in a single folder, results in the best user experience for DSR export requests.</span></span> <span data-ttu-id="d3ce0-245">Results.csv 匯出報告會列出找到的重複郵件的所有位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-245">The Results.csv export report lists all locations where duplicate messages were found.</span></span>
    
    <span data-ttu-id="d3ce0-246">或者，您可以選取 **[包含 SharePoint 文件版本]** 選項，以匯出所有版本的 SharePoint 和 OneDrive 文件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-246">Optionally, you can select **Include versions for SharePoint documents** option to export all versions of SharePoint and OneDrive documents.</span></span> <span data-ttu-id="d3ce0-247">這需要開啟文件庫的版本設定。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-247">This requires that versioning is turned on for document libraries.</span></span> <span data-ttu-id="d3ce0-248">此選項有助於確保匯出所有相關資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-248">This option helps to ensure that all relevant data is exported.</span></span>
    
5. <span data-ttu-id="d3ce0-249">選擇匯出設定之後，按一下 **[匯出]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-249">After you choose the export settings, click **Export**.</span></span>
    
    <span data-ttu-id="d3ce0-250">系統會準備要下載的搜尋結果，也就是說，這些搜尋結果會上傳至 Microsoft 雲端中您組織的 Azure 儲存體區域。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-250">The search results are prepared for downloading, which means they're uploaded to the Azure Storage area for your organization in the Microsoft cloud.</span></span> <span data-ttu-id="d3ce0-251">接下來的步驟會示範如何將此資料下載到您的本機電腦。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-251">The next steps show you how to download this data to your local computer.</span></span>
    
6. <span data-ttu-id="d3ce0-252">按一下 **[匯出]** 索引標籤以顯示您建立的匯出工作。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-252">Click the **Export** tab to display the export job you created.</span></span> <span data-ttu-id="d3ce0-253">匯出工作的名稱與對應的搜尋相同，並在搜尋名稱的結尾附加 **_Export**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-253">Export jobs have the same name as the corresponding search with **_Export** appended to the end of search name.</span></span> 
    
7. <span data-ttu-id="d3ce0-254">按一下您剛建立的匯出工作以顯示 [匯出] 飛出視窗頁面。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-254">Click the export job that you just created to display the export flyout page.</span></span> <span data-ttu-id="d3ce0-255">此頁面會顯示搜尋的相關資訊，例如，要匯出的項目的大小和總數，以及已轉移到 Azure 儲存體區域的項目的百分比。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-255">This page shows information about the search, such as the size and total number of items to be exported, and the percentage of the items that have been transferred to an Azure storage area.</span></span> <span data-ttu-id="d3ce0-256">按一下 **[重新整理]** 以更新上傳狀態資訊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-256">Click **Refresh** to update the upload status information.</span></span> 
    
8. <span data-ttu-id="d3ce0-257">在 **[匯出金鑰]** 下，按一下 **[複製到剪貼簿]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-257">Under **Export key**, click **Copy to clipboard**.</span></span> <span data-ttu-id="d3ce0-258">您要使用步驟 11 中的這個金鑰下載搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-258">You use this key in step 11 to download the search results.</span></span>
    
9. <span data-ttu-id="d3ce0-259">按一下 [匯出] 飛出視窗頁面頂端的 ![[匯出搜尋結果圖示]](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **[下載結果]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-259">Click ![Export search results icon](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **Download results** at the top of the export flyout page.</span></span> 
    
10. <span data-ttu-id="d3ce0-260">在頁面底部的快顯視窗中，按一下 **[開啟]** 以開啟 **[電子文件探索匯出工具]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-260">In the pop-up window at the bottom of the page, click **Open** to open the **eDiscovery Export Tool**.</span></span> <span data-ttu-id="d3ce0-261">當您第一次下載搜尋結果時，將會安裝 **[電子文件探索匯出工具]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-261">The **eDiscovery Export Tool** will be installed the first time you download search results.</span></span> 
    
11. <span data-ttu-id="d3ce0-262">在 **[電子文件探索匯出工具]** 中，於適當的方塊中貼上您在步驟 8 中複製的匯出金鑰。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-262">In the **eDiscovery Export Tool**, paste the export key that you copied in step 8 in the appropriate box.</span></span>
    
12. <span data-ttu-id="d3ce0-263">按一下 **[瀏覽]** 以指定搜尋結果檔案要下載到的位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-263">Click **Browse** to specify the location where you want to download the search result files.</span></span> 
    
    > [!NOTE]
    > <span data-ttu-id="d3ce0-264">由於大量的磁碟活動 (讀取和寫入) 的緣故，您應該將搜尋結果下載至本機磁碟機。請勿將搜尋結果下載到對應的網路磁碟機或其他網路位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-264">Due to the high amount of disk activity (reads and writes), you should download search results to a local disk drive; don't download them to a mapped network drive or other network location.</span></span> 
  
13. <span data-ttu-id="d3ce0-265">按一下 **[開始]** 將搜尋結果下載至您的電腦。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-265">Click **Start** to download the search results to your computer.</span></span> 
    
    <span data-ttu-id="d3ce0-266">**[電子文件探索匯出工具]** 會顯示匯出程序的相關狀態資訊，包括待下載剩餘項目的估計數目 (和大小)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-266">The **eDiscovery Export Tool** displays status information about the export process, including an estimate of the number (and size) of the remaining items to be downloaded.</span></span> <span data-ttu-id="d3ce0-267">匯出程序完成後，您可以在下載位置存取這些檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-267">When the export process is complete, you can access the files in the location where they were downloaded.</span></span> <span data-ttu-id="d3ce0-268">如需有關下載內容搜尋結果時包含之報告的詳細資訊，請參閱「匯出內容搜尋結果」中的[詳細資訊](/microsoft-365/compliance/export-search-results#more-information)一節。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-268">For more information about the reports that included when you download Content Search results, see the [More information](/microsoft-365/compliance/export-search-results#more-information) section in "Export Content Search results".</span></span> 
    
<span data-ttu-id="d3ce0-269">資料匯出之後，搜尋結果和匯出報告會位於與 DSR 案例名稱相同的資料夾中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-269">After the data is exported, the search results and export reports are located in a folder that has the same name as the DSR case.</span></span> <span data-ttu-id="d3ce0-270">包含信箱項目的 PST 檔案位於名為 **Exchange** 的子資料夾中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-270">The PST files that contain mailbox items are located in a subfolder named **Exchange**.</span></span> <span data-ttu-id="d3ce0-271">來自網站的文件和其他項目位於名為 **SharePoint** 的子資料夾中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-271">Documents and other items from sites are located in a subfolder named **SharePoint**.</span></span> 
  
## <a name="optional-step-5-revise-the-built-in-search-query"></a><span data-ttu-id="d3ce0-272">(選擇性) 步驟 5：修改內建搜尋查詢</span><span class="sxs-lookup"><span data-stu-id="d3ce0-272">(Optional) Step 5: Revise the built-in search query</span></span>

<span data-ttu-id="d3ce0-273">執行內建搜尋之後，您可以加以修改以縮小範圍，傳回更少的搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-273">After you run the built-in search, you can revise it to narrow the scope to return fewer search results.</span></span> <span data-ttu-id="d3ce0-274">您可以將條件新增至查詢，以執行這項操作。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-274">You can do this by adding conditions to the query.</span></span> <span data-ttu-id="d3ce0-275">系統會使用 **AND** 運算子，將條件以邏輯方式連接至關鍵字查詢。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-275">A condition is logically connected to the keyword query by the **AND** operator.</span></span> <span data-ttu-id="d3ce0-276">這表示若要在搜尋結果中傳回，項目必須同時滿足關鍵字查詢以及您新增的任何條件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-276">That means to be returned in the search results, items must satisfy both the keyword query and any conditions you add.</span></span> <span data-ttu-id="d3ce0-277">這是條件協助縮小搜尋結果範圍的方式。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-277">This is how conditions help to narrow the results.</span></span> <span data-ttu-id="d3ce0-278">如果您將兩個或多個的獨特條件新增至搜尋查詢 (指定不同屬性的條件)，則會使用 **AND** 運算子，以邏輯方式連接這些條件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-278">If you add two or more unique conditions to a search query (conditions that specify different properties), those conditions are logically connected by the **AND** operator.</span></span> <span data-ttu-id="d3ce0-279">這表示只會傳回滿足所有條件 (除了關鍵字查詢之外) 的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-279">That means only items that satisfy all the conditions (in addition to the keyword query) are returned.</span></span> <span data-ttu-id="d3ce0-280">如果您將多個值 (以逗號或分號分隔) 加入至單一條件，這些值會以 **OR** 運算子連接。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-280">If you add multiple values (separated by commas or semi-colons) to a single condition, those values are connected by the **OR** operator.</span></span> <span data-ttu-id="d3ce0-281">這表示如果項目在條件中包含任何指定的屬性值，則會傳回項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-281">That means items are returned if they contain any of the specified values for the property in the condition.</span></span> 
  
<span data-ttu-id="d3ce0-282">以下是一些您可以新增到 DSR 案例內建搜尋查詢的條件範例。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-282">Here are some examples of the conditions that you can add to the built-in search query of a DSR case.</span></span> <span data-ttu-id="d3ce0-283">搜尋查詢中使用的實際屬性名稱會顯示在括號中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-283">The name of the actual property used in a search query is shown parentheses.</span></span>
  
- <span data-ttu-id="d3ce0-284">**檔案類型 ( `filetype`)** – 指定文件或檔案的副檔名。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-284">**File type ( `filetype`)** – Specifies the extension of a document or file.</span></span> <span data-ttu-id="d3ce0-285">使用此條件搜尋特定 Office 應用程式 (例如 Word、Excel 和 OneNote) 所建立的文件和檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-285">Use this condition to search for documents and files created by specific Office applications, such as Word, Excel, and OneNote.</span></span> 
    
- <span data-ttu-id="d3ce0-286">**郵件類型 ( `kind`)** - 指定要搜尋的電子郵件項目的類型。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-286">**Message type ( `kind`)** – Specifies the type of email item to search for.</span></span> <span data-ttu-id="d3ce0-287">例如，您可以使用語法 `kind:email OR kind:im`，僅傳回 Microsoft Teams 中的電子郵件訊息和商務用 Skype 交談或一對一聊天。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-287">For example, you can use the syntax  `kind:email OR kind:im` to return only email messages and Skype for Business conversations or one-to-one chats in Microsoft Teams.</span></span> 
    
- <span data-ttu-id="d3ce0-288">**合規性標籤 (`compliancetag`)** - 指定指派給電子郵件訊息或文件的標籤。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-288">**Compliance tag (`compliancetag`)** – Specifies a label assigned to an email message or a document.</span></span> <span data-ttu-id="d3ce0-289">此條件會傳回以特定標籤分類的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-289">This condition returns items that are classified with a specific label.</span></span> <span data-ttu-id="d3ce0-290">標籤是用來分類電子郵件和文件，以進行資料控管，並根據標籤定義的分類，強制執行保留規則。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-290">Labels are used to classify email and documents for data governance and enforce retention rules based on the classification defined by the label.</span></span> <span data-ttu-id="d3ce0-291">這是對 DSR 調查很有用的條件，因為組織可能會使用標籤來分類與資料隱私權相關的內容，或含有個人資料或敏感性資訊的內容。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-291">This is a useful condition for DSR investigations because your organization may be using labels to classify content related to data privacy or that contains personal data or sensitive information.</span></span> <span data-ttu-id="d3ce0-292">針對此條件的值，請使用完整的標籤名稱或標籤名稱的第一部分與萬用字元。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-292">For the value of this condition, use the complete label name or the first part of the label name with a wildcard.</span></span> <span data-ttu-id="d3ce0-293">如需詳細資訊，請參閱[了解 Office 365 中的保留原則和保留標籤](/microsoft-365/compliance/retention)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-293">For more information, see [Learn about retention policies and retention labels in Office 365](/microsoft-365/compliance/retention).</span></span>
    
<span data-ttu-id="d3ce0-294">如需 DSR 案例中可用的所有條件的清單和描述，請參閱「內容搜尋的關鍵字查詢和搜尋條件」一文中的[搜尋條件](/microsoft-365/compliance/keyword-queries-and-search-conditions#search-conditions)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-294">For a list and description of all the conditions available in the DSR case tool, see [Search conditions](/microsoft-365/compliance/keyword-queries-and-search-conditions#search-conditions) in the "Keyword queries and search conditions for Content Search" article.</span></span> 
  
### <a name="changing-the-content-locations-that-are-searched"></a><span data-ttu-id="d3ce0-295">變更搜尋的內容位置</span><span class="sxs-lookup"><span data-stu-id="d3ce0-295">Changing the content locations that are searched</span></span>

<span data-ttu-id="d3ce0-296">除了修改 DSR 案例的內建搜尋之外，您也可以變更搜尋的內容位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-296">In addition to revising the built-in search for a DSR case, you can also change the content locations that are searched.</span></span> <span data-ttu-id="d3ce0-297">如先前所說明，內建搜尋會搜尋組織中的每個信箱和網站，以及任何 Exchange Online 公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-297">As previously explained, the built-in search searches every mailbox and site in the organization, and any Exchange Online public folders.</span></span> <span data-ttu-id="d3ce0-298">例如，您可以縮小搜尋範圍，只搜尋資料主體的信箱和 OneDrive 帳戶，以及選取的 SharePoint 網站。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-298">For example, you could narrow the search to only search the data subject's mailbox and OneDrive account and selected SharePoint sites.</span></span> <span data-ttu-id="d3ce0-299">如果您選擇搜尋特定網站，您必須新增要搜尋的每個網站。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-299">If you choose to search specific sites, you have to add each site that you want to search.</span></span>
  
<span data-ttu-id="d3ce0-300">若要修改要搜尋的內容位置：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-300">To modify the content locations to search:</span></span>
  
1. <span data-ttu-id="d3ce0-301">開啟您想要為其變更內容位置的內建搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-301">Open the built-in search that you want to change the content locations for.</span></span>
    
2. <span data-ttu-id="d3ce0-302">在搜尋查詢的 **[位置]** 下，按一下 **[特定位置]** 旁的 **[修改]** 選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-302">In the search query, under **Locations**, click **Modify** next to the **Specific locations** option.</span></span> 
    
    ![按一下 [修改] 以變更內建搜尋查詢的內容位置](../media/d66f7ba7-b71f-4ff5-a030-460ff02e3123.png)
  
    <span data-ttu-id="d3ce0-304">**[修改位置]** 飛出視窗頁面隨即顯示。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-304">The **Modify locations** flyout page is displayed.</span></span> <span data-ttu-id="d3ce0-305">以下是內建搜尋中內容位置的描述，以及修改搜尋位置的一些相關資訊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-305">Here's a description of the content locations in the built-in search and some information about modifying the locations that are searched.</span></span> 
    
    ![修改位置飛出視窗頁面](../media/56c033f6-6735-46ba-abb2-a263a2b79836.png)
  
    <span data-ttu-id="d3ce0-307">a.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-307">a.</span></span> <span data-ttu-id="d3ce0-308">在飛出視窗頁面頂端的信箱區段中，選取 **[全選]** 底下的切換開關，這表示搜尋所有信箱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-308">The toggle under **Select all** in mailbox section at the top of the flyout page is selected, which indicates that all mailboxes are searched.</span></span> <span data-ttu-id="d3ce0-309">若要縮小搜尋範圍，按一下切換開關以取消選取它，然後按一下 **[選擇使用者、群組或小組]**，然後選擇要搜尋的特定信箱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-309">To narrow the scope of the search, click the toggle to unselect it, and then click **Choose users, groups, or teams** and choose specific mailboxes to search.</span></span>
    
    <span data-ttu-id="d3ce0-310">b.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-310">b.</span></span> <span data-ttu-id="d3ce0-311">在飛出視窗頁面中間的網站區段中，選取 **[全選]** 底下的切換開關，這表示搜尋所有網站。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-311">The toggle under **Select all** in the sites section in the middle of the flyout page is selected, which indicates that all sites are searched.</span></span> <span data-ttu-id="d3ce0-312">若要將搜尋範圍縮小到選取的網站，您可以取消選取切換開關，然後按一下 **[選擇網站]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-312">To narrow the search to selected sites, you would unselect the toggle and then click **Choose sites**.</span></span> <span data-ttu-id="d3ce0-313">您必須新增要搜尋的每個特定網站，包括資料主體的 OneDrive 帳戶。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-313">You have to add each specific site that you want to search, including the data subject's OneDrive account.</span></span>
    
    <span data-ttu-id="d3ce0-314">c.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-314">c.</span></span> <span data-ttu-id="d3ce0-315">選取 Exchange 公用資料夾區段中的切換開關，這表示搜尋所有 Exchange 公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-315">The toggle in the Exchange public folders section is selected, which means all Exchange public folders are searched.</span></span> <span data-ttu-id="d3ce0-316">您只能搜尋所有 Exchange 公用資料夾或完全不搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-316">You can only search all Exchange public folders or none of them.</span></span> <span data-ttu-id="d3ce0-317">您無法選擇要搜尋的特定資料夾。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-317">You can't choose specific ones to search.</span></span>
    
3. <span data-ttu-id="d3ce0-318">如果您在內建搜尋中修改內容位置，請按一下 **[儲存 &amp; 執行]** 以重新開始搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-318">If you modify the content locations in the built-in search, click **Save &amp; run** to restart the search.</span></span> 

> [!NOTE]
> <span data-ttu-id="d3ce0-319">如果您搜尋所有信箱位置或只搜尋特定信箱，當您匯出搜尋的結果時，會包含來自其他 Office 365 應用程式且儲存到使用者信箱的資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-319">When you search all mailbox locations or just specific mailboxes, data from other Office 365 applications that's saved to user mailboxes is included when you export the results of the search.</span></span> <span data-ttu-id="d3ce0-320">此資料不會包含在估計的搜尋結果中，並且無法提供預覽。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-320">This data won't be included in the estimated search results and isn't available for preview.</span></span> <span data-ttu-id="d3ce0-321">但是當您匯出並下載搜尋結果時，該資料會包含在內。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-321">But it's included when you export and download the search results.</span></span> <span data-ttu-id="d3ce0-322">如需有關將資料儲存在使用者信箱中的應用程式的詳細資訊，請參閱[儲存在 Exchange Online 信箱中的內容](/microsoft-365/compliance/what-is-stored-in-exo-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-322">For more information the applications that store data in a user's mailbox, see [Content stored in Exchange Online mailboxes](/microsoft-365/compliance/what-is-stored-in-exo-mailbox).</span></span>
  
## <a name="more-information-about-using-the-dsr-case-tool"></a><span data-ttu-id="d3ce0-323">關於使用 DSR 案例工具的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="d3ce0-323">More information about using the DSR case tool</span></span>

<span data-ttu-id="d3ce0-324">以下幾節包含使用 DSR 案例工具回應 DSR 匯出要求的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-324">The following sections contain more information about using the DSR case tool to respond to DSR export requests.</span></span>
  
[<span data-ttu-id="d3ce0-325">從 Office 漫遊服務匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-325">Exporting data from the Office Roaming Service</span></span>](#exporting-data-from-the-office-roaming-service)

[<span data-ttu-id="d3ce0-326">匯出部分編製索引的項目</span><span class="sxs-lookup"><span data-stu-id="d3ce0-326">Exporting partially indexed items</span></span>](#exporting-partially-indexed-items)

[<span data-ttu-id="d3ce0-327">從 Microsoft Teams 和 Microsoft 365 群組搜尋及匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-327">Searching and exporting data from Microsoft Teams and Microsoft 365 Groups</span></span>](#searching-and-exporting-data-from-microsoft-teams-and-microsoft-365-groups)

[<span data-ttu-id="d3ce0-328">搜尋 Exchange 公用資料夾</span><span class="sxs-lookup"><span data-stu-id="d3ce0-328">Searching Exchange public folders</span></span>](#searching-exchange-public-folders)
  
### <a name="exporting-data-from-the-office-roaming-service"></a><span data-ttu-id="d3ce0-329">從 Office 漫遊服務匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-329">Exporting data from the Office Roaming Service</span></span>

<span data-ttu-id="d3ce0-330">您可以使用 DSR 案例工具搜尋及匯出 Office 漫遊服務所產生的使用狀況資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-330">You can use the DSR case tool to search for and export usage data that's generated by the Office Roaming Service.</span></span> <span data-ttu-id="d3ce0-331">漫遊是一項服務，可儲存 Office 相關設定，例如 Office 佈景主題、自訂字典、語言設定、開發人員模式和自動校正。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-331">Roaming is a service that stores Office-related settings, such as Office theme, custom dictionary, language settings, developer mode, and auto correct.</span></span> 
    
<span data-ttu-id="d3ce0-332">Office 漫遊服務的資料會儲存在資料主體的信箱中，位於 Exchange Online 信箱個人往來之間郵件 (非 IPM) 樹狀子目錄中的隱藏資料夾中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-332">The data from the Office Roaming service is stored in a data subject's mailbox in a hidden folder located in a non-interpersonal message (non-IPM) subtree of Exchange Online mailboxes.</span></span> <span data-ttu-id="d3ce0-333">這表示當使用者使用 Outlook 或其他郵件用戶端存取其信箱時，使用者看不到該資料。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-333">This means that the data is hidden from the user's view when they use Outlook or other mail clients to access their mailbox.</span></span> <span data-ttu-id="d3ce0-334">如需有關隱藏資料夾的詳細資訊，請參閱 [MAPI 隱藏資料夾](https://go.microsoft.com/fwlink/?linkid=872758)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-334">For more information about hidden folders, see [MAPI Hidden Folders](https://go.microsoft.com/fwlink/?linkid=872758).</span></span>
  
<span data-ttu-id="d3ce0-335">您可以建立能夠在資料主體的信箱中傳回 Office 漫遊服務使用狀況資料的個別內容搜尋 (並將其與 DSR 案例建立關聯)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-335">You can create a separate content search (and associate it with a DSR case) that returns the Office Roaming Service usage data in the data subject's mailbox.</span></span> <span data-ttu-id="d3ce0-336">此資料不包含在搜尋統計資料中，且無法預覽。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-336">This data isn't included in the search statistics and it won't be available for preview.</span></span> <span data-ttu-id="d3ce0-337">但您可以匯出資料，然後將其提供給資料主體，以回應 DSR 匯出要求。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-337">But you can export it and then give it to the data subject in response to a DSR export request.</span></span>
  
<span data-ttu-id="d3ce0-338">當您從 Office 漫遊服務匯出資料時，資料會儲存到位於 **ApplicationDataRoot** 資料夾中的個別資料夾，該資料夾位於名稱為資料主體電子郵件地址的資料夾下。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-338">When you export data from the Office Roaming Service, the data is saved to a separate folder that's located in the **ApplicationDataRoot** folder, which is under a folder that is name with the data subject's email address.</span></span> <span data-ttu-id="d3ce0-339">此資料會匯出為 JSON 檔案，這是附加到電子郵件訊息的人類可讀取文字檔，類似 XML 或 TXT 檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-339">This data is exported as JSON files, which are human-readable text files similar to XML or TXT files, that are attached to email messages.</span></span> <span data-ttu-id="d3ce0-340">目前，此資料夾是以全域唯一識別碼 (GUID) 命名：**1caee58f-eb14-4a6b-9339-1fe2ddf6692b**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-340">Currently, this folder is named with the globally unique identifier (GUID): **1caee58f-eb14-4a6b-9339-1fe2ddf6692b**.</span></span> <span data-ttu-id="d3ce0-341">在之後版本的 DSR 案例工具中，GUID 將會取代為實際應用程式的名稱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-341">In future versions of the DSR case tool, the GUID will be replaced with the name of the actual application.</span></span> 

   
 <span data-ttu-id="d3ce0-342">**若要搜尋及匯出 Office 漫遊服務資料：**</span><span class="sxs-lookup"><span data-stu-id="d3ce0-342">**To search for and export Office Roaming Service data:**</span></span>
  
1. <span data-ttu-id="d3ce0-343">在安全性與合規性中心，按一下 **[資料隱私權]** \> **[資料主體要求]**，然後針對您要為其匯出使用狀況資料的資料主體，按一下其 DSR 案例旁的 **[開啟]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-343">In the Security & Compliance Center, click **Data privacy** \> **Data subject requests**, and then click **Open** next to the DSR case for the data subject that you want to export usage data for.</span></span> 
    
2. <span data-ttu-id="d3ce0-344">按一下頁面頂端的 **[搜尋]** 索引標籤，然後按一下 ![[新增圖示]](../media/ITPro-EAC-AddIcon.gif) **[引導式搜尋]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-344">Click the **Search** tab at the top of the page, and then click ![Add Icon](../media/ITPro-EAC-AddIcon.gif) **Guided search**.</span></span>
    
3. <span data-ttu-id="d3ce0-345">按一下 **[命名您的搜尋]** 頁面上的 **[取消]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-345">Click **Cancel** on the **Name your search** page.</span></span> 
    
4. <span data-ttu-id="d3ce0-346">在 **[搜尋查詢]** 底下的 **[類型]** 條件中，選取 **[Office 漫遊服務]** 旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-346">Under **Search query**, in the **Type** condition, select the check box next to **Office Roaming Service**.</span></span> 
    
    ![選取 [Office 漫遊服務] 核取方塊以匯出使用狀況資料](../media/O365_DSRCase_SDSDataExport1.png)
  
    <span data-ttu-id="d3ce0-348">**[類型]** 條件 (即電子郵件訊息類別) 應該是搜尋查詢中唯一的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-348">The **Type** condition (which are email message classes) should be the only item in the search query.</span></span> <span data-ttu-id="d3ce0-349">您可以刪除 **[關鍵字]** 方塊或將其留空。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-349">You can delete the **Keywords** box or leave it blank.</span></span> 
    
5. <span data-ttu-id="d3ce0-350">在 **[位置]** 下，確認已選取 **[特定位置]**，然後按一下 **[修改]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-350">Under **Locations**, make sure that **Specific locations** is selected, and then click **Modify**.</span></span>
    
6. <span data-ttu-id="d3ce0-351">在 **[修改位置]** 飛出視窗頁面的上半部 (信箱區段)，按一下 **[選擇使用者、群組或小組]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-351">On top part of the **Modify locations** flyout page (the mailbox section), click **Choose users, groups, or teams**.</span></span>
    
7. <span data-ttu-id="d3ce0-352">在 **[編輯位置]** 頁面上，按一下 **[選擇使用者、群組或小組]**、選擇資料主體的信箱，然後儲存您的選取項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-352">On the **Edit locations** page, click **Choose users, groups, or teams**, choose the data subject's mailbox, and then save your selection.</span></span> 
    
8. <span data-ttu-id="d3ce0-353">按一下 **[儲存並執行]**，然後為搜尋命名並加以儲存。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-353">Click **Save & run**, and then name the search and save it.</span></span>
    
    <span data-ttu-id="d3ce0-354">搜尋隨即開始。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-354">The search is started.</span></span>
    
 <span data-ttu-id="d3ce0-355">**若要匯出 Office 漫遊服務資料：**</span><span class="sxs-lookup"><span data-stu-id="d3ce0-355">**To export Office Roaming Service data:**</span></span>
  
1. <span data-ttu-id="d3ce0-356">完成您在上一個步驟中建立的搜尋後，按一下頁面頂端的 **[搜尋]** 索引標籤，然後按一下搜尋旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-356">When the search that you created in the previous step is complete, click the **Search** tab at the top of the page, and then click the checkbox next to the search.</span></span> <span data-ttu-id="d3ce0-357">您可能需要按一下 ![[重新整理]](../media/165fb3ad-38a8-4dd9-9e76-296aefd96334.png) **[重新整理]**，才能顯示搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-357">You may have to click ![Refresh](../media/165fb3ad-38a8-4dd9-9e76-296aefd96334.png) **Refresh** to display the search.</span></span> 
    
2. <span data-ttu-id="d3ce0-358">在 [搜尋] 飛出視窗頁面上，按一下 ![[匯出搜尋結果圖示]](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **[其他]**，然後從下拉式清單選取 **[匯出結果]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-358">On the search flyout page, click ![Export search results icon](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **More**, and then select **Export results** from the drop-down list.</span></span> 
    
3. <span data-ttu-id="d3ce0-359">在 **[匯出結果]** 頁面上，選取匯出使用狀況資料的建議選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-359">On the **Export results** page, select the recommended options to export usage data.</span></span> 
    
    ![匯出 Office 漫遊服務使用狀況資料時匯出選項](../media/470a7d1e-eeae-4b42-95aa-15cb82ce2f68.png)
  
    <span data-ttu-id="d3ce0-361">a.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-361">a.</span></span> <span data-ttu-id="d3ce0-362">在 **[輸出選項]** 下，選取第一個選項 (**[所有項目，但不包含格式無法辨識的項目、已加密或因其他原因而未編製索引的項目]**)，以便僅匯出已編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-362">Under **Output options**, select the first option (**All items, excluding ones that have ones that have an unrecognized format, are encrypted, or weren't indexed for other reasons**) to export indexed items only.</span></span>
    
    <span data-ttu-id="d3ce0-363">b.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-363">b.</span></span> <span data-ttu-id="d3ce0-364">在 **[將 Exchange 內容匯出為]** 下，選取第二個選項，亦即 **[一個包含所有郵件的 PST 檔案]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-364">Under **Export Exchange content as**, select the second option, **One PST file containing all messages**.</span></span>
    
    <span data-ttu-id="d3ce0-365">c.</span><span class="sxs-lookup"><span data-stu-id="d3ce0-365">c.</span></span> <span data-ttu-id="d3ce0-366">維持不選取其餘的匯出選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-366">Leave the remaining export options unselected.</span></span>
    
4. <span data-ttu-id="d3ce0-367">選擇匯出設定之後，按一下 **[匯出]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-367">After you choose the export settings, click **Export**.</span></span>
    
    <span data-ttu-id="d3ce0-368">系統會準備要下載的搜尋結果，也就是說，這些搜尋結果會上傳至 Microsoft 雲端中您組織的 Azure 儲存體區域。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-368">The search results are prepared for downloading, which means they're uploaded to the Azure storage area for your organization in the Microsoft cloud.</span></span> <span data-ttu-id="d3ce0-369">接下來的步驟會示範如何將此資料下載到您的本機電腦。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-369">The next steps show you how to download this data to your local computer.</span></span>
    
5. <span data-ttu-id="d3ce0-370">按一下 **[匯出]** 索引標籤以顯示您建立的匯出工作。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-370">Click the **Export** tab to display the export job you created.</span></span> <span data-ttu-id="d3ce0-371">匯出工作的名稱與對應的搜尋相同，並在搜尋名稱的結尾附加 **_Export**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-371">The export jobs have the same name as the corresponding search with **_Export** appended to the end of search name.</span></span> 
    
6. <span data-ttu-id="d3ce0-372">按一下您剛建立的匯出工作以顯示 [匯出] 飛出視窗頁面。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-372">Click the export job that you just created to display the export flyout page.</span></span> 
    
7. <span data-ttu-id="d3ce0-373">在 **[匯出金鑰]** 下，按一下 **[複製到剪貼簿]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-373">Under **Export key**, click **Copy to clipboard**.</span></span> <span data-ttu-id="d3ce0-374">您要使用步驟 10 中的這個金鑰下載搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-374">You use this key in step 10 to download the search results.</span></span>
    
8. <span data-ttu-id="d3ce0-375">按一下 [匯出] 飛出視窗頁面頂端的 ![[匯出搜尋結果圖示]](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **[下載結果]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-375">Click ![Export search results icon](../media/47205c65-babd-4b3a-bd7b-98dfd92883ba.png) **Download results** at the top of the export flyout page.</span></span> 
    
9. <span data-ttu-id="d3ce0-376">在頁面底部的快顯視窗中，按一下 **[開啟]** 以開啟 **[電子文件探索匯出工具]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-376">In the pop-up window at the bottom of the page, click **Open** to open the **eDiscovery Export Tool**.</span></span> <span data-ttu-id="d3ce0-377">當您第一次下載搜尋結果時，將會安裝 **[電子文件探索匯出工具]**。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-377">The **eDiscovery Export Tool** will be installed the first time you download search results.</span></span> 
    
10. <span data-ttu-id="d3ce0-378">在 [電子文件探索匯出工具] 中，於適當的方塊中貼上您在步驟 7 中所複製的匯出金鑰。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-378">In the **eDiscovery Export Tool**, paste the export key that you copied in step 7 in the appropriate box.</span></span>
    
11. <span data-ttu-id="d3ce0-379">按一下 [瀏覽] 以指定搜尋結果檔案要下載到的位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-379">Click **Browse** to specify the location where you want to download the search result files.</span></span> 
    
    > [!NOTE]
    > <span data-ttu-id="d3ce0-380">由於大量的磁碟活動 (讀取和寫入) 的緣故，您應該將搜尋結果下載至本機磁碟機。請勿將搜尋結果下載到對應的網路磁碟機或其他網路位置。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-380">Due to the high amount of disk activity (reads and writes), you should download search results to a local disk drive; don't download them to a mapped network drive or other network location.</span></span> 
  
12. <span data-ttu-id="d3ce0-381">按一下 **[開始]** 將搜尋結果下載至您的電腦。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-381">Click **Start** to download the search results to your computer.</span></span> 
    
    <span data-ttu-id="d3ce0-382">**[電子文件探索匯出工具]** 會顯示匯出程序的相關狀態資訊，包括待下載剩餘項目的估計數目 (和大小)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-382">The **eDiscovery Export Tool** displays status information about the export process, including an estimate of the number (and size) of the remaining items to be downloaded.</span></span> <span data-ttu-id="d3ce0-383">匯出程式完成後，您可以在 Outlook 中開啟 Exchange PST 檔案，然後前往 **ApplicationDataRoot** 資料夾，存取漫遊服務的子資料夾。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-383">When the export process is complete, you can open the Exchange PST file in Outlook and then go to the **ApplicationDataRoot** folder to access the subfolder for the Roaming service.</span></span> 
    
    <span data-ttu-id="d3ce0-384">如先前所說明，包含使用狀況資料的 JSON 檔案會附加到郵件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-384">As previously explained, the JSON files that contain usage data are attached to messages.</span></span> <span data-ttu-id="d3ce0-385">若要檢視 JSON 檔案，請按一下該郵件，然後開啟附加的 JSON 檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-385">To view a JSON file, click a message and then open the attached JSON file.</span></span> 
  
### <a name="exporting-partially-indexed-items"></a><span data-ttu-id="d3ce0-386">匯出部分編製索引的項目</span><span class="sxs-lookup"><span data-stu-id="d3ce0-386">Exporting partially indexed items</span></span>

<span data-ttu-id="d3ce0-387">建議您不要從建立 DSR 案例時所建立的內建搜尋中，匯出部分編製索引的項目 (也稱為未編製索引的項目)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-387">We recommend that you don't export partially indexed items (also called unindexed items) from the built-in search that's created when you create a DSR case.</span></span> <span data-ttu-id="d3ce0-388">這是因為搜尋結果很可能會包含組織中其他使用者的部分編製索引的項目，而不只是資料主體的部分編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-388">That's because the search results will more than likely include partially indexed items for other users in your organization, and not just partially indexed items for the data subject).</span></span> <span data-ttu-id="d3ce0-389">但是，建議您建立與 DSR 案例相關聯的個別內容搜尋，其設計目的是只匯出與資料主體相關的部分編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-389">Instead, we recommend that you create a separate Content Search that's associated with the DSR case that's designed to export only the partially indexed items related to the data subject.</span></span> 
  
<span data-ttu-id="d3ce0-390">以下是匯出部分編製索引的項目的高層級程序。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-390">Here's a high-level process to export partially indexed items.</span></span> <span data-ttu-id="d3ce0-391">匯出之後，您可以檢閱這些項目，以判斷項目是否回應 DSR 存取或匯出要求。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-391">After they're export, you can review them to determine if an item is responsive to a DSR access or export request.</span></span>
  
1. <span data-ttu-id="d3ce0-392">開啟 DSR 案例，然後在 **[搜尋]** 頁面上建立搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-392">Open the DSR case and create a search on the **Search** page.</span></span> 
    
2. <span data-ttu-id="d3ce0-393">使用下列準則設定搜尋查詢以及要搜尋的內容位置：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-393">Use the following criteria for configuring the search query and the content locations to search:</span></span>
    
    - <span data-ttu-id="d3ce0-394">使用空的/空白關鍵字查詢。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-394">Use an empty/blank keyword query.</span></span> <span data-ttu-id="d3ce0-395">如此會傳回搜尋的內容位置中的所有項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-395">This returns all items in the content locations that are searched.</span></span>
    
    - <span data-ttu-id="d3ce0-396">只搜尋資料主體的 Exchange Online 信箱及其 OneDrive 帳戶。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-396">Search only the data subject's Exchange Online mailbox and their OneDrive account.</span></span>
    
3. <span data-ttu-id="d3ce0-397">執行搜尋並完成之後，您可以匯出並下載搜尋結果 (如[步驟 4](#step-4-export-the-data) 中所述)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-397">After you run the search and it completes, you can export and download the search results (as described in [Step 4](#step-4-export-the-data)).</span></span> <span data-ttu-id="d3ce0-398">使用下列設定匯出部分編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-398">Use the following settings to export partially indexed items.</span></span> 
    
    - <span data-ttu-id="d3ce0-399">在 **[輸出選項]** 下，選取第三個選項 (**[僅限格式無法辨識，已加密或因其他原因而未編製索引的項目]**)，以便僅匯出已編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-399">Under **Output options**, select the third option (**Only items that have an unrecognized format, are encrypted, or weren't indexed for other reasons**) to export partially indexed items only.</span></span>
    
    - <span data-ttu-id="d3ce0-400">在 **[將 Exchange 內容匯出為]** 下，您可以根據您的喜好設定，選取任何選項。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-400">Under **Export Exchange content as**, you can select any option based on your preferences.</span></span> 
    
    - <span data-ttu-id="d3ce0-401">選取 **[包含 SharePoint 文件版本]** 選項會在部分編製索引版本時匯出文件的版本。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-401">Selecting the **Include versions for SharePoint documents** option exports versions of documents if a version is partially indexed.</span></span> 
    
<span data-ttu-id="d3ce0-402">如需有關部分編製索引的項目的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-402">For more information about partially indexed items, see:</span></span> 
  
- [<span data-ttu-id="d3ce0-403">位於 Office 365 中內容搜尋的部分編製索引項目</span><span class="sxs-lookup"><span data-stu-id="d3ce0-403">Partially indexed items in Content Search in Office 365</span></span>](/microsoft-365/compliance/partially-indexed-items-in-content-search)

- [<span data-ttu-id="d3ce0-404">匯出部分編製索引的項目</span><span class="sxs-lookup"><span data-stu-id="d3ce0-404">Exporting partially indexed items</span></span>](/microsoft-365/compliance/export-search-results#exporting-partially-indexed-items)

### <a name="searching-and-exporting-data-from-microsoft-teams-and-microsoft-365-groups"></a><span data-ttu-id="d3ce0-405">從 Microsoft Teams 和 Microsoft 365 群組搜尋及匯出資料</span><span class="sxs-lookup"><span data-stu-id="d3ce0-405">Searching and exporting data from Microsoft Teams and Microsoft 365 Groups</span></span>

<span data-ttu-id="d3ce0-406">屬於 Microsoft Teams 中聊天清單的交談 (稱為 Team 聊天或一對一聊天) 會儲存在參與聊天的使用者的 Exchange Online 信箱中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-406">Conversations that are part of the Chat list in Microsoft Teams (called Team chats or one-to-one chats) are stored in the Exchange Online mailbox of the users who participate in the chats.</span></span> <span data-ttu-id="d3ce0-407">此外，人員在一對一聊天中分享的檔案會儲存在檔案共用者的 OneDrive 帳戶中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-407">Also, the files a person shares in a one-to-one chat are stored in the OneDrive account of the person who shares the file.</span></span> <span data-ttu-id="d3ce0-408">內建搜尋會搜尋組織中的所有信箱和 OneDrive 帳戶，因此 DSR 案例中的內建搜尋會傳回在聊天工作階段 (建立或上傳的資料主體) 中共用的小組聊天和文件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-408">Because the built-in search searches all mailboxes and OneDrive accounts in the organization, team chats and documents shared in a chat session (that the data subject created or uploaded) are returned by built-in search in a DSR case.</span></span>
  
<span data-ttu-id="d3ce0-409">或者，屬於 Teams 頻道一部分的交談 (也稱為頻道訊息) 會儲存在與小組相關聯的信箱中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-409">Alternatively, conversations that are part of a Teams channel (also called channel messages) are stored in the mailbox that's associated with a team.</span></span> <span data-ttu-id="d3ce0-410">內建搜尋也會傳回資料主體參與的這些交談類型，因為系統會搜尋與 Teams 相關聯的所有信箱。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-410">These types of conversations that the data subject participated in are also returned by the built-in search because all mailboxes associated with Teams are searched.</span></span> <span data-ttu-id="d3ce0-411">此外，資料主體在 Teams 頻道中共用的檔案會儲存在小組的 SharePoint 網站上。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-411">Additionally, files that a data subject shares in a Teams channel are stored on the team's SharePoint site.</span></span> <span data-ttu-id="d3ce0-412">DSR 案例中的內建搜尋會傳回資料主體所建立或上傳的檔案，因為與 Teams 相關聯的網站會包含在搜尋中。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-412">Files created or uploaded by the data subject are returned by the built-in search in a DSR case because the sites associated with Teams are included in the search.</span></span>
  
<span data-ttu-id="d3ce0-413">同樣地，內建搜尋中也會包含對應至 Microsoft 365 群組的信箱和 SharePoint 網站。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-413">Similarly, mailboxes and SharePoint sites that correspond to an Microsoft 365 Group are also included in the built-in search.</span></span> <span data-ttu-id="d3ce0-414">這表示系統會傳回資料主體所傳送或接收的電子郵件訊息，以及資料主體所建立或上傳的檔案。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-414">This means that email messages sent or received by the data subject and files created or uploaded by the data subject are returned.</span></span> 
  
<span data-ttu-id="d3ce0-415">如需有關如何使用內容搜尋來搜尋 Microsoft Teams 和 Microsoft 365 群組中的項目的詳細資訊，或者要了解如何取得成員清單，請參閱 [Microsoft 365 中的內容搜尋](/microsoft-365/compliance/content-search#searching-microsoft-teams-and-microsoft-365-groups)中的「搜尋 Microsoft Teams 和 Microsoft 365 群組」一節。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-415">For more information about using Content Search to search for items in Microsoft Teams and Microsoft 365 Groups or to see how to get a list of members, see the "Searching Microsoft Teams and Microsoft 365 Groups" section in [Content Search in Microsoft 365](/microsoft-365/compliance/content-search#searching-microsoft-teams-and-microsoft-365-groups).</span></span> 
  
### <a name="searching-exchange-public-folders"></a><span data-ttu-id="d3ce0-416">搜尋 Exchange 公用資料夾</span><span class="sxs-lookup"><span data-stu-id="d3ce0-416">Searching Exchange public folders</span></span>

<span data-ttu-id="d3ce0-417">DSR 案例中的內建搜尋只會傳回資料主體傳送至已啟用郵件功能的公用資料夾的電子郵件訊息，或其他人傳送至公用資料夾，同時也複製資料主體的郵件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-417">The built-in search in a DSR case will only return email messages that the data subject sent to a mail-enabled public folder or messages that someone else sent to a public folder and also copied the data subject.</span></span> <span data-ttu-id="d3ce0-418">它不會傳回資料主體張貼到公用資料夾的郵件。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-418">It doesn't return messages that the data subject posted to a public folder.</span></span> <span data-ttu-id="d3ce0-419">若要搜尋資料主體張貼到公用資料夾的項目，您可以建立個別的內容搜尋，此內容搜尋可搜尋資料主體張貼至公用資料夾的任何項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-419">To search for items that the data subject posted to a public folder, you can create a separate create a separate Content Search that searches for any item posted to a public folder by the data subject.</span></span>
  
<span data-ttu-id="d3ce0-420">以下是搜尋資料主體張貼到公用資料夾之項目的高層級程序。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-420">Here's a high-level process to search for items that the data subject posted to a public folder.</span></span> 
  
1. <span data-ttu-id="d3ce0-421">開啟 DSR 案例，然後在 **[搜尋]** 頁面上建立搜尋。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-421">Open the DSR case and create a search on the **Search** page.</span></span> 
    
2. <span data-ttu-id="d3ce0-422">使用下列準則設定搜尋查詢以及要搜尋的內容位置：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-422">Use the following criteria for configuring the search query and the content locations to search:</span></span>
    
  - <span data-ttu-id="d3ce0-423">在 **[關鍵字]** 方塊中，使用下列搜尋查詢：</span><span class="sxs-lookup"><span data-stu-id="d3ce0-423">In the **Keywords** box, use the following search query:</span></span> 
    
    ```powershell
    itemclass:ipm.post AND "<email address of the data subject>"
    ```

  - <span data-ttu-id="d3ce0-424">搜尋所有 Exchange 公用資料夾</span><span class="sxs-lookup"><span data-stu-id="d3ce0-424">Search all Exchange public folders</span></span>
    
  - <span data-ttu-id="d3ce0-425">執行搜尋並完成之後，您可以匯出並下載搜尋結果 (如[步驟 4](#step-4-export-the-data) 中所述)。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-425">After you run the search and it completes, you can export and download the search results (as described in [Step 4](#step-4-export-the-data)).</span></span> <span data-ttu-id="d3ce0-426">使用下列設定匯出部分編製索引的項目。</span><span class="sxs-lookup"><span data-stu-id="d3ce0-426">Use the following settings to export partially indexed items.</span></span> 
