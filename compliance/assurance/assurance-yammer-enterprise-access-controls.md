---
title: Microsoft 365 Yammer 企業存取控制
description: 本文摘要說明實際執行環境中 Yammer Enterprise 的存取控制。
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
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: d9a3604bd987170ea266871cf4c384c0e071817dc10640eb01e560debb5d9664
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54291641"
---
# <a name="yammer-enterprise-access-controls"></a>Yammer 企業存取控制 

實體和邏輯存取 Yammer 的實際執行環境只限于一小組 (基礎結構和作業) 的人員。 與其他 Microsoft 365 工程師一樣，Yammer 的工程師也可讓使用者存取客戶資料。 您必須使用具有有限的核准者的即時存取控制系統來要求存取，類似于密碼箱。 核准者會驗證要求 (例如，他們會驗證要求是否根據需求、業務案例、時間等 ) 進行合法，然後核准或拒絕要求。 若要求遭到核准，就會將 JIT 存取權授與已定義和限制的時間。 超過存取時間之後，access 會自動到期。

與其他 Microsoft 365 服務一樣，所有 Yammer 實際執行環境的存取都使用多重要素驗證。 所有存取和命令歷史記錄皆為使用者，並定期由 Yammer 安全小組進行記錄及檢查。

如需 Yammer 管理與管理的詳細資訊，請參閱[Yammer 系統管理](/yammer/yammer-landing-page)說明。