---
title: 'Arm 規章中的國際流量 (ITAR) '
description: Azure 政府支援客戶在具有 Arm Regs 功能的系統中建立國際流量。
keywords: Microsoft 365、合規性、方案
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
ms.openlocfilehash: 0797161b0c7bfca8d4fda37cbf05a037d29322de
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53384633"
---
# <a name="international-traffic-in-arms-regulations-itar"></a><span data-ttu-id="2049a-104">Arm 規章中的國際流量 (ITAR) </span><span class="sxs-lookup"><span data-stu-id="2049a-104">International Traffic in Arms Regulations (ITAR)</span></span>

## <a name="itar-overview"></a><span data-ttu-id="2049a-105">ITAR 概述</span><span class="sxs-lookup"><span data-stu-id="2049a-105">ITAR overview</span></span>

<span data-ttu-id="2049a-106">美國州的部門負責管理防護文章的匯出和暫時匯入， (表示任何專案或技術資料（由 Arm 匯出控制法案所規定），如) 的「標題 # CFR 121.1) 所述（由 Arm 匯出控制法案 (標題 22 USC 2778 和 Munitions 中的國際流量 (ITAR)  (Title 22 CFR 120-130) 。</span><span class="sxs-lookup"><span data-stu-id="2049a-106">The US Department of State is responsible for managing the export and temporary import of defense articles (meaning any item or technical data designated under the US Munitions List, as described in Title 22 CFR 121.1) that are governed by the Arms Export Control Act (Title 22 USC 2778) and the International Traffic in Arms Regulations (ITAR) (Title 22 CFR 120-130).</span></span> <span data-ttu-id="2049a-107"> (DDTC) 的國防貿易控制 Directorate，負責管理受這些程式管理的實體。</span><span class="sxs-lookup"><span data-stu-id="2049a-107">The Directorate for Defense Trade Controls (DDTC) is responsible for managing entities governed under these programs.</span></span>

## <a name="microsoft-and-itar"></a><span data-ttu-id="2049a-108">Microsoft 和 ITAR</span><span class="sxs-lookup"><span data-stu-id="2049a-108">Microsoft and ITAR</span></span>

<span data-ttu-id="2049a-109">Microsoft 提供某些可以支援 ITAR 義務之客戶的雲端服務或服務功能。</span><span class="sxs-lookup"><span data-stu-id="2049a-109">Microsoft provides certain cloud services or service features that can support customers with ITAR obligations.</span></span> <span data-ttu-id="2049a-110">雖然 ITAR 未提供相容性認證，但 Microsoft 會運作並設計出範圍內的服務，以支援客戶的 ITAR 義務和合規性計畫。</span><span class="sxs-lookup"><span data-stu-id="2049a-110">While there is no compliance certification for the ITAR, Microsoft operates and has designed in-scope services to be capable of supporting a customer's ITAR obligations and compliance program.</span></span>  
  
<span data-ttu-id="2049a-111">Microsoft Azure政府和 Microsoft Office 365 美國政府針對國防公司透過其他合約承諾給客戶 ITAR，以提供有關儲存資料位置的其他合約承諾，以及對 US 人員存取這類資料的能力限制。</span><span class="sxs-lookup"><span data-stu-id="2049a-111">Microsoft Azure Government and Microsoft Office 365 U.S. Government for Defense provide support for customers with data subject to the ITAR through additional contractual commitments to customers regarding the location of stored data, and limitations on the ability to access such data to US persons.</span></span> <span data-ttu-id="2049a-112">Microsoft 為這些政府雲端服務的基礎結構和操作元件提供這些保證，但客戶最終負責其環境中其應用程式的保護和架構。</span><span class="sxs-lookup"><span data-stu-id="2049a-112">Microsoft provides these assurances for the infrastructure and operational components of these government cloud services, but customers are ultimately responsible for the protection and architecture of their applications within their environments.</span></span>  
  
<span data-ttu-id="2049a-113">客戶必須為其他合約簽署其他合約，以將 Microsoft 的意圖儲存 ITAR 控制的資料，讓 Microsoft 能夠遵守我們對客戶及美國政府的責任。</span><span class="sxs-lookup"><span data-stu-id="2049a-113">Customers must sign additional agreements formally notifying Microsoft of their intention to store ITAR-controlled data, so that Microsoft may comply with responsibilities both to our customers and to the US government.</span></span>  
  
<span data-ttu-id="2049a-114">ITAR 對舉報違規有特定責任，可提供某些風險降低的效益。</span><span class="sxs-lookup"><span data-stu-id="2049a-114">The ITAR has specific obligations to report violations, which can provide certain risk mitigation benefits.</span></span> <span data-ttu-id="2049a-115">microsoft Enterprise 合約修正功能可讓 microsoft 與客戶一起運作，以舉報這類違規行為。</span><span class="sxs-lookup"><span data-stu-id="2049a-115">The Microsoft Enterprise Agreement Amendment enables Microsoft and the customer to work together in reporting such violations.</span></span>  
  
<span data-ttu-id="2049a-116">尋找主控 ITAR 管制資料的客戶應使用其 Microsoft 帳戶和授權小組來深入瞭解、取得正確的協定，以及存取相關的系統架構資訊。</span><span class="sxs-lookup"><span data-stu-id="2049a-116">Customers seeking to host ITAR-regulated data should work with their Microsoft account and licensing teams to learn more, obtain proper agreements, and access relevant system architecture information.</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="2049a-117">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="2049a-117">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="2049a-118">Azure 政府</span><span class="sxs-lookup"><span data-stu-id="2049a-118">Azure Government</span></span>
- <span data-ttu-id="2049a-119">Office 365美國政府高、Office 365 防衛</span><span class="sxs-lookup"><span data-stu-id="2049a-119">Office 365 U.S. Government - High, Office 365 Defense</span></span>

## <a name="azure-dynamics-365-and-itar"></a><span data-ttu-id="2049a-120">Azure、Dynamics 365 和 ITAR</span><span class="sxs-lookup"><span data-stu-id="2049a-120">Azure, Dynamics 365, and ITAR</span></span>

<span data-ttu-id="2049a-121">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE ITAR 服務](/azure/compliance/offerings/offering-itar)。</span><span class="sxs-lookup"><span data-stu-id="2049a-121">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure ITAR offering](/azure/compliance/offerings/offering-itar).</span></span>

## <a name="office-365-and-itar"></a><span data-ttu-id="2049a-122">Office 365 和 ITAR</span><span class="sxs-lookup"><span data-stu-id="2049a-122">Office 365 and ITAR</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="2049a-123">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="2049a-123">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="2049a-124">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="2049a-124">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="2049a-125">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="2049a-125">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="2049a-126">**適用性**</span><span class="sxs-lookup"><span data-stu-id="2049a-126">**Applicability**</span></span> | <span data-ttu-id="2049a-127">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="2049a-127">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="2049a-128">**GCC High**</span><span class="sxs-lookup"><span data-stu-id="2049a-128">**GCC High**</span></span> | <span data-ttu-id="2049a-129">活動摘要服務，Bing 服務，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="2049a-129">Activity Feed Service, Bing Services, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |
| <span data-ttu-id="2049a-130">**DoD**</span><span class="sxs-lookup"><span data-stu-id="2049a-130">**DoD**</span></span> | <span data-ttu-id="2049a-131">活動摘要服務，Bing 服務，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink</span><span class="sxs-lookup"><span data-stu-id="2049a-131">Activity Feed Service, Bing Services, Exchange Online, Intelligent Services, Microsoft Teams, Office 365 Customer Portal, Office Online, Office Service Infrastructure, Office Usage Reports, OneDrive for Business, People Card, SharePoint Online, Skype for Business, Windows Ink</span></span> |

### <a name="frequently-asked-questions"></a><span data-ttu-id="2049a-132">常見問題集</span><span class="sxs-lookup"><span data-stu-id="2049a-132">Frequently asked questions</span></span>

<span data-ttu-id="2049a-133">**我可以在哪裡要求 ITAR 的 Office 365 規範資訊？**</span><span class="sxs-lookup"><span data-stu-id="2049a-133">**Where can I request Office 365 compliance information for ITAR?**</span></span>

<span data-ttu-id="2049a-134">請與您的 Microsoft Office 365 帳戶代表聯繫。</span><span class="sxs-lookup"><span data-stu-id="2049a-134">Contact your Microsoft Office 365 account representative.</span></span>

### <a name="resources"></a><span data-ttu-id="2049a-135">資源</span><span class="sxs-lookup"><span data-stu-id="2049a-135">Resources</span></span>

- [<span data-ttu-id="2049a-136">DDTC ITAR</span><span class="sxs-lookup"><span data-stu-id="2049a-136">DDTC ITAR</span></span>](https://www.pmddtc.state.gov/?id=ddtc_kb_article_page&sys_id=24d528fddbfc930044f9ff621f961987)
- [<span data-ttu-id="2049a-137">ITAR Title 22 CFR 120-130</span><span class="sxs-lookup"><span data-stu-id="2049a-137">ITAR Title 22 CFR 120–130</span></span>](https://aka.ms/itar)
- [<span data-ttu-id="2049a-138">Office 365美國政府</span><span class="sxs-lookup"><span data-stu-id="2049a-138">Office 365 U.S. Government</span></span>](https://products.office.com/government/office-365-web-services-for-government)
- [<span data-ttu-id="2049a-139">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="2049a-139">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
