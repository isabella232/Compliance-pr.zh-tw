---
title: 適用於 Project Server 的 GDPR
description: 瞭解如何解決內部部署 Project Server 中的一般資料保護規定 (GDPR) 需求。
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Priority
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-apr2020
ms.collection: MS-Compliance
ms.openlocfilehash: 5f753b5d522649575f92178e6f9c932d5ae4725f
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/30/2020
ms.locfileid: "49507395"
---
# <a name="gdpr-for-project-server"></a><span data-ttu-id="ab130-103">適用於 Project Server 的 GDPR</span><span class="sxs-lookup"><span data-stu-id="ab130-103">GDPR for Project Server</span></span>

<span data-ttu-id="ab130-p101">Project Server 會使用自訂指令碼來匯出及編輯 Project Web App 中的使用者資料。基本程序為：</span><span class="sxs-lookup"><span data-stu-id="ab130-p101">Project Server uses custom scripts to export and redact user data in Project Web App. The basic process is:</span></span>

1.  <span data-ttu-id="ab130-106">在您的伺服器陣列中尋找 Project Web App 網站。</span><span class="sxs-lookup"><span data-stu-id="ab130-106">Find the Project Web App sites in your farm.</span></span>

2.  <span data-ttu-id="ab130-107">在包含使用者的每個網站中尋找專案。</span><span class="sxs-lookup"><span data-stu-id="ab130-107">Find the projects in each site that contain the user.</span></span>

3.  <span data-ttu-id="ab130-108">匯出及檢閱您想要檢閱的資料類型。</span><span class="sxs-lookup"><span data-stu-id="ab130-108">Export and review the types of data that you want to review.</span></span>

4.  <span data-ttu-id="ab130-109">視需要編輯資料。</span><span class="sxs-lookup"><span data-stu-id="ab130-109">Redact data as needed.</span></span>

<span data-ttu-id="ab130-110">下列文章會詳細說明這些步驟：</span><span class="sxs-lookup"><span data-stu-id="ab130-110">These steps are covered in detail in the following articles:</span></span>

- [<span data-ttu-id="ab130-111">從 Project Server 匯出使用者資料</span><span class="sxs-lookup"><span data-stu-id="ab130-111">Export user data from Project Server</span></span>](/Project/export-user-data-from-project-server?toc=/Office365/Enterprise/toc.json)

- [<span data-ttu-id="ab130-112">從 Project Server 刪除使用者資料</span><span class="sxs-lookup"><span data-stu-id="ab130-112">Delete user data from Project Server</span></span>](/Project/delete-user-data-from-project-server?toc=/Office365/Enterprise/toc.json)


<span data-ttu-id="ab130-p102">請注意，Project Server 是以 SharePoint Server 為基礎來建置的，並且會將事件記錄到 SharePoint ULS 記錄和使用狀況資料庫。如需詳細資訊，請參閱 [SharePoint Server 的 GDPR](gdpr-for-sharepoint-server.md)。</span><span class="sxs-lookup"><span data-stu-id="ab130-p102">Note that Project Server is built on top of SharePoint Server and logs events to the SharePoint ULS logs and Usage database. See [GDPR for SharePoint Server](gdpr-for-sharepoint-server.md) for more information.</span></span>
