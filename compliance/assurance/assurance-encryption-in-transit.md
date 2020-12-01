---
title: 資料內傳輸的加密
description: 在本文中，會找到 Microsoft 如何在傳輸中加密 Microsoft 365 客戶資料的簡短說明。
ms.author: krowley
author: kccross
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: None
search.appverid:
- MET150
ms.collection:
- Strat_O365_Enterprise
- M365-security-compliance
- Strat_O365_Enterprise
- MS-Compliance
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: d1587e4bc315f99dc554158500638645606fbcec
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/30/2020
ms.locfileid: "49506189"
---
# <a name="encryption-for-data-in-transit"></a><span data-ttu-id="9570e-103">資料內傳輸的加密</span><span class="sxs-lookup"><span data-stu-id="9570e-103">Encryption for data-in-transit</span></span>

<span data-ttu-id="9570e-104">除了保護靜態客戶資料之外，Microsoft 還使用加密技術來保護傳輸中的客戶資料。</span><span class="sxs-lookup"><span data-stu-id="9570e-104">In addition to protecting customer data at rest, Microsoft uses encryption technologies to protect customer data in transit.</span></span> <span data-ttu-id="9570e-105">資料正在傳輸中：</span><span class="sxs-lookup"><span data-stu-id="9570e-105">Data is in transit:</span></span>

- <span data-ttu-id="9570e-106">當用戶端電腦與 Microsoft 伺服器通訊時;</span><span class="sxs-lookup"><span data-stu-id="9570e-106">when a client machine communicates with a Microsoft server;</span></span>
- <span data-ttu-id="9570e-107">當 Microsoft 伺服器與另一部 Microsoft 伺服器通訊時，和</span><span class="sxs-lookup"><span data-stu-id="9570e-107">when a Microsoft server communicates with another Microsoft server; and</span></span>
- <span data-ttu-id="9570e-108">當 Microsoft 伺服器與非 Microsoft 伺服器通訊時 (例如，Exchange Online 將電子郵件傳送至協力廠商電子郵件伺服器) 。</span><span class="sxs-lookup"><span data-stu-id="9570e-108">when a Microsoft server communicates with a non-Microsoft server (for example, Exchange Online delivering email to a third-party email server).</span></span>

<span data-ttu-id="9570e-109">透過 TLS 或 IPsec 進行資料中心之間的通訊，而所有客戶對向伺服器會使用 TLS 與用戶端電腦協商安全會話 (例如，Exchange Online 使用 TLS 1.2 搭配256位密碼強度，以 (FIPS 140-2 等級2驗證的) 。</span><span class="sxs-lookup"><span data-stu-id="9570e-109">Inter-data center communications between Microsoft servers take place over TLS or IPsec, and all customer-facing servers negotiate a secure session using TLS with client machines (for example, Exchange Online uses TLS 1.2 with 256-bit cipher strength is used (FIPS 140-2 Level 2-validated).</span></span> <span data-ttu-id="9570e-110"> (請參閱 [技術參考詳細資料](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) ，以瞭解 Office 365 支援的 TLS 密碼套件清單。 ) 這適用于用戶端（例如 Outlook、商務用 Skype、Microsoft 團隊和 outlook (網頁版）所使用的通訊協定（例如，HTTP、POP3 等等 ) ）。</span><span class="sxs-lookup"><span data-stu-id="9570e-110">(See [Technical reference details about encryption](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) for a list of TLS cipher suites supported by Office 365.) This applies to the protocols that are used by clients such as Outlook, Skype for Business, Microsoft Teams, and Outlook on the web (for example, HTTP, POP3, etc.).</span></span>

<span data-ttu-id="9570e-111">公用憑證是由 Microsoft IT SSL 使用 SSLAdmin （內部 Microsoft 工具）發行，以保護傳輸資訊的機密性。</span><span class="sxs-lookup"><span data-stu-id="9570e-111">The public certificates are issued by Microsoft IT SSL using SSLAdmin, an internal Microsoft tool to protect confidentiality of transmitted information.</span></span> <span data-ttu-id="9570e-112">所有由 Microsoft 所發行的憑證，其長度最低為2048位，且 Webtrust 合規性需要 SSLAdmin，以確保只將憑證發行給 Microsoft 所擁有的公用 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="9570e-112">All certificates issued by Microsoft IT have a minimum of 2048 bits in length, and Webtrust compliance requires SSLAdmin to make sure that certificates are issued only to public IP addresses owned by Microsoft.</span></span> <span data-ttu-id="9570e-113">任何無法符合此準則的 IP 位址，都是透過例外狀況流程進行路由傳送。</span><span class="sxs-lookup"><span data-stu-id="9570e-113">Any IP addresses that fail to meet this criterion are routed through an exception process.</span></span>

<span data-ttu-id="9570e-114">已啟用轉寄保密 (FS) 等所有執行詳細資料（如 TLS 的版本）是否已啟用，密碼套件等的順序皆可公開使用。</span><span class="sxs-lookup"><span data-stu-id="9570e-114">All implementation details such as the version of TLS being used, whether Forward Secrecy (FS) is enabled, the order of cipher suites, etc., are available publicly.</span></span> <span data-ttu-id="9570e-115">查看這些詳細資料的一種方式是使用協力廠商網站，例如 [QUALYS SSL 實驗](https://www.ssllabs.com)。</span><span class="sxs-lookup"><span data-stu-id="9570e-115">One way to see these details is to use a third-party website, such as [Qualys SSL Labs](https://www.ssllabs.com).</span></span> <span data-ttu-id="9570e-116">以下是 Qualys 中的自動測試頁面連結，可顯示下列服務的資訊：</span><span class="sxs-lookup"><span data-stu-id="9570e-116">Below are the links to automated test pages from Qualys that display information for the following services:</span></span>

- [<span data-ttu-id="9570e-117">Office 365 入口網站</span><span class="sxs-lookup"><span data-stu-id="9570e-117">Office 365 Portal</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [<span data-ttu-id="9570e-118">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="9570e-118">Exchange Online</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [<span data-ttu-id="9570e-119">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9570e-119">SharePoint Online</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [<span data-ttu-id="9570e-120">商務用 Skype (SIP) </span><span class="sxs-lookup"><span data-stu-id="9570e-120">Skype for Business (SIP)</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [<span data-ttu-id="9570e-121">商務用 Skype (網頁) </span><span class="sxs-lookup"><span data-stu-id="9570e-121">Skype for Business (Web)</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [<span data-ttu-id="9570e-122">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="9570e-122">Exchange Online Protection</span></span>](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [<span data-ttu-id="9570e-123">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9570e-123">Microsoft Teams</span></span>](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

<span data-ttu-id="9570e-124">針對 Exchange Online Protection，URLs 會因租使用者名稱而異;不過，所有客戶都可以使用 **microsoft-com.mail.protection.outlook.com** 測試 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="9570e-124">For Exchange Online Protection, URLs vary by tenant names; however, all customers can test Microsoft 365 using **microsoft-com.mail.protection.outlook.com**.</span></span>
