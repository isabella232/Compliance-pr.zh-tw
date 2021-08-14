---
title: '狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) '
description: Azure 和 Office 365 會驗證健康資訊信任同盟 (HITRUST) 常見的安全性框架 (CSF) 。
keywords: Microsoft 365, 合規性, 方案
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
ms.openlocfilehash: e910593e80c49acf7f1e94c9ade74fb51f225912
ms.sourcegitcommit: 01938022a292c07e98041dc6ae1312a1b8c617db
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260697"
---
# <a name="health-information-trust-alliance-hitrust-common-security-framework-csf"></a>狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) 

## <a name="hitrust-csf-overview"></a>HITRUST CSF 一覽

狀況資訊信任同盟 (HITRUST) 是由醫療保健行業的代表所管理的組織。 HITRUST 建立並維護常見的安全性框架 (CSF) ，一種 certifiable 架構，可協助醫療保健組織及其提供者示範其安全性和符合性，以一致且簡潔的方式。

CSF 建立于 HIPAA 和高科技法案，這是美國醫療保健法，已針對個別身分識別健康資訊的使用、披露和保護，以及強制執行不相容的要求。 HITRUST 提供一個基準-標準化的規範架構、評估和認證程式，讓雲端服務提供者和涵蓋的健康情況實體可以測量規范。 CSF 也會將這類現有架構的醫療保健特定安全性、隱私權及其他法規需求納入到支付卡行業資料安全性標準 ([PCI-DSS](https://www.microsoft.com/trustcenter/compliance/pci)) 、 [ISO/IEC 27001](https://www.microsoft.com/trustcenter/compliance/iso-iec-27001) 資訊安全性管理標準，以及 ([火星-E](https://www.microsoft.com/trustcenter/compliance/mars-e)) 的最小可接受風險標準。

CSF 分為19個不同的網域，包括 endpoint protection、行動裝置安全性和存取控制。 HITRUST 會針對這些控制項來驗證 IT 產品。 HITRUST 也會根據組織、系統和法規因素，改編組織風險的認證需求。

狀況資訊信任同盟 (HITRUST) 常見的安全性架構 (CSF) 

HITRUST 提供三種確定性或評估等級：自我評估、CSF 驗證及 CSF 認證。 每個層級組建都會在其下一個層級上增加嚴謹。 最高層次的組織，CSF 認證，符合 CSF 的所有認證需求。 Microsoft Azure 和 Office 365 是第一個超大型雲端服務，可接收 HITRUST CSF 的認證。 Coalfire，HITRUST assessor 公司，根據 Azure 和 Office 365 如何執行安全性、隱私權和法規需求，以保護機密資訊，來執行評估。 Microsoft 支援 HITRUST 共用責任計畫。

瞭解如何使用 Azure 安全性和合規性藍圖加速您的 HITRUST 部署。

[ (CRM) 藍圖 HITRUST，下載 Microsoft Azure 的客戶責任矩陣](https://servicetrust.microsoft.com/ViewPage/Blueprint?command=Download&downloadType=Document&downloadId=3ccde498-4761-4be0-be8b-cd8d379a3a4f&docTab=fc060920-cdb8-11e7-bacf-0bf52b09d912_Healthcare_Blueprint)

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure 和 Azure Government
- Intune
- [Microsoft 受管理的電腦](/microsoft-365/managed-desktop/intro/compliance)
- Office 365

## <a name="azure-dynamics-365-and-hitrust"></a>Azure、Dynamics 365 和 HITRUST

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE HITRUST 服務](/azure/compliance/offerings/offering-hitrust)。

## <a name="office-365-and-hitrust"></a>Office 365 和 HITRUST

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | 活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink |

### <a name="office-365-audits-reports-and-certificates"></a>Office 365 稽核、報告和認證

Office 365 的 HITRUST CSF 證書是兩年有效。

- [Office 365憑證的 HITRUST 字母](https://aka.ms/O365HITRUSTcertification)

### <a name="frequently-asked-questions"></a>常見問題集

**為什麼有些 Office 365 服務不在此認證的範圍內？**

Microsoft 提供最全面的選項，與其他雲端服務提供者相較。 為了維持跨地區和行業的廣泛合規性服務，我們根據市場需求、客戶意見反應及產品生命週期，在我們的保證工作範圍內加入服務。 如果服務並未包含在特定規范產品的目前範圍內，則您的組織有責任根據您的合規性義務評估風險，並決定處理該服務中資料的方式。 我們會持續收集客戶的意見反應，與管理機構和審計員合作，以擴大我們的安全性和合規性需求。

**Microsoft 憑證表示如果我的組織使用 Office 365，它符合 HITRUST CSF？**

當您將資料儲存在 Office 365 的 SaaS 中時，Microsoft 與您組織之間的共同責任，以達成法規。 Microsoft 會管理大部分的基礎結構控制，包括實體安全性、網路控制、應用層級控制等，而且您的組織有責任管理存取控制和保護您的敏感性資料。 Office 365 HITRUST 認證示範 Microsoft 的控制架構合規性。 為此，您的組織必須實施及維護您自己的資料保護控制，以符合 HITRUST CSF 需求。

**當使用 Office 365 時，Microsoft 是否會為我的組織提供指導，以執行適當的控制項？**

是的，您可以在合規性分數中尋找建議的客戶動作，以協助您的組織在使用雲端服務時符合複雜的合規性義務。 具體說來，針對 HITRUST CSF，我們建議您使用 NIST 800-53 和 NIST CSF 評估遵循合規性分數來執行風險評估。 在評估中，我們為您提供逐步指導方針，以及您可以用來實施資料保護控制的 Microsoft 解決方案。 您可以深入瞭解 [Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)中的合規性分數。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何 [在合規性管理員中建立及管理評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [HITRUST 同盟](https://hitrustalliance.net/)
- [HITRUST CSF 9。3](https://hitrustalliance.net/csf-license-agreement/)
- [瞭解和利用 CSF](https://hitrustalliance.net/understanding-leveraging-csf/)
- [進一步瞭解 HITRUST 共用責任計畫](https://go.microsoft.com/fwlink/p/?linkid=2100268)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
