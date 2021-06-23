---
title: 'Arm 規章中的國際流量 (ITAR) '
description: Azure 政府支援客戶在具有 Arm Regs 功能的系統中建立國際流量。
keywords: Microsoft 365, 合規性, 方案
localization_priority: None
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: 5ee31d5d61048593eec53a6bb72f8af538d2c3b3
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088922"
---
# <a name="international-traffic-in-arms-regulations-itar"></a><span data-ttu-id="21cdb-104">Arm 規章中的國際流量 (ITAR) </span><span class="sxs-lookup"><span data-stu-id="21cdb-104">International Traffic in Arms Regulations (ITAR)</span></span>

## <a name="itar-overview"></a><span data-ttu-id="21cdb-105">ITAR 概述</span><span class="sxs-lookup"><span data-stu-id="21cdb-105">ITAR overview</span></span>

<span data-ttu-id="21cdb-106">美國州的部門負責管理防護文章的匯出和暫時匯入， (表示任何專案或技術資料（由 Arm 匯出控制法案所規定），如) 的「Munitions」清單121.1 中所述的任何專案或技術資料) （由 Arm 匯出控制法案 (標題 22 USC 2778 及的國際流量 (ITAR)  (Title 22 CFR 120 – 130) 。</span><span class="sxs-lookup"><span data-stu-id="21cdb-106">The US Department of State is responsible for managing the export and temporary import of defense articles (meaning any item or technical data designated under the US Munitions List, as described in Title 22 CFR 121.1) that are governed by the Arms Export Control Act (Title 22 USC 2778) and the International Traffic in Arms Regulations (ITAR) (Title 22 CFR 120–130).</span></span> <span data-ttu-id="21cdb-107"> (DDTC) 的國防貿易控制 Directorate，負責管理受這些程式管理的實體。</span><span class="sxs-lookup"><span data-stu-id="21cdb-107">The Directorate for Defense Trade Controls (DDTC) is responsible for managing entities governed under these programs.</span></span>

## <a name="microsoft-and-itar"></a><span data-ttu-id="21cdb-108">Microsoft 和 ITAR</span><span class="sxs-lookup"><span data-stu-id="21cdb-108">Microsoft and ITAR</span></span>

<span data-ttu-id="21cdb-109">Microsoft 提供某些可以支援 ITAR 義務之客戶的雲端服務或服務功能。</span><span class="sxs-lookup"><span data-stu-id="21cdb-109">Microsoft provides certain cloud services or service features that can support customers with ITAR obligations.</span></span> <span data-ttu-id="21cdb-110">雖然 ITAR 未提供相容性認證，但 Microsoft 會運作並設計出範圍內的服務，以支援客戶的 ITAR 義務和合規性計畫。</span><span class="sxs-lookup"><span data-stu-id="21cdb-110">While there is no compliance certification for the ITAR, Microsoft operates and has designed in-scope services to be capable of supporting a customer's ITAR obligations and compliance program.</span></span>  
  
<span data-ttu-id="21cdb-111">Microsoft Azure政府和 Microsoft Office 365 美國政府針對國防公司透過其他合約承諾給客戶 ITAR，以提供有關儲存資料位置的其他合約承諾，以及對 US 人員存取這類資料的能力限制。</span><span class="sxs-lookup"><span data-stu-id="21cdb-111">Microsoft Azure Government and Microsoft Office 365 U.S. Government for Defense provide support for customers with data subject to the ITAR through additional contractual commitments to customers regarding the location of stored data, and limitations on the ability to access such data to US persons.</span></span> <span data-ttu-id="21cdb-112">Microsoft 為這些政府雲端服務的基礎結構和操作元件提供這些保證，但客戶最終負責其環境中其應用程式的保護和架構。</span><span class="sxs-lookup"><span data-stu-id="21cdb-112">Microsoft provides these assurances for the infrastructure and operational components of these government cloud services, but customers are ultimately responsible for the protection and architecture of their applications within their environments.</span></span>  
  
<span data-ttu-id="21cdb-113">客戶必須為其他合約簽署其他合約，以將 Microsoft 的意圖儲存 ITAR 控制的資料，讓 Microsoft 能夠遵守我們對客戶及美國政府的責任。</span><span class="sxs-lookup"><span data-stu-id="21cdb-113">Customers must sign additional agreements formally notifying Microsoft of their intention to store ITAR-controlled data, so that Microsoft may comply with responsibilities both to our customers and to the US government.</span></span>  
  
<span data-ttu-id="21cdb-114">ITAR 對舉報違規有特定責任，可提供某些風險降低的效益。</span><span class="sxs-lookup"><span data-stu-id="21cdb-114">The ITAR has specific obligations to report violations, which can provide certain risk mitigation benefits.</span></span> <span data-ttu-id="21cdb-115">microsoft Enterprise 合約修正功能可讓 microsoft 與客戶一起運作，以舉報這類違規行為。</span><span class="sxs-lookup"><span data-stu-id="21cdb-115">The Microsoft Enterprise Agreement Amendment enables Microsoft and the customer to work together in reporting such violations.</span></span>  
  
<span data-ttu-id="21cdb-116">尋找主控 ITAR 管制資料的客戶應使用其 Microsoft 帳戶和授權小組來深入瞭解、取得正確的協定，以及存取相關的系統架構資訊。</span><span class="sxs-lookup"><span data-stu-id="21cdb-116">Customers seeking to host ITAR-regulated data should work with their Microsoft account and licensing teams to learn more, obtain proper agreements, and access relevant system architecture information.</span></span>

## <a name="microsoft-in-scope-cloud-services"></a><span data-ttu-id="21cdb-117">Microsoft 範圍內雲端服務</span><span class="sxs-lookup"><span data-stu-id="21cdb-117">Microsoft in-scope cloud services</span></span>

- [<span data-ttu-id="21cdb-118">Azure 政府</span><span class="sxs-lookup"><span data-stu-id="21cdb-118">Azure Government</span></span>](https://aka.ms/AzureCompliance)
- [<span data-ttu-id="21cdb-119">Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="21cdb-119">Office 365 U.S. Government Defense</span></span>](https://go.microsoft.com/fwlink/p/?LinkID=2077751)

## <a name="frequently-asked-questions"></a><span data-ttu-id="21cdb-120">常見問題集</span><span class="sxs-lookup"><span data-stu-id="21cdb-120">Frequently asked questions</span></span>

<span data-ttu-id="21cdb-121">**我可以在哪裡要求規範資訊？**</span><span class="sxs-lookup"><span data-stu-id="21cdb-121">**Where can I request compliance information?**</span></span>

<span data-ttu-id="21cdb-122">請與您的 Microsoft 客戶代表聯繫。</span><span class="sxs-lookup"><span data-stu-id="21cdb-122">Contact your Microsoft account representative.</span></span>

## <a name="resources"></a><span data-ttu-id="21cdb-123">資源</span><span class="sxs-lookup"><span data-stu-id="21cdb-123">Resources</span></span>

- [<span data-ttu-id="21cdb-124">DDTC ITAR</span><span class="sxs-lookup"><span data-stu-id="21cdb-124">DDTC ITAR</span></span>](https://www.pmddtc.state.gov/?id=ddtc_kb_article_page&sys_id=24d528fddbfc930044f9ff621f961987)
- [<span data-ttu-id="21cdb-125">ITAR Title 22 CFR 120-130</span><span class="sxs-lookup"><span data-stu-id="21cdb-125">ITAR Title 22 CFR 120–130</span></span>](https://aka.ms/itar)
- [<span data-ttu-id="21cdb-126">搭配使用 Azure 政府與 ITAR 控制的資料</span><span class="sxs-lookup"><span data-stu-id="21cdb-126">Using Azure Government with ITAR controlled data</span></span>](https://aka.ms/azure-itar-guide)
- [<span data-ttu-id="21cdb-127">Azure 政府</span><span class="sxs-lookup"><span data-stu-id="21cdb-127">Azure Government</span></span>](https://azure.microsoft.com/features/gov/)
- [<span data-ttu-id="21cdb-128">Office 365美國政府</span><span class="sxs-lookup"><span data-stu-id="21cdb-128">Office 365 U.S. Government</span></span>](https://products.office.com/government/office-365-web-services-for-government)
- [<span data-ttu-id="21cdb-129">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="21cdb-129">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
