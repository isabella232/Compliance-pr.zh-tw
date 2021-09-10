---
title: Microsoft 365處理資料損毀
description: 本文說明 Microsoft 365 中的資料損毀，以及 Microsoft 採取的措施，以防止及復原資料。
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
ms.openlocfilehash: 860a150760e080df4a577d73478a75ac94b8700b
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58946947"
---
# <a name="dealing-with-data-corruption-in-microsoft-365"></a>處理 Microsoft 365 中的資料損毀

執行大規模雲端服務的一個富有挑戰性的層面是如何處理資料損毀，並提供大量的資料和獨立的系統。 資料損毀可能是由下列原因所造成：

- 應用程式或基礎結構錯誤，破壞部分或所有應用程式狀態
- 導致資料遺失或無法讀取資料的硬體問題
- 人力運作錯誤
- 惡意駭客和不滿的員工
- 外部服務中導致資料遺失的事件

因為資料完整性的彈性程度較高，所以 Microsoft 已內置 Microsoft 365 保護機制，以避免發生損毀，以及可讓我們恢復資料的系統和程式。 在工程發佈過程的各個階段內，都存在檢查和處理常式，以提升資料損毀的復原能力，包括：

- 系統設計
- 程式碼組織和結構
- 程式碼檢查
- 單元測試、整合測試及系統測試
- 行程電線測試/關口

在 Microsoft 365 的實際執行環境中，資料中心間的對等複寫可確保任何資料都有多個即時複本。 標準映射和腳本用於復原遺失的伺服器，而複寫的資料則用於還原客戶資料。 由於內建的資料恢復檢查和程式，Microsoft 只會維護 Microsoft 365 資訊系統檔 (的備份，包括安全性相關檔) ，使用內建複寫 SharePoint 線上及內部程式碼存放庫工具，來源返廠。 系統檔儲存在 SharePoint 線上，來源返廠包含系統和應用程式影像。 線上和來源返廠 SharePoint 都使用版本設定，而且會以接近即時的時間進行複製。
