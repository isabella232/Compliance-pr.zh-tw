---
title: Microsoft 365資源限制
description: 在本文中，您可以找到 Microsoft 365 中各種應用程式的資源限制的相關資訊。
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
ms.openlocfilehash: 764259e22b23ecc7cea363283fc313a94875a2d1
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158572"
---
# <a name="service-resource-limits"></a>服務資源限制

資源限制是使用配額來強制執行 (限制) 和節流。 Azure Active Directory (Azure AD) 和個別 Microsoft 365 服務都會使用兩者。 限制是服務特有的，而且隨時間而變更會隨著新功能的增加而變更。 如需各種服務目前限制的詳細資訊，請參閱下列主題：

- [Azure AD 服務限制和限制](/azure/azure-resource-manager/management/azure-subscription-service-limits)
- [Exchange Online 限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
- [SharePoint線上軟體界限和限制](https://support.office.com/article/SharePoint-Online-software-boundaries-and-limits-8F34FF47-B749-408B-ABC0-B605E1F6D498)
- [商務用 Skype限制](https://technet.microsoft.com/library/skype-for-business-online-limits.aspx)
- [YammerREST API 和速率限制](https://developer.yammer.com/docs/rest-api-rate-limits)
- [Sway 中的檔案大小限制](https://support.office.com/article/File-size-limits-in-Sway-4db21bc6-b42b-499f-9272-66e089db109f)

除了這些限制以外，還會在整個 Azure AD 和 Microsoft 365 中使用多個節流機制。 在服務內節流尤其重要，因為 Microsoft 資料中心的網路資源已針對使用服務的廣泛客戶進行優化。 節流機制包括：

- Azure AD 和 Microsoft 365 功能的使用者層級節流，它會限制由單一使用者執行的腳本或程式碼) 所 (的交易或並行通話數目。
- 在建立承租人時，會將預設的 PowerShell 節流原則指派給每個承租人。 這些設定會影響其他專案，例如可由單一系統管理員開啟的最大併發 PowerShell 會話數目。
- 每個 Exchange Online 客戶都有預設的 Exchange Web 服務 (ews) 原則，以進行 EWS 用戶端作業，以及適用于所有 Outlook 用戶端的節流。
