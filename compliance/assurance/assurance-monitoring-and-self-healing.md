---
title: Microsoft 365 中的資料監控及自我修復
description: 在本文中，您將深入瞭解 Microsoft 365 的監控及自我修復功能。
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
ms.custom:
- seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: d55621d10284c427afedeb3d60807411841d41dda2e07c52b293a676448dbe73
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54290621"
---
# <a name="data-monitoring-and-self-healing-in-microsoft-365"></a>Microsoft 365 中的資料監控及自我修復

在 Microsoft 365 規模的情況下，不可能讓客戶資料的彈性和安全，而不需要內建的監控，只是智慧化且具有快速且可靠的自我修復的警示。 在 Microsoft 365 規模監控一組服務是非常困難的。 需要引進新的 mindsets 和方法，並在已連線的全域環境中建立新的技術集合，以進行操作及管理服務。 我們已從傳統的監控方式收集資料集合及篩選，以建立以資料分析為基礎的方法提醒;在該資料中採取信號及建立信任，然後使用「自動化」來復原或解決問題。 這種方法可協助您從復原方程式中移出，進而使作業執行成本變低、速度更快，且易出錯。 

Microsoft 365 監視的基礎是一種包含資料 Insights 引擎的技術集合，該引擎是以 Azure、SQL Azure 和[開放來源流式資料庫技術](https://cassandra.apache.org/)為基礎。 其設計目的是收集和匯總資料，並取得結論。 目前，它會從超過100000個伺服器處理超過500000000個事件， (每天大約 15 TB) 分散于許多地區的數十個資料中心，且這些數位不斷增加。 

Microsoft 365 會使用 *外部監控*，這包括建立綜合交易，以測試重要的內容。 例如，在 Exchange Online 每個案例中，每隔五分鐘以分散的方式測試每個資料庫，提供系統中所有專案的接近連續覆蓋率。 從多個位置，每日250000000測試交易會執行，以建立服務的可靠基準或心跳。 

Microsoft 365 也會使用 *紅色警示* 的概念，它會將資料中心內所有機器的監控信號，向內部分縮小，以供人工管理。 此概念非常簡單：若有多個信號發生問題，則必須有一些問題。 它不是要在一個信號中建立信任，因此，每個信號都有合理的逼真度，使您獲得更高的精確度。 這個監視系統很強大，我們不會讓員工收看我們的監視器;我們所有的機器都是喚醒的機器，如果它偵測到問題，在這種情況下，它會向適當的呼叫人員進行尋呼，也就是在案例中，它會繼續並解決問題。 當我們開始收集信號，併發出紅色警示時，我們可以在所有的服務分割區中開始 triangulating。 

此警示會根據失敗警示和紅色警示的組合，確切指出哪些元件可能出現問題，以及系統即將嘗試重新開機信箱伺服器以修正問題。 

除了單一分頁還原之類的自我修復功能之外，Exchange Online 還包含一些功能，採用監控和自我修復的方式，其重點是保留使用者體驗。 這些功能包括 *受管理的可用性*，其可提供內建的監控和復原動作，以及 AutoReseed，它會在磁片故障後自動還原資料庫冗余。 

## <a name="managed-availability"></a>受管理的可用性 

受管理的可用性提供原始的健全狀況檢查和復原解決方案，可透過恢復導向的動作來監視和保護使用者的體驗。 受管理的可用性是與 Exchange 高可用性平臺整合內建的監控和復原動作。 其設計目的是在發生問題時立即偵測並修復，以供系統探索。 與舊版的外部監控解決方案及 Exchange 不同，受管理的可用性不會嘗試識別或傳達問題的根本原因。 相反地，其重點是針對下列三個主要使用者經驗方面的復原層面：

- **可用性** –使用者是否可以存取服務？ 
- **延遲** -使用者的經驗如何？ 
- **錯誤** -使用者是否可以完成所需的功能？ 

受管理的可用性是一項內部功能，可在執行 Exchange Online 的每一部 Microsoft 365 伺服器上執行。 它會輪詢並分析每秒的數百個健康情況度量。 如果發現有問題，大部分會自動修正。 但是，受管理的可用性一定會發生問題，但無法自行修復。 在這種情況下，受管理的可用性會透過事件記錄將問題提升至 Microsoft 365 支援小組。

## <a name="autoreseed"></a>AutoReseed

Exchange Online 伺服器是以儲存在相同非 RAID 磁片上的多個資料庫及其記錄資料流程的設定進行部署。 這項設定通常稱為 (JBOD) *一組磁片* ，因為不會使用任何儲存重複機制（例如 RAID）來複製磁片上的資料。 當 JBOD 環境中的磁片失敗時，該磁片上的資料將會遺失。 

已知 Exchange Online 大小，而且在其中部署的事實是數百萬磁片磁片磁碟機，則磁片磁碟機故障是 Exchange Online 中的正常情況。 實際上，每日超過100的失敗。 當內部部署企業部署中的磁片失敗時，系統管理員必須手動更換失敗的磁片並還原受影響的資料。 在雲端部署中 Microsoft 365 大小，具有 (雲端系統管理員的操作員) 手動取代磁片既不實用也可行。 

自動重新植入（或 *AutoReseed*）是一項功能，取代了操作員導向的動作，以回應磁片失敗、資料庫損毀事件或其他需要重新植入資料庫副本的問題。 AutoReseed 專為磁碟故障後，使用佈建在系統上的備用磁碟自動還原資料庫備援而設計。 磁片失敗時，儲存在該磁片上的資料庫副本會自動重新植入至伺服器上預先設定的備用磁片，進而還原冗余。 