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
ms.localizationpriority: medium
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
ms.openlocfilehash: 20a21fe0d67f8986ec6e89b8ecbfd2915f9b8245
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481935"
---
# <a name="internal-logging-for-microsoft-365-engineering"></a>Microsoft 365 工程內部記錄

除了可供客戶使用的事件和記錄資料之外，Microsoft 還會維護內部的記錄資料收集系統，可供 Microsoft 365 的工程師使用。 許多不同類型的記錄資料會從 Microsoft 365 伺服器上傳至專有的安全性監控解決方案，以進行接近即時 (NRT) 分析和內部、大型資料計算服務 (Cosmos) 以進行長期存放。 使用 (ODL) 的專屬自動化 Office 工具，在已核准的埠和通訊協定上，使用一種已核准的埠和通訊協定，以 FIPS 140-2 驗證的 TLS 連線進行此資料傳輸。 Microsoft 365 用來收集和處理審計記錄的工具不允許對原始的審計記錄內容或時間順序進行永久或不可逆的變更。

服務小組使用 Cosmos 做為集中式存放庫，進行應用程式使用方式的分析，以測量系統和作業效能，並尋找可能指出問題或安全性問題的 abnormalities 和模式。 每個服務小組都會上載包含下列各項的基準：

- 事件記錄檔
- AppLocker 記錄
- 效能資料
- System Center 資料
- 詳細通話記錄
- 經驗品質資料
- IIS 網頁伺服器記錄檔
- SQL Server 記錄
- Syslog 資料
- 安全性審核記錄檔

在上傳之前，ODL 應用程式會使用清理服務來移除任何包含客戶資料的欄位，例如承租人資訊和使用者識別資訊，並以雜湊值取代這些欄位。 登入的記錄會上傳至 Cosmos 和 NRT 安全性監視解決方案，以分析記錄中潛在的安全性事件和效能指標。 Cosmos 中的審計記錄資料保留期間是由服務小組決定。大多數的審計記錄資料會保留90天或更長的時間，以支援安全性事件調查，並符合法規保留要求。

Cosmos 中儲存的 Microsoft 365 資料存取權僅限於授權的人員。 Microsoft 會將審核記錄的管理限制為負責審計功能的安全小組成員的有限子集。 安全小組不具備 Cosmos 的管理存取權，且會記錄和審核所有變更。

NRT 分析之後，每個服務小組都可以流量分析工具及儀表板，進行資料關聯、互動式查詢及資料分析。 這些報告可用於監視及改善服務的整體效能。
