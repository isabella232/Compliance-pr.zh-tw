---
title: 適用於商務用 Skype Server 的 GDPR
description: 深入了解如何在內部部署商務用 Skype Server 和 Lync Server 中解決 GDPR 需求。
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: high
titleSuffix: Microsoft GDPR
ms.collection: MS-Compliance
hideEdit: true
ms.openlocfilehash: e6c7eb83a8838e7942aa79c63482eaa30b095d00
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482598"
---
# <a name="gdpr-for-skype-for-business-server-and-lync-server"></a>適用於商務用 Skype Server 和 Lync Server 的 GDPR

商務用 Skype Server 和 Lync Server 的大部分資料會儲存在 Exchange Server 中，包括：

-   交談歷程記錄

-   語音信箱通知和抄錄

-   會議邀請

使用[適用於 Exchange Server 的 GDPR](gdpr-for-exchange-server.md) 中概述的程序，以針對 GDPR 要求尋找、匯出或刪除這些類型的資料。

連絡人清單會儲存在 SQL Server 資料庫中。他們可以透過下列方式匯出：

-   使用者可以自行匯出連絡人，方法是以滑鼠右鍵按一下群組標頭，然後選取 [複製]。這樣會將該群組中的所有連絡人複製到剪貼簿，然後貼入任何應用程式。

-   您可以使用 [Export-CsUserData](/powershell/module/skype/export-csuserdata) Cmdlet 來匯出此資料。

上傳至會議的內容 (例如 PowerPoint 檔案或講義) 或會議中產生的內容 (例如白板、投票或 Q/A) 會儲存在檔案管理工具中。如果使用者重新登入未過期的任何會議並且下載任何已上傳內容，或者擷取已產生內容的螢幕擷取畫面，那麼這個項目也可以匯出。

不在 Exchange 行事曆和連絡人清單和連絡人權限 (家人、同事等等) 的 MeetNow 會議是在使用者資料庫中。在 Lync Server 2013 及更新版本中，您可以使用 [Export-CsUserData](/powershell/module/skype/export-csuserdata) Cmdlet 來匯出此資料。
