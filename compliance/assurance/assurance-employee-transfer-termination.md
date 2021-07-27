---
title: Microsoft 員工調職和離職
description: 深入瞭解 Microsoft 員工的轉接與終止程式 Microsoft 365
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 4a71ab3ddf6688df5480a8f260e004778aa6212b
ms.sourcegitcommit: 07578a8e03b931f47c49f4e34b78cf8ba0605e8f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/23/2021
ms.locfileid: "53573358"
---
# <a name="microsoft-employee-transfer-and-termination"></a>Microsoft 員工調職和離職

Microsoft 與其他所有組織一樣，處理員工轉接及終止工作，成為其正常運作的一部分。 當員工變更職位或離開公司時，請務必及時撤銷不適當的存取。 為了便於進行有效的存取變更和存取 revocations，Microsoft 使用標準化的程式和自動化的程式，以 (IDM) System 的身分識別管理，協調人力資源資訊系統 (HRIS) 。 這兩個系統之間的自動化業務流程對於維護運作一致性、保護 Microsoft 的線上服務和資料、避免特權蔓延，以及減少與內幕威脅相關的風險非常重要。

Microsoft 線上服務是設計來運作，而不會對我們的工程師進行實際執行環境的系統管理存取。 Microsoft 會使用即時 (JIT) ，只需足夠存取 (JEA) 模型，以在必要時為工程師提供必要的臨時存取，以支援其服務。 若要要求和使用服務小群組帳戶進行 JIT 存取，工程師必須透過 IDM 工具要求及維護 eligibilities。 當員工轉移或終止時，系統會自動修改其服務小群組帳戶和相關的 eligibilities，以防止不適當的存取。

## <a name="transfer-and-reassignment"></a>轉移和重新指派

員工轉帳是透過員工主管的轉移交易要求來啟動。 管理員會建立一項申請，並與全球人才購置提供的信件流程。 一旦員工接受新角色的提供，HR 服務便會在人力資源核心工具中完成傳輸，觸發 IDM 以設定所有員工 eligibilities 的到期日。 員工必須送出要求並收到其新管理員的核准，以保留其 eligibilities。 無法提交要求或接收管理員核准會導致已轉移員工的 eligibilities 撤銷。 針對包含特定安全性含義的傳輸，系統存取和安全性群組成員資格會立即重新評估，以反映其新角色。

## <a name="termination"></a>終止

Microsoft 使用明確定義的原則和程式，在員工終止時立即撤銷對 Microsoft 系統和資源的實體和邏輯存取。 當員工提供通知時，該員工的主管會將終止日期輸入 HRIS。 在員工的最後一天之後，HRIS 會將該員工標示為已終止，並將該資訊共用給 IDM，這會自動移除所有的服務小群組帳戶和 eligibilities。

針對 involuntary 終止，HR 與員工的主管合作，遵循適當的步驟來終止和下架員工。 與自願終止類似，終止資訊會輸入 HRIS，以及任何必要的步驟，例如有效的日期協調、存取權移除。 和任何其他與角色轉換相關的步驟。
