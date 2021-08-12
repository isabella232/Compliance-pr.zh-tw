---
title: 資料內傳輸的加密
description: 在本文中，將會深入說明 Microsoft 如何在傳輸中加密 Microsoft 365 客戶資料。
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
hideEdit: true
ms.openlocfilehash: 6a4707be17c0ef5d992e1f98db9638b9b8337dfd22f012af914ef65891c315ed
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54291280"
---
# <a name="encryption-for-data-in-transit"></a>資料內傳輸的加密

除了保護靜態客戶資料之外，Microsoft 還使用加密技術來保護傳輸中的客戶資料。 資料正在傳輸中：

- 當用戶端電腦與 Microsoft 伺服器通訊時;
- 當 Microsoft 伺服器與另一部 Microsoft 伺服器通訊時，和
- 當 Microsoft 伺服器與非 Microsoft server 通訊時 (例如，Exchange Online 將電子郵件傳遞至協力廠商電子郵件伺服器) 。

透過 tls 或 IPsec 進行資料中心之間的通訊，而所有客戶對向伺服器會使用 tls 與用戶端電腦協商安全的會話 (例如，Exchange Online 使用 tls 1.2 搭配256位密碼強度， (FIPS 140-2 Level 2 驗證) 。  (查看有關 Office 365 所支援之 TLS 密碼套件之[詳細資料的技術參考詳細資料](/microsoft-365/compliance/technical-reference-details-about-encryption)。 ) 這適用于用戶端所使用的通訊協定，例如 Outlook、商務用 Skype、Microsoft Teams 和 Outlook 網頁版 (例如，HTTP、POP3 等 ) 。

公用憑證是由 Microsoft IT SSL 使用 SSLAdmin （內部 Microsoft 工具）發行，以保護傳輸資訊的機密性。 所有由 Microsoft 所發行的憑證，其長度最低為2048位，且 Webtrust 合規性需要 SSLAdmin，以確保只將憑證發行給 Microsoft 所擁有的公用 IP 位址。 任何無法符合此準則的 IP 位址，都是透過例外狀況流程進行路由傳送。

已啟用轉寄保密 (FS) 等所有執行詳細資料（如 TLS 的版本）是否已啟用，密碼套件等的順序皆可公開使用。 查看這些詳細資料的一種方式是使用協力廠商網站，例如 [QUALYS SSL 實驗](https://www.ssllabs.com)。 以下是 Qualys 中的自動測試頁面連結，可顯示下列服務的資訊：

- [Office 365門戶](https://www.ssllabs.com/ssltest/analyze.html?d=portal.office.com&hideResults=on)
- [Exchange Online](https://www.ssllabs.com/ssltest/analyze.html?d=outlook.office365.com&hideResults=on)
- [SharePoint Online](https://www.ssllabs.com/ssltest/analyze.html?d=microsoft-my.sharepoint.com&hideResults=on)
- [商務用 Skype (SIP) ](https://www.ssllabs.com/ssltest/analyze.html?d=sipdir.online.lync.com)
- [商務用 Skype (網頁) ](https://www.ssllabs.com/ssltest/analyze.html?d=webdir.online.lync.com&hideResults=on)
- [Exchange Online Protection](https://ssl-tools.net/mailservers/microsoft-com.mail.protection.outlook.com)
- [Microsoft Teams](https://www.ssllabs.com/ssltest/analyze.html?d=teams.microsoft.com&latest)

針對 Exchange Online Protection，URLs 會因租使用者名稱而異;不過，所有客戶都可以使用 **microsoft-com.mail.protection.outlook.com** 測試 Microsoft 365。
