---
title: NIST SP 800-171
description: Microsoft 雲端服務遵循 NIST SP 800-171 指導方針，以保護 nonfederal 資訊系統中受控制的未分類資訊 (CUI) 。
keywords: Microsoft 365, 合規性, 方案
ms.localizationpriority: medium
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
ms.openlocfilehash: bce6847fe4c0cd1541348b70aadacc9c13238c31
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481135"
---
# <a name="nist-sp-800-171"></a>NIST SP 800-171

## <a name="about-nist-sp-800-171"></a>關於 NIST SP 800-171

美國國家標準和技術協會 (NIST) 會促進及維護度量標準和準則，以協助保護聯邦機構的資訊和資訊系統。 如需管理受控未分類資訊的管理順序 13556 (CUI) ，它已發佈 [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-1/final)， *保護 Nonfederal 資訊系統和組織中的受控未分類資訊*。 CUI 是定義為由政府 (或其代表) 所建立的資訊，但不是保密的，但仍然機密且需要保護。

NIST SP 800-171 最初發佈于6月2015，已于此後更新數次，以回應演變的 cyberthreats。 它提供有關如何在 nonfederal 資訊系統和組織中安全地存取、傳送和儲存 CUI 的指導方針;其需求分為四個主要類別：

- 管理及保護的控制項和程式
- IT 系統的監控與管理
- 適用于使用者的清晰做法和程式
- 技術和實體安全性措施的實施

## <a name="microsoft-and-nist-sp-800-171"></a>Microsoft 和 NIST SP 800-171

已取得協力廠商評估組織，Kratos Secureinfo 和 Coalfire，與 Microsoft 合作以證明其範圍內的雲端服務符合 NIST SP 800-171 中的準則， *保護受控未分類資訊 (CUI) 在 Nonfederal 資訊系統和組織中* 處理 CUI。 [Microsoft 對 FedRAMP](offering-fedramp.md)需求的實施，可協助確保 Microsoft 內部的雲端服務使用已到位的系統和做法，符合或超過 NIST SP 800-171 的需求。

NIST SP 800-171 的需求是 NIST SP 800-53 （FedRAMP 使用的標準）的子集。 NIST SP 800-171 的附錄 D 可將其 CUI 安全性需求直接對應至 NIST SP 800-53 中的相關安全性控制，其範圍內的雲端服務已在 FedRAMP 程式下評估並授權。

任何處理或儲存我們政府 CUI 的實體（調研機構、諮詢公司、製造合同工）都必須遵守 NIST SP 800-171 的嚴格需求。 這項證明意味著 Microsoft in 範圍的雲端服務可讓客戶在尋求部署 CUI 工作負載時，確保 Microsoft 符合完全規範。 例如，在其資訊系統中使用內部範圍的 Microsoft 雲端服務處理、儲存或傳輸「涵蓋的防禦資訊」的所有 DoD 承包商，都符合美國國防部 DFARS 子句，需要符合 NIST SP 800-171 的安全性需求。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure 商用，Azure 政府版
- 美國政府的 Dynamics 365
- Intune
- Office 365U.S. 政府社群雲端 (GCC) 、Office 365 GCC 高及 DoD

## <a name="azure-dynamics-365-and-nist-sp-800-171"></a>Azure、Dynamics 365 和 NIST SP 800-171

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE NIST SP 800-171 服務](/azure/compliance/offerings/offering-nist-800-171)。

## <a name="office-365-and-nist-sp-800-171"></a>Office 365 和 NIST SP 800-171

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **GCC** | 活動摘要服務，Bing 服務，Delve，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink |
| **GCC High** | 活動摘要服務，Bing 服務，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、 
SharePoint線上、商務用 Skype Windows Ink |
| **DoD** | 活動摘要服務，Bing 服務，Exchange Online，智慧服務，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用方式報告、商務用 OneDrive、人員卡片、Microsoft Teams、SharePoint 線上、商務用 Skype Windows Ink |

### <a name="frequently-asked-questions"></a>常見問題集

**我可以使用 Microsoft 對我的組織使用 NIST SP 800-171 的規範嗎？**

是。 Microsoft 客戶可以使用來自獨立協力廠商評估組織的報告中所述的審核控制項， (3PAO) FedRAMP 標準的一部分 FedRAMP 及 NIST 風險分析和資格工作。 這些報告證明 Microsoft 已在其範圍內雲端服務中實施之控制項的效能。 客戶負責確保其 CUI 工作負載符合 NIST SP 800-171 指導方針。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [Microsoft DoD 認證符合 NIST 800-171 的需求](offering-DoD-DISA-L2-L4-L5.md)
- [NIST 800-171 合規性始于 Cybersecurity 檔](https://www.nist800171.com/)
- [Microsoft Cloud Services FedRAMP 授權](https://marketplace.fedramp.gov/index.html?status=Compliant&sort=productName#/products)
- [NIST 800-171 3.3 審計和責任制 Office 365 GCC 高](https://info.summit7systems.com/blog/nist-3.3-audit-and-accountability-with-office-365)
- [Microsoft 和 NIST Cybersecurity Framework](offering-nist-csf.md)
- [Microsoft 政府雲端](https://www.microsoft.com/enterprise/government)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
