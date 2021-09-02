---
title: Microsoft 365 中的資料保留、刪除及銷毀
description: 有關資料保留、刪除及銷毀之 Microsoft 365 的 Microsoft 原則的概述。
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
ms.openlocfilehash: c851b235a70104720457d08c51529ee7b25c65e4
ms.sourcegitcommit: 1fd50ef5f165228109a3f2f0aef4b0c2aa59b2ff
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/02/2021
ms.locfileid: "58862353"
---
# <a name="data-retention-deletion-and-destruction-in-microsoft-365"></a>Microsoft 365 中的資料保留、刪除及銷毀

Microsoft 有一個用於 Microsoft 365 的資料處理標準原則，用以指定客戶資料在刪除之後保留多久。 一般來說，客戶資料遭到刪除的情況有兩種：

- 使用中 **刪除**：承租人具有使用中的訂閱，且使用者或系統管理員刪除資料，或系統管理員刪除使用者。
- **被動式刪除**：承租人訂閱已結束。

## <a name="data-retention"></a>資料保留

在每個刪除案例中，下表會根據資料類別和分類，顯示資料保留期間上限：

| 資料類別 | 資料分類 | 描述 | 範例 | 保留期間 |
|-----------------|-----------------|-----------------|----------------------------------|-------------------------------|
| 客戶資料 | 客戶內容| 管理員和使用者直接提供或建立的內容 <br><br> 在使用 Microsoft 365 中的服務時，包含在 Microsoft 資料中心內建立及儲存的所有文字、聲音、影片、圖像檔案及軟體 | Microsoft 365 應用程式中最常使用的範例，可讓使用者製作資料包含 Word、Excel、PowerPoint、Outlook 及 OneNote <br><br> 客戶內容也包含由客戶擁有/提供的機密 (密碼、憑證、加密金鑰、儲存金鑰)  | **主動刪除案例：** 最多30天 <br><br> **被動刪除案例：** 最多180天 |
| 客戶資料 |  (EUII 的使用者身分識別資訊)  | 識別或可用來識別 Microsoft 服務使用者的資料。 EUII 不含客戶內容 | 使用者名稱或顯示名稱 (網域 \ 使用者名稱)  <br><br>  (name@domain 的使用者主要名稱)  <br><br>  使用者特有的 IP 位址 | 使用中 **刪除案例：** 最多180天 (僅限租使用者系統管理員的動作)  <br><br> **被動刪除案例：** 最多180天 |
| 個人資料 <br>  (不包含在客戶資料) 中的資料 | 最終使用者 Pseudonymous 識別碼 (EUPI)  | Microsoft 所建立的識別碼，會與 Microsoft 服務的使用者關聯。 結合其他資訊（例如對應表格）時，EUPI 會識別使用者 <br><br> EUPI 不包含客戶上傳或建立的資訊 | 使用者 Guid、PUIDs 或 Sid <br><br> 會話 IDs | **主動刪除案例：** 最多30天 <br><br> **被動刪除案例：** 最多180天 |

## <a name="subscription-retention"></a>訂閱保留

在使用中訂閱的期限內，訂戶可以存取、解壓縮或刪除儲存在 Microsoft 365 中的客戶資料。 如果付費訂閱結束或終止，Microsoft 會將儲存在有限功能帳戶中 Microsoft 365 的客戶資料，保留90天，讓訂戶能夠解壓縮資料。 在90日保留期間結束後，Microsoft 會停用帳戶並刪除客戶資料。 在 Microsoft 365 訂閱到期或終止後的 180 天內，Microsoft 會停用帳戶並刪除此帳戶中的所有客戶資料。 一旦任何資料的最大保留期間超過時，資料會遭到商務性轉譯且無法恢復。

在您的免費試用版中，您的帳戶會在大部分的國家和地區中，移至30天的寬限狀態。 在此寬限期期間，您可以購買 Microsoft 365。 如果您決定不購買 Microsoft 365，您可以取消您的試用版或讓寬限期過期，並刪除您的試用版帳戶資訊和資料。

## <a name="expedited-deletion"></a>加急刪除

對於任何訂閱，訂閱者可以聯絡 Microsoft 支援服務並要求解除佈建訂閱。 在此程序中，所有的使用者資料會在系統管理員輸入 Microsoft 提供的鎖定代碼三天後遭到刪除。 這包括位於 SharePoint Online 和 Exchange Online 中的資料，在非使用中信箱處於保留狀態或儲存的資料。

如需加速取消布建的詳細資訊，請參閱 [取消您的訂閱](/microsoft-365/commerce/subscriptions/cancel-your-subscription)。

## <a name="related-links"></a>相關連結

- [資料貼上裝置銷毀](assurance-data-bearing-device-destruction.md)
- [Office 365 中的不變性](assurance-data-immutability.md)
- [Exchange Online 資料刪除](assurance-exchange-online-data-deletion.md)
- [SharePoint Online 資料刪除](assurance-sharepoint-online-data-deletion.md)
