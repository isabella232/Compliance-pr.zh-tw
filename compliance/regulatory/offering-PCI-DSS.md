---
title: 支付卡行業 (PCI) 資料安全標準 (DSS)
description: Azure、SharePoint Online 和商務用 OneDrive 符合支付卡行業資料安全標準第 1 級 3.2 版。
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
ms.openlocfilehash: 09c18fce6544984a7e9d639e68d0f0201c584768
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158876"
---
# <a name="payment-card-industry-pci-data-security-standard-dss"></a>支付卡行業 (PCI) 資料安全標準 (DSS)

## <a name="pci-dss-overview"></a>PCI DSS 概觀

支付卡行業 (PCI) 資料安全標準 (DSS) 是一個全球資訊安全性標準，旨在透過進一步控制信用卡資料來防止詐欺行為。 任何規模的組織在接受來自五大信用卡品牌 (Visa、MasterCard、American Express、Discover 及 Japan Credit Bureau (JCB)) 的付款卡時，都必須遵循 PCI DSS 標準。 任何儲存、處理或傳輸付款和持卡人資料的組織皆需符合 PCI DSS 規範。

## <a name="microsoft-and-pci-dss"></a>Microsoft 和 PCI DSS

Microsoft 已透過經核准的合格資安評估商 (QSA) 完成年度 PCI DSS 評估。 審查員已審查 Microsoft Azure、Microsoft 商務用 OneDrive 和 Microsoft SharePoint Online 環境，其中包括驗證基礎結構、開發、作業、管理、支援和範圍內服務。 PCI DSS 根據交易量指定 4 個合規性等級。 Azure、商務用 OneDrive 和 SharePoint Online 通過服務提供者第 1 級 PCI DSS 3.2 版認證 (最高交易量，一年超過 600 萬)。

評估會提供合規性證明 (AoC) 供客戶使用，以及 QSA 發出的合規性報告 (RoC)。 合規性的有效期從通過審核及收到評估商提供的 AoC 開始，並在 AoC 簽署日一年後結束。 

想要開發持卡人環境或支付卡處理服務的客戶可在許多基礎部分使用這些驗證，從而降低自行取得 PCI DSS 認證的相關工作量和成本。

請注意，Azure、商務用 OneDrive 和 SharePoint Online 的 PCI DSS 合規性狀態不會自動轉換成客戶在這些平台上建立或託管的服務的 PCI DSS 認證。 客戶需負責確保符合 PCI DSS 要求。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure 和 Azure Government
- Intune
- Microsoft 雲端應用程式安全性
- [適用於端點的 Microsoft Defender](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-advanced-threat-protection)
- Microsoft Graph
- Office 365
- 商務用 OneDrive 和 SharePoint Online (僅限美國)
- PPowerApps 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中
- 電源自動化 (可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中)
- Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中

## <a name="azure-dynamics-365-and-pci-dss"></a>Azure、Dynamics 365 和 PCI DSS

如需 Azure、Dynamics 365 及其他線上服務合規性的詳細資訊，請參閱 [Azure PCI DSS 供應項目](/azure/compliance/offerings/offering-pci-dss)。

## <a name="office-365-and-pci-dss"></a>Office 365 和 PCI DSS

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | 商務用 OneDrive (美國)、SharePoint Online |

### <a name="office-365-audit-reports-and-certificates"></a>Office 365 稽核、報告和認證

- [商務用 OneDrive 和 SharePoint Online PCI DSS 合規性證明 (AoC)](https://aka.ms/spo-pci)

### <a name="frequently-asked-questions"></a>常見問題集

**為什麼合規性證明 (AoC) 封面頁顯示「2018 年 6 月」？**

封面頁上的 2018 年 6 月日期是發佈 AoC 範本的時間。 如需評估的日期，請參閱第 2 節。 

**PA DSS 和 PCI DSS 之間的關聯是什麼？**

支付應用程式資料安全標準 (PA DSS) 是符合 PCI DSS 的一組要求，且取代 Visa 的支付應用程式最佳實務，並合併其他主要發卡機構的合規性要求。 PA DSS 可協助軟體廠商開發協力廠商應用程式，在卡片授權或結算程序中儲存、處理或傳輸持卡人付款資料。 零售商必須使用 PA DSS 認證應用程式以有效地達到其 PCI DSS 合規性。 PA DSS 不適用於 Azure。

**什麼是收單行？Azure 使用收單行嗎？**

收單行是處理支付卡交易的銀行或其他實體。 Azure 不會以服務提供支付卡處理，因此不會使用收單行。

**PCI DSS 適用於哪些組織和商家？**

PCI DSS 適用於任何接受、傳輸或儲存持卡人資料的公司，無論規模或交易次數。 也就是說，如果任何客戶使用信用卡或轉帳卡付款給某公司，便適用 PCI DSS 要求。 系統會根據 12 個月內的總交易量，以四個層級中的其中一個層級驗證公司。 第 1 級適用於每年處理超過 600 萬筆交易的公司；第 2 級適用於 100 萬至 600 萬筆交易；第 3 級適用於 20,000 至 1 百萬筆交易；而第 4 級則適用於少於 20,000 筆交易。

**美國以外的國家/地區是否有符合 PCI DSS 規範的商務用 OneDrive 和 SharePoint Online 方案？**

目前符合 PCI DSS 規範的商務用 OneDrive 和 SharePoint Online 僅限美國。 Microsoft 會評估美國以外地區的需求和時間表，並在其他地區新增至藍圖時提供更新。

**[商務用 OneDrive] 和 [SharePoint Online] 的適用範圍為何？**

目前，只有上傳至 [商務用 OneDrive] 和 [SharePoint Online] 的檔案和文件符合 PCI DSS 的要求。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評定風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [PCI 安全標準協會](https://www.pcisecuritystandards.org/)
- [PCI 資料安全性標準](https://www.pcisecuritystandards.org/documents/PCI_DSS_v3-1.pdf)
- [PCI DSS 快速參考指南](https://www.pcisecuritystandards.org/documents/PCISSC%20QRG%20August%202014%20-print.pdf)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
