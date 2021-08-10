---
title: 美國內年收入服務出版物1075
description: Microsoft 的控制措施符合美國內部收入服務出版物1075的需求。
keywords: Microsoft 365、合規性、方案
localization_priority: None
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
ms.openlocfilehash: 6406c63d73e30a62d3cbe54bf8cef632cc5564b2cae3d1a9588652644b8f8c96
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54293900"
---
# <a name="us-internal-revenue-service-publication-1075"></a>美國內年收入服務出版物1075

## <a name="us-internal-revenue-service-publication-1075-overview"></a>美國內部收入服務出版物1075概述

Internal 創收服務出版物 1075 (IRS 1075) 提供美國政府代理商和其代理商用來存取聯邦稅收資訊 (FTI) 的指導方針，以確保他們使用原則、作法和控制措施來保護其機密性。 IRS 1075 的目的是為了降低因外部政府機構所持有之 FTI 所造成的遺失、破壞或誤用風險。 例如，用來處理某位居民的稅收傳回的狀態部門（或存取 FTI 的健康情況服務中心），必須具備適當的程式，以保護該資訊。  
  
為了保護 FTI，IRS 1075 規定了應用程式、平臺及資料中心服務的安全性和隱私權控制。 例如，它會排定資料中心活動的安全性，例如正確處理 FTI，以及資料中心承包商的監察能力來限制專案。 為了確保接收到的政府代理商套用到這些控制，IRS 已建立了安全保護計劃，其中包括定期檢查這些機構及其承包商。

## <a name="microsoft-and-us-internal-revenue-service-publication-1075"></a>Microsoft 和 US 內部收入服務出版物1075

Microsoft Azure政府和[Microsoft Office 365 美國政府](https://products.office.com/government/office-365-web-services-for-government)雲端服務會提供合約承諾，讓他們具備適當的控制措施，以及 Microsoft agency 客戶符合 IRS 1075 的實體需求所需的安全性功能。  
  
這些適用于政府的 Microsoft 雲端服務提供一個平臺，客戶可以在其中建立及操作其解決方案，但是客戶必須自行決定是否要根據 IRS 1075 運作特定的解決方案，因此，也就是在進行 IRS 審計時使用。  
  
為了協助政府機構在其法規遵從性工作中，Microsoft：

- 提供詳細的指導，以協助各機構瞭解他們的責任，以及如何對應到 Azure 政府及 Office 365 美國政府的功能。 IRS 1075 防護安全性報告 (SSR) 完整檔 Microsoft 服務如何執行適當的 IRS 控制，並根據 Azure 政府和 Office 365 美國政府的 FedRAMP 套件。 因為 IRS 1075 和 FedRAMP 都是以 NIST 800-53 為基礎，所以 IRS 1075 的相容性界限與 FedRAMP 授權相同。
- IRS 必須明確核准任何 IRS 防護檔的發行，所以只有保密協定下的政府客戶才能檢查 SSR。
- 針對其雲端服務，提供可供獨立評估者的審計報告及監控資訊。
- 提供對應的 Azure 政府合規性考慮，以及 Office 365 美國政府合規性考慮，其概括了代理商如何使用 Microsoft 雲端政府服務的方式，遵循 IRS 1075 的方式。 保密協定下的政府客戶可以要求這些檔。
- 在需要時，向客戶供應商機 (，以與 Microsoft 主題專家或外部審計員) 進行通訊。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

根據 NIST 指導方針，以三個影響層級授與 FedRAMP 授權：低、中和高。 這些排名可影響組織的機密性、完整性或可用性喪失的程度，也就是低 (有限的效果) 、中 (嚴重的不利影響) ，以及高 (嚴重或嚴重影響) 。

- Azure 和 Azure Government
- 美國政府的 Dynamics 365
- Office 365，Office 365 美國政府
- Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中

## <a name="azure-dynamics-365-and-irs-1075"></a>Azure、Dynamics 365 和 IRS 1075

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE IRS 1075 產品](/azure/compliance/offerings/offering-irs-1075)。

## <a name="office-365-and-irs-1075"></a>Office 365 和 IRS 1075

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **Office 365** | 活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 使用狀況報告、商務用 OneDrive、人員卡片、服務基礎結構、SharePoint 線上、商務用 Skype、Windows Ink |
| **GCC** | 活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告，商務用 OneDrive，人員卡片，SharePoint 線上，商務用 Skype，Windows Ink |

### <a name="office-365-audits-reports-and-certificates"></a>Office 365 稽核、報告和認證

遵守 IRS 1075 的實體需求涵蓋每年 FedRAMP 的審計。

- [FedRAMP 授權](https://marketplace.fedramp.gov/#/product/azure-government?sort=productName&productNameSearch=azure)

### <a name="frequently-asked-questions"></a>常見問題集

**Microsoft 如何滿足 IRS 1075 的需求？**

Microsoft 會定期監視其安全性、隱私權、運作控制措施和 NIST 800-53 rev。 FedRAMP 一般影響資訊系統的比較基準所要求的4個控制項。 透過連續的監控報告可提供對此資訊的季度存取。 Azure 政府和 Office 365 美國政府客戶可以透過[服務信任入口網站](https://aka.ms/stphelp)來存取這種機密的合規性資訊。

此外，Microsoft 已承諾為 Azure 政府和 Office 365 美國政府等其主要控制組中包含 IRS 1075 控制項，並每年進行審計。

**我可以查看 FedRAMP 套件或系統安全性計畫嗎？**

是的，如果您的組織符合 Azure 政府和 Office 365 美國政府的資格需求。 請直接聯繫您的 Microsoft 客戶代表以查看這些檔。 您也可以參閱相容的雲端服務提供者的 FedRAMP 清單。

**我可以使用 Azure 或 Office 365 公用雲端環境，是否仍然相容于 IRS 1075？**

錯誤。 可以儲存並處理的唯一環境是 Azure 政府或 Office 365 美國政府。 政府客戶必須符合資格的要求才能使用這些環境。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [IRS 出版物1075](https://www.irs.gov/pub/irs-pdf/p1075.pdf)
- [IRS 安全措施計畫](https://www.irs.gov/uac/Safeguards-Program)
- [Microsoft 通用控制措施中樞合規性架構](https://www.microsoft.com/trust-center/compliance/compliance-overview)
- [適用於政府的 Microsoft 雲端](https://azure.microsoft.com/global-infrastructure/government/)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
