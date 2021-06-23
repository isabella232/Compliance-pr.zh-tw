---
title: Microsoft 365 Microsoft 365 工程的內部記錄
description: 在本文中，將說明 Microsoft 365 工程小組的內部記錄如何運作。
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
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 71b08509ae920ad88ecfa1566b9a11d640b0534f
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53088592"
---
# <a name="internal-logging-for-microsoft-365-engineering"></a><span data-ttu-id="601b9-103">Microsoft 365 工程內部記錄</span><span class="sxs-lookup"><span data-stu-id="601b9-103">Internal logging for Microsoft 365 engineering</span></span>

<span data-ttu-id="601b9-104">除了可供客戶使用的事件和記錄資料之外，Microsoft 還會維護內部的記錄資料收集系統，可供 Microsoft 365 的工程師使用。</span><span class="sxs-lookup"><span data-stu-id="601b9-104">In addition to the events and log data available for customers, Microsoft maintains an internal log data collection system that is available to Microsoft 365 engineers.</span></span> <span data-ttu-id="601b9-105">許多不同類型的記錄資料會從 Microsoft 365 伺服器上傳至專有的安全性監控解決方案，以進行接近即時 (NRT) 分析和內部、大型資料計算服務 (Cosmos) 以進行長期存放。</span><span class="sxs-lookup"><span data-stu-id="601b9-105">Many different types of log data are uploaded from Microsoft 365 servers to a proprietary security monitoring solution for near real-time (NRT) analysis and an internal, big data computing service (Cosmos) for long-term storage.</span></span> <span data-ttu-id="601b9-106">使用 (ODL) 的專屬自動化 Office 工具，在已核准的埠和通訊協定上，使用一種已核准的埠和通訊協定，以 FIPS 140-2 驗證的 TLS 連線進行此資料傳輸。</span><span class="sxs-lookup"><span data-stu-id="601b9-106">This data transfer occurs over a FIPS 140-2-validated TLS connection on approved ports and protocols using a proprietary automation tool called the Office Data Loader (ODL).</span></span> <span data-ttu-id="601b9-107">Microsoft 365 用來收集和處理審計記錄的工具不允許對原始的審計記錄內容或時間順序進行永久或不可逆的變更。</span><span class="sxs-lookup"><span data-stu-id="601b9-107">The tools used in Microsoft 365 to collect and process audit records do not allow permanent or irreversible changes to the original audit record content or time ordering.</span></span>

<span data-ttu-id="601b9-108">服務小組使用 Cosmos 做為集中式存放庫，進行應用程式使用方式的分析，以測量系統和作業效能，並尋找可能指出問題或安全性問題的 abnormalities 和模式。</span><span class="sxs-lookup"><span data-stu-id="601b9-108">Service teams use Cosmos as a centralized repository to conduct an analysis of application usage, to measure system and operational performance, and to look for abnormalities and patterns that may indicate problems or security issues.</span></span> <span data-ttu-id="601b9-109">每個服務小組都會上載包含下列各項的基準：</span><span class="sxs-lookup"><span data-stu-id="601b9-109">Each service team uploads a baseline that includes:</span></span>

- <span data-ttu-id="601b9-110">事件記錄檔</span><span class="sxs-lookup"><span data-stu-id="601b9-110">Event logs</span></span>
- <span data-ttu-id="601b9-111">AppLocker 記錄</span><span class="sxs-lookup"><span data-stu-id="601b9-111">AppLocker logs</span></span>
- <span data-ttu-id="601b9-112">效能資料</span><span class="sxs-lookup"><span data-stu-id="601b9-112">Performance data</span></span>
- <span data-ttu-id="601b9-113">System Center 資料</span><span class="sxs-lookup"><span data-stu-id="601b9-113">System Center data</span></span>
- <span data-ttu-id="601b9-114">詳細通話記錄</span><span class="sxs-lookup"><span data-stu-id="601b9-114">Call detail records</span></span>
- <span data-ttu-id="601b9-115">經驗品質資料</span><span class="sxs-lookup"><span data-stu-id="601b9-115">Quality of experience data</span></span>
- <span data-ttu-id="601b9-116">IIS 網頁伺服器記錄檔</span><span class="sxs-lookup"><span data-stu-id="601b9-116">IIS Web Server logs</span></span>
- <span data-ttu-id="601b9-117">SQL Server 記錄</span><span class="sxs-lookup"><span data-stu-id="601b9-117">SQL Server logs</span></span>
- <span data-ttu-id="601b9-118">Syslog 資料</span><span class="sxs-lookup"><span data-stu-id="601b9-118">Syslog data</span></span>
- <span data-ttu-id="601b9-119">安全性審核記錄檔</span><span class="sxs-lookup"><span data-stu-id="601b9-119">Security audit logs</span></span>

<span data-ttu-id="601b9-120">在上傳之前，ODL 應用程式會使用清理服務來移除任何包含客戶資料的欄位，例如承租人資訊和使用者識別資訊，並以雜湊值取代這些欄位。</span><span class="sxs-lookup"><span data-stu-id="601b9-120">Prior to uploading, the ODL application uses a scrubbing service to remove any fields that contain customer data, such as tenant information and end-user identifiable information, and replace those fields with a hash value.</span></span> <span data-ttu-id="601b9-121">登入的記錄會上傳至 Cosmos 和 NRT 安全性監視解決方案，以分析記錄中潛在的安全性事件和效能指標。</span><span class="sxs-lookup"><span data-stu-id="601b9-121">The scrubbed logs are uploaded to Cosmos and to the NRT security monitoring solution that analyzes the logs for potential security events and performance indicators.</span></span> <span data-ttu-id="601b9-122">Cosmos 中的審計記錄資料保留期間是由服務小組決定。大多數的審計記錄資料會保留90天或更長的時間，以支援安全性事件調查，並符合法規保留要求。</span><span class="sxs-lookup"><span data-stu-id="601b9-122">The period of audit log data retention in Cosmos is determined by the service teams; most audit log data is retained for 90 days or longer to support security incident investigations and to meet regulatory retention requirements.</span></span>

<span data-ttu-id="601b9-123">Cosmos 中儲存的 Microsoft 365 資料存取權僅限於授權的人員。</span><span class="sxs-lookup"><span data-stu-id="601b9-123">Access to Microsoft 365 data stored in Cosmos is restricted to authorized personnel.</span></span> <span data-ttu-id="601b9-124">Microsoft 會將審核記錄的管理限制為負責審計功能的安全小組成員的有限子集。</span><span class="sxs-lookup"><span data-stu-id="601b9-124">Microsoft restricts the management of audit logs to a limited subset of Security Team members responsible for audit functionality.</span></span> <span data-ttu-id="601b9-125">安全小組不具備 Cosmos 的管理存取權，且會記錄和審核所有變更。</span><span class="sxs-lookup"><span data-stu-id="601b9-125">The Security Team does not have standing administrative access to Cosmos, and all changes are recorded and audited.</span></span>

<span data-ttu-id="601b9-126">NRT 分析之後，每個服務小組都可以流量分析工具及儀表板，進行資料關聯、互動式查詢及資料分析。</span><span class="sxs-lookup"><span data-stu-id="601b9-126">After NRT analysis, each service team can use analysis tools and dashboards for data correlation, interactive queries, and data analytics.</span></span> <span data-ttu-id="601b9-127">這些報告可用於監視及改善服務的整體效能。</span><span class="sxs-lookup"><span data-stu-id="601b9-127">These reports are used to monitor and improve the overall performance of the service.</span></span>
