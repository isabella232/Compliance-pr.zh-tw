---
title: Microsoft 365 中的帳戶管理
description: 深入瞭解 Microsoft 365 中的帳戶管理
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: d525edfb9854df156f5b7b8571199b7a0102a0bf
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58946969"
---
# <a name="account-management-in-microsoft-365"></a>Microsoft 365 中的帳戶管理

Microsoft 投入大量的系統和控制，可自動化大多數的 Microsoft 365 作業，同時會特意限制服務人員直接存取伺服器及客戶資料的需求。 人工管理服務和軟體會運作服務。 此結構可讓 Microsoft 以比例管理 Microsoft 365，並將內部和外部威脅的風險降至最低。 Microsoft 會進行存取控制，假設每個人都是潛在威脅 Microsoft 365 服務和客戶資料。 基於這個理由，零開始存取 (ZSA) 原則為 Microsoft 365 所使用的整個存取控制結構奠定基礎。

根據預設，Microsoft 人員在任何 Microsoft 365 環境或組織的客戶資料上都有零的特殊許可權存取權。 它只是透過可靠的檢查和核准系統，讓服務小組人員可以透過窄的動作和時間範圍獲得許可權存取。 透過此系統，Microsoft 可大幅減少 Microsoft 365 服務人員和攻擊者取得未授權存取的可能性，或對 Microsoft 服務和客戶造成惡意或意外傷害的可能性。

## <a name="account-types"></a>帳戶類型

Microsoft 365 會使用三種帳戶類別，滿足所有的組織使命和商務職能：服務小群組帳戶、服務帳戶及客戶帳戶。 管理這些帳戶是 Microsoft 與客戶之間的共同責任。 Microsoft 會管理服務小組和服務帳戶，其作用是用來操作和支援 Microsoft 產品及服務。 客戶帳戶是由客戶管理，並可讓他們調整帳戶存取權，以符合其內部存取控制需求。

![帳戶的共用責任](../media/assurance-shared-responsibility-for-accounts.png)

## <a name="microsoft-managed-accounts"></a>受 Microsoft 管理的帳戶

**服務小群組帳戶** 是由開發及維護 Microsoft 365 服務的 Microsoft 365 服務小組人員使用。 這些帳戶不具備 Microsoft 365 服務的特殊許可權存取權，而是可用於要求暫時和有限的許可權存取，以執行指定的工作功能。 並非每個服務小群組帳戶都可以執行相同的動作，但使用以角色為基礎的存取控制 (RBAC) 強制進行責任的分隔。 角色可確保服務小組成員和其帳戶只具備執行特定工作職責所需的最低存取權。 此外，服務小群組帳戶不能隸屬于多個角色，在這些角色中，他們可以做為自己動作的核准者。

在透過自動化程式與其他服務通訊時，Microsoft 365 服務會使用 **服務帳戶** 進行驗證。 就像服務小群組帳戶只會獲得執行特定人員工作職責所需的最低存取權之外，服務帳戶只會授與其預定用途所需的最低存取權。 此外，還有多種類型的服務帳戶可用於滿足特定需求。 一個 Microsoft 365 服務可以有多個服務帳戶，每個帳戶都具有不同的角色以執行。

## <a name="customer-managed-accounts"></a>受客戶管理的帳戶

**客戶帳戶** 是用來存取 Microsoft 365 服務，且是每位客戶都負責的帳戶。 客戶在組織中建立及管理帳戶的責任，以維護安全的環境。 管理客戶帳戶是透過 Azure Active Directory (AAD) 或與內部部署 Active Directory (AD) 進行的同盟。 每個客戶都有一組獨特的存取控制需求，必須符合這些需求，而且客戶帳戶會授與每個客戶滿足其個人需求的能力。 客戶帳戶無法存取其客戶組織之外的任何資料。

## <a name="service-team-account-management"></a>服務小群組帳戶管理

Microsoft 365 會使用名為身分識別管理 (IDM) 的帳戶管理系統，在其整個生命週期中管理服務小群組帳戶。 IDM 會結合使用自動驗證程式和管理核准，以強制執行與服務小群組帳戶存取相關的安全性需求。

服務小組成員不會自動取得服務小群組帳戶，他們必須先符合資格需求，並取得授權的管理員核准。 若要獲得服務小群組帳戶的資格，服務小組人員必須先進行 [雇傭前人員篩選](assurance-pre-employment-screening.md)、 [雲端背景檢查](assurance-cloud-background-check.md)，並完成所有標準及必要的角色型訓練。 一旦符合所有資格需求，便可要求服務小群組帳戶的要求，且必須由授權的主管進行核准。

![人員篩選過程](../media/assurance-personnel-screening-process.png)

IDM 也負責追蹤維護服務小群組帳戶所需的定期 rescreening 和訓練。 每兩年都必須完成 Microsoft 雲端背景檢查，所有訓練材料都必須每年檢查一次。 如果到期日未滿足上述其中一項需求，便會撤銷其資格，並自動停用服務小群組帳戶。

此外，服務小群組帳戶資格也會由 [人員轉接和終止](assurance-employee-transfer-termination.md)功能自動更新。 在人力資源資訊系統 (HRIS 中所做的變更) 觸發 IDM 以採取動作，這會視情況而異。 轉接至另一個服務小組的人員將會為其 eligibilities 設定到期日，而且必須由服務小組成員提交，並由其新管理員核准，以維護 eligibilities 的要求。 終止的人員會自動將所有 eligibilities 撤銷，並在過去一天停用其服務小群組帳戶。 可對 involuntary 終止進行帳戶撤銷的緊急要求。

根據預設，服務小群組帳戶對用於定期疑難排解的廣泛系統中繼資料具有有限的讀取權限。 此外，「基準服務小群組帳戶」無法要求 Microsoft 365 或客戶資料的特殊許可權存取權。 您必須針對服務小群組帳戶進行另一個要求，才能將服務小群組帳戶新增至允許服務小組成員要求更高許可權，以執行特定工作和作業的角色。
