---
title: 資料中心資產管理
description: Microsoft datacenter 資產管理的概述。
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
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: fafba29a25c5b01fa37d091fb210185a98365192
ms.sourcegitcommit: b228be59e13ae2e05ba85f65c1d4648fef5e9260
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/14/2021
ms.locfileid: "60356380"
---
# <a name="datacenter-asset-management"></a>資料中心資產管理

Microsoft 資料中心由各種實體和虛擬元件組成，每個元件稱為資產。 Microsoft Cloud Operations and 創新 (共同 + I) 工程群組遵循安全標準化的程式，以進行部署、追蹤及解除委任實體和虛擬資產。

## <a name="supply-chain-integrity"></a>供應鏈完整性

保護資產的開始，只是保護供應鏈的安全。 Microsoft 致力於供應鏈完整性及端對端供應鏈安全性。 供應商在傳輸雲端元件時遵循嚴格的保管鏈程式，以降低變更與篡改的風險。 所有輸入和輸出庫存都經過仔細檢查和監控，以確保韌體和元件完整性。

傳遞至 Microsoft 資料中心的資訊系統元件通常會排程。 對於未排程的傳遞，Microsoft 會徹底檢查並確保在實際錄入之前，已核准其進入 Microsoft 電腦聊天室的專案。 當資訊系統元件進入大樓時，資產管理小組會比較接收的專案與參考的憑證，並將裝置掃描至資產管理工具。 所有接收或運送的資訊系統元件，都是由工作流程票證檢查工具及資產管理工具中的貨運記錄檔追蹤。 訪客無法使用個人可擕式電腦和手機 (，但除了緊急通話和採取記事) 之外，) 的實際執行環境中也允許訪客 (colocations。 將 cellphones 插入裝置或拍攝相片是禁止每個資料中心原則。 如果進入資料中心的設備是用來維護的目的，該裝置需要資料中心存取工具系統中的資料中心管理核准。

## <a name="asset-inventory"></a>資產庫存

Microsoft 要求所有資料中心資產，都有一個指定的擁有者負責。 擁有者負責維護其實體和虛擬資產的最新資產資訊。 當新的實體資產新增到資料中心時，這些資產會簽署、掃描、建立唯一標記，並存回庫存控制系統。 自動化監控工具有助於追蹤實體和虛擬資產。

## <a name="asset-maintenance"></a>資產維護

Microsoft 有兩個團隊提供不同類型的資產維護：重要環境 (CE) 和網站服務小組。 CE 小組為包含設施運作基礎結構的電氣、機械和實體系統提供設施管理。 他們也會排程、執行、記錄及檢查對 CE 元件所執行的所有維護活動。 Microsoft 資料中心依靠電腦化維護管理系統來管理維護排程和工作順序。 網站服務小組服務的所有 Microsoft 線上服務資產都位於 Microsoft 資料中心。 此外，網站服務小組為屬於內容布建服務之資產的資源提供現場技術支援和中斷修復服務。

## <a name="asset-classification"></a>資產分類

Microsoft 資產（包括資料）會依照 Enterprise 資料分類法指導方針分類。 這些指導方針會提升整個企業的標準化，並每年檢查和更新。 資產分類及資產保護標準概述了員工在與每項資產互動時必須遵循的安全性程式。 客戶被視為其儲存在 Microsoft 雲端環境中之資料的擁有者。 分類為客戶內容或客戶資料的資料資產受到適用的安全性程序保護。

Microsoft 認為所有檔都歸類為系統資產。 網站服務小組負責分類資產，並根據資產分類和資產保護標準使用相關聯的保護，以及服務小組所定義的任何其他需求。

資產擁有者必須指派資產分類的資產分類，不例外。 在 Microsoft 資料中心環境中，資產是指伺服器和網路裝置。 其他數位媒體（例如 USB 快閃磁片磁碟機、外部硬碟或 CD/Dvd）不會用於服務作業。 資料中心未使用非數位媒體。

## <a name="media-storage"></a>媒體儲存

Microsoft 數位媒體資產實際和安全地儲存在 Microsoft datacenter colocation 聊天室中。 實體存取控制和影片監控有多種層級，都是用來保護和監視這些資產。 當數位媒體資產到達生命週期的結尾時，在處置之前，使用與 NIST SP 800-88 一致的方法，清除、清除或銷毀這些資產。 [資料貼上裝置的銷毀](assurance-data-bearing-device-destruction.md)文章涵蓋安全處置資產的處理常式。

## <a name="media-transport"></a>媒體傳輸

Microsoft 透過保管階層的保護，將資產傳輸活動限制于授權的人員。 使用鎖定、防篡改憑證及必要的資產清查驗證，可確保只有經過授權的人員才會參與資產傳輸。

所有從 Microsoft 資料中心傳輸的媒體都需要正確追蹤。 Microsoft 已與數個核准的廠商簽訂合同，以提供安全的運送服務。 安全傳輸是以準確的清查和保管鏈的方式開始。 在傳遞位置，傳輸公司的核准人員必須將移除的鎖定憑證解除鎖定，並解除鎖定容器。 接收人員會清查貨物，並傳送確認資產收據的訊息。 Microsoft 也會與廠商簽定，以提供設備銷毀。 根據資產分類，需要在現場銷毀一些裝置。

在安全控制空間以外的 Microsoft 數位媒體傳輸，必須監督兩個資料中心運作小組成員。 授權的人員在損毀之前，系統會持續附帶和監督資產。

資料中心管理小組透過票證檢查工具中追蹤的入場券，控制資訊系統元件的傳遞與移除。 資訊系統元件的傳遞和移除是由系統擁有者所授權。

## <a name="asset-retention"></a>資產保留

根據公司記錄管理、資產分類或合約需求所設定的保留需求，以適當方式保留 Microsoft 擁有的資產。 如需資料保留的詳細資訊，請參閱[資料保留、刪除及銷毀 Microsoft 365](assurance-data-retention-deletion-and-destruction-overview.md)。
