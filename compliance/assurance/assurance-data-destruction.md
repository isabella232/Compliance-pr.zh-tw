---
title: Microsoft 365 中的資料銷毀
description: 有關回收、處置或毀壞 Microsoft 365 資料中心磁片磁碟機和伺服器之 Microsoft 原則的概述。
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
ms.openlocfilehash: 229221d9cba2d7cc92e99086d647071556dae9e3
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482126"
---
# <a name="data-destruction-in-microsoft-365"></a>Microsoft 365 中的資料銷毀

## <a name="physical-data-destruction"></a>實體資料銷毀

Microsoft 有資料處理標準原則，可處理磁片磁碟機的回收與處置，以及失敗或淘汰伺服器的情況。 在重複使用任何 Microsoft 365 磁片磁碟機之前，Microsoft 會執行實體淨化處理常式與國家安全局的標準及技術特殊出版物 800-88 ([NIST SP 800-88 指導方針，以進行媒體淨化](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf)) 。 因為 Microsoft 365 中的所有磁片磁碟機都使用 BitLocker 磁片區層級加密進行加密，所以從技術上而言，並不需要 NIST SP 800-88 相容的擦除功能。 不過，Microsoft 會執行此程式。

在 Microsoft 365 資料中心內使用的失敗磁片，會透過 ISO 程式遭到實際銷毀和審核。 資產類型決定適當的處置方式。 對於無法擦出的硬碟，Microsoft 會使用銷毀程式來銷毀媒體，並不可能轉譯資訊的修復。 例如，磁片實際損毀、pulverized 或 incinerated。 Microsoft 保留所有毀壞記錄，並在 Microsoft 365 內重複使用的伺服器上執行類似的清理程式。 這些指導方針包含電子和實體的淨化。

每個資料中心都使用現場實際毀壞程式來處理其磁片。 在資料中心的每個區域中，為磁片處置指定的儲存媒體的安全容器。 每個安全的 bin 工作站都有影片監控監控。 一旦處置紙盒的容量大約為50%，網站服務小組便會聯繫實體安全小組，以協調移除。 網站服務人員和安全性 Office 移除安全處置 bin，並將它放在指定的安全儲存區。 在處理過程中，控制對貼出裝置之資料處理的原則和程式會進行經常性的測試，包括確定已核准機器的狀況的程式。

在資料銷毀過程中，磁片會以符合 NIST 800-88 (的方式來清除（如有可能）) 然後放入工業碎紙機，並以實際 demolished。 Microsoft 會利用 NIST SP 800-88 的一致性清理/清除、資產銷毀、加密、準確清查、追蹤，以及保護傳輸期間的保管鏈，對資產進行責任。 此程式是透過封閉式電視監控，並在完成時發出銷毀憑證。

Microsoft 會使用資料擦除的單位從 [極端的通訊協定方案](https://www.enterprisedataerasure.com/) (EPS) 。 EPS 軟體支援用於清理及清除/安全擦除的 NIST SP 800-88 需求。 在 [清理] 或「銷毀」之前，庫存是由 Microsoft 資產管理員所建立。 如果供應商用於損毀，則廠商會為銷毀的每個資產（由資產管理員驗證）提供損毀憑證。

## <a name="virtual-data-destruction"></a>虛擬資料銷毀

Microsoft 具有處理有效虛擬資料銷毀的資料處理原則和程式，以防範在服務租使用者間不正當的資料共用，或在服務中實刪除之後可存取的可能性。 從一個承租人中的服務刪除的資料無法存取另一個服務租使用者，即使已重新指派任何基礎實體儲存體也是一樣。 這是多種虛擬化和分散技術用來調整虛擬環境的複雜效果的結果，每個服務租使用者內之應用程式的使用中刪除行為 (例如 [分頁清零](/office365/securitycompliance/office-365-exchange-online-data-deletion#page-zeroing)) ，以及所需的媒體和應用程式內容加密處理常式。