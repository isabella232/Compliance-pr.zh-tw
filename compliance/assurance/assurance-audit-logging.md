---
title: 稽核記錄概觀
description: 深入瞭解 Microsoft 365 中的審計記錄
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
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 6e32e089a5b42f846a332e32218959fef5103615
ms.sourcegitcommit: 7a5b6bc58fc4613b38f3fda20aebee5cec6a5730
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/08/2021
ms.locfileid: "49787502"
---
# <a name="audit-logging-overview"></a>稽核記錄概觀

## <a name="how-does-microsoft-365-employ-audit-logging"></a>Microsoft 365 如何使用審核記錄？

Microsoft 365 採用審核記錄，偵測其產品和服務中未經授權的活動，並為 Microsoft 人員提供責任。 審核記錄會捕獲系統設定變更和存取事件的詳細資料，並提供詳細資訊來識別誰負責該活動、活動發生的時間和位置，以及活動的結果。 自動化記錄分析可支援接近即時偵測可疑行為。 可能的事件會上報至 Microsoft 365 的安全性回應小組，以進一步調查。

Microsoft 365 內部審核記錄會從各種來源捕獲記錄檔資料，例如：

- 事件記錄檔
- AppLocker 記錄
- 效能資料
- System Center 資料
- 詳細通話記錄
- 經驗品質資料
- IIS 網頁伺服器記錄檔
- SQL Server 記錄檔
- Syslog 資料
- 安全性審核記錄檔

## <a name="how-does-microsoft-365-centralize-and-report-on-audit-logs"></a>Microsoft 365 如何集中及報告審計記錄檔？

許多不同類型的記錄資料會從 Microsoft 365 伺服器上傳至內部的大型資料計算服務，稱為 Cosmos。 每個服務小組都會將審核記錄從各自的伺服器上傳至 Cosmos 資料庫，以進行匯總和分析。 使用稱為 Office Data Loader () 的專屬自動化工具，在已核准的埠和通訊協定上進行 FIPS 140-2 驗證的 TLS 連線，便會進行此資料傳輸。

服務小組對 Cosmos 中的資料，針對記錄關聯、警示和報告，對其資料執行範圍內查詢。 例如，Microsoft 365 安全小組會使用來自 Cosmos 的資料與專有的事件記錄分析程式，以關聯記錄資料、傳送警示，並產生 Microsoft 365 實際執行環境中可能可疑活動的可操作報告。 這些資料中的報告是用來修正漏洞，以及改善服務的整體效能。

## <a name="how-does-microsoft-365-protect-audit-logs"></a>Microsoft 365 如何保護審核記錄？

Microsoft 365 中用來收集和處理審計記錄的工具不允許對原始的審計記錄內容或時間順序進行永久或不可逆的變更。 存取儲存在 Cosmos 中的 Microsoft 365 資料會限制在授權的人員。 Microsoft 365 會限制對負責審計功能之服務小組成員的有限子集進行審計功能的管理。 這些小組成員無法修改或刪除 Cosmos 中的資料，而且會記錄及審核 Cosmos 之記錄機制的所有變更。 審核記錄會保留足夠長的時間，以支援事件調查並符合法規需求。 Cosmos 中的審計記錄資料保留量的確切期限是由服務小組決定。大部分的審計記錄資料會保留90天或更長的時間。

## <a name="how-does-microsoft-365-protect-end-user-identifiable-information-that-may-be-captured-in-audit-logs"></a>Microsoft 365 如何保護使用者可在審計記錄中捕獲的使用者識別資訊嗎？

在將資料上傳至 Cosmos 之前，ODL 應用程式會使用清理服務，以模糊顯示任何包含客戶資料的欄位（如租使用者資訊和使用者身分識別資訊），並以雜湊值取代這些欄位。 匿名和雜湊記錄會重新寫入並上傳至 Cosmos。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與審核記錄相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | AU-2：審核事件 <br> AU-3：審計記錄的內容 <br> AU-4：審計儲存容量 <br> AU-5：對審計處理失敗的回應 <br> AU-6：審核檢查、分析和報告 <br> AU-7：審核減少與報告產生 <br> AU-8：時間戳記 <br> AU-9：保護審計資訊  <br> AU-10：不可否認性 <br> AU-11：審計記錄保留 <br> AU-12：審計產生  | 2020年9月24日 | 
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.4：記錄和監控 | 2020 年 2 月 22 日 |
| [ISO 27017 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.4：記錄和監控 | 2020 年 2 月 22 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48：資料中心記錄 <br> CA-60：審核記錄 | 2020月24日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-48：資料中心記錄 <br> CA-60：審核記錄 | 2020月24日|