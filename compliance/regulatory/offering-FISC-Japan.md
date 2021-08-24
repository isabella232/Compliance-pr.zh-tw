---
title: 金融業資訊系統中心 (FISC)
description: Microsoft 符合日本金融業資訊系統第 8 版標準的需求。
keywords: Microsoft 365, 合規性, 方案
ms.localizationpriority: high
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: f1eba3e819ae351f1bdff2f8fbdd47c7fca7a1a1
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482226"
---
# <a name="center-for-financial-industry-information-systems-fisc"></a>金融業資訊系統中心 (FISC)

## <a name="fisc-overview"></a>FISC 概觀

金融業資訊系統中心 (FISC) 是由日本財務省於 1984 年成立的非營利組織，旨在提升日本銀行電腦系統的安全性。 日本大約有 700 家公司支持此組織，包括主要的金融機構、保險和信貸公司、證券公司、電腦製造商和電信企業。

FISC 與其成員機構、日本銀行和金融服務局 (負責監督日本銀行、證券和交易，以及保險的政府組織) 合作，制定了銀行資訊系統安全性的準則。 其中包括適用於電腦系統控制的基本稽核標準、發生重大災難時的應急規劃，以及開發內含超過 300 個控制的安全性原則和標準。

雖然法規沒有要求在雲端運算環境中應用這些準則，但是日本大多數實作雲端服務的金融機構已建立了符合這些安全性標準的資訊系統，並且難以證明與它們相背離。 (2015 年發布的最新準則第 8 版補充修訂版增加了兩個修訂版，涉及金融機構對雲端服務的使用，以及針對網絡攻擊的對策。)

法規不要求符合此架構，並且未經 FISC 稽核或驗證。

## <a name="microsoft-and-fisc"></a>Microsoft 和 FISC

Microsoft 已聘雇外部評估員來驗證 Microsoft Azure、Dynamics 365 和 Microsoft Office 365 是否符合 FISC 金融機構電腦系統安全性準則第 9 版修訂版的需求。Microsoft 提供下列各個領域的合規性證據：

- 建築物和電腦機房、電源、空調、資料中心和設施監視的資料中心準則。
- 組織、訓練、存取控制、系統開發和稽核的操作準則。
- 改善硬體和軟體可靠性，以及防範安全風險 (包括資料保護、防範未經授權的使用、威脅偵測，以及災難復原) 的措施技術準則。

金融機構可以依賴下列評估：評估 Azure、Dynamics 365、Office 365 和 Microsoft Cloud App Security 的範圍內基礎架構和平台服務是否符合這三個區域。

[深入了解外部評估者的驗證和評估者網站連結 (僅提供日文)](https://cloudblogs.microsoft.com/industry-blog/ja-jp/financial-services/2018/05/11/fisc_v9/)。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- Intune
- Microsoft 雲端應用程式安全性
- Office 365
- Power BI 雲端服務 (可作為獨立服務或包含在 Office 365 品牌方案或套件中)

## <a name="office-365-and-fisc"></a>Office 365 和 FISC

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | Access Online、Azure Active Directory、Delve、Exchange Online、Exchange Online Protection、Microsoft Teams、Office 365 專業增強版、Office Online、商務用 OneDrive、Power BI for Office 365、Project Online、SharePoint Online、商務用 Skype |

## <a name="frequently-asked-questions"></a>常見問題集

**誰適用 FISC 準則？**

日本的銀行和其他金融機構若要驗證其在系統安全性、可靠性和稽核方面的方法，並與日本已建立的最佳做法保持一致，請遵循 FISC 準則。

**哪裡可以取得第 8 版 FISC 需求的詳細資訊？**

FISC 已發佈兩份來自其專家委員會的報告：

- [金融機構使用雲端運算的情況](https://aka.ms/cloud-computing-report-en)
- [金融機構防範網路攻擊的對策](https://aka.ms/cyberattack-counter)

**哪裡可以取得 Microsoft 回應 FISC 架構的詳細資料？**

如需協力廠商評估 Microsoft 雲端服務 FISC 合規性的安全性參考，請與您的 Microsoft 帳戶代表聯繫。

**我是否可以在組織的資格程序中使用 Microsoft 對此架構的回應？**

是的。不過，雖然 Microsoft 對此架構的回應是由協力廠商確認，但客戶負責驗證其已在 Azure 或 Office 365 上實作的解決方案合規性。

## <a name="resources"></a>資源

- [Microsoft Online Services 條款](https://aka.ms/Online-Services-Terms)
- [FISC 安全性準則/安全標準](https://www.fisc.or.jp/english)
- [有關使用雲端運算的 FISC 報告](https://aka.ms/cloud-computing-report-en)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)

## <a name="resources-in-japanese"></a>日本的資源

- [FISC](https://www.fisc.or.jp/)
