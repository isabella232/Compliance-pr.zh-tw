---
title: 資訊安全性控制的 ISO/IEC 27017:2015 工作條例規定
description: Microsoft 雲端服務已實作此「資訊安全性控制的工作條例規定」。
keywords: Microsoft 365, 合規性, 方案
localization_priority: Priority
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
ms.openlocfilehash: 54ae2345f72e6ea0b9b0e856721acc7ff6590e52
ms.sourcegitcommit: 01938022a292c07e98041dc6ae1312a1b8c617db
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260475"
---
# <a name="isoiec-270172015-code-of-practice-for-information-security-controls"></a>資訊安全性控制的 ISO/IEC 27017:2015 工作條例規定

## <a name="iso-iec-27017-overview"></a>ISO-IEC 27017 概觀

ISO/IEC 27017:2015 工作條例規定專為組織設計，可在基於 ISO/IEC 27002:2013 實作雲端運算資訊安全管理系統時，用來做為選取雲端服務資訊安全性控制的參考。 雲端服務提供者也可以使用它做為實作常見防護控制的指導方針文件。

此國際標準提供基於 ISO/IEC 27002 的額外雲端特定實作指導方針，並提供額外的控制來處理雲端特定資訊安全性威脅和風險，請查閱 ISO/IEC 27002:2013 的條款 5 至 18 中相關的控制、實作指導方針及其他資訊。 具體來說，此標準提供 ISO/IEC 27002 中 37 項控制的指導方針，並提供未與 ISO/IEC 27002 中重複的七項新控制。 這些新的控制能解決下列重要領域：

- 雲端運算環境內的共同角色和責任
- 在合約終止時移除並退回雲端服務客戶資產
- 保護客戶的虛擬環境並與其他客戶的虛擬環境隔離
- 虛擬機器強化需求，以滿足商務需求
- 雲端運算環境系統管理操作的程序
- 讓客戶能夠監視雲端運算環境內的相關活動
- 結合虛擬和實體網路的安全性管理

## <a name="microsoft-and-isoiec-27017"></a>Microsoft 和 ISO/IEC 27017

ISO/IEC 27017 在為雲端服務提供者和雲端服務客戶提供指導方針方面與眾不同。 它也會為雲端服務客戶提供有關他們應該對雲端服務提供者所預期的實務資訊。 透過確保客戶了解在雲端中的共用責任，客戶可以直接從 ISO/IEC 27017 獲益。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- [Azure、Azure Government 和 Azure 德國](https://aka.ms/AzureCompliance)
- Microsoft Cloud App Security
- [Dynamics 365、Dynamics 365 和 Dynamics 365 德國](https://aka.ms/d365-compliance-list)
- Intune
- 適用於端點的 Microsoft Defender
- Microsoft Graph
- Microsoft Healthcare Bot
- [Microsoft 受管理的電腦](/microsoft-365/managed-desktop/intro/compliance)
- Office 365、Office 365 美國政府、Office 365 美國政府國防版和 Office 365 Germany
- Power Automate (先前為 Microsoft Flow) 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中
- PowerApps 雲端服務可作為獨立服務或包含在 Office 365 或 Dynamics 365 品牌方案或套件中
- Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中
- Power BI Embedded

## <a name="azure-dynamics-365-and-iso-270172015"></a>Azure、Dynamics 365 和 ISO 27017:2015

如需 Azure、Dynamics 365 及其他線上服務合規性的詳細資訊，請參閱 [Azure ISO 27017 供應項目](/azure/compliance/offerings/offering-iso-27017)。

## <a name="office-365-and-iso-270172015"></a>Office 365 和 ISO 27017:2015

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | Access Online、Azure Active Directory、Azure Communications Service、合規性管理員、客戶加密箱、Delve、Exchange Online、Exchange Online Protection、Forms、Griffin、Identity Manager、Lockbox (Torus)、Microsoft Defender for Office 365、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 客戶入口網站、Office 365 微服務 (包含但不限 Kaizala、ObjectStore、Sway、PowerPoint Online Document Service、Query Annotation Service、學校資料同步處理、Siphon、Speech、StaffHub、eXtensible Application Program)、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、Office Services Infrastructure、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、Project Online、使用客戶金鑰的服務加密、SharePoint Online、商務用 Skype、Stream |
| **GCC** | Azure Active Directory、Azure Communications Service、合規性管理員、Delve、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、MyAnalytics、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype、Stream |
| **GCC High** | Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、PowerApps、Power Automate、Power BI、SharePoint Online、商務用 Skype |
| **DoD** | Azure Active Directory、Azure Communications Service、Exchange Online、Forms、適用於 Office 365 的 Microsoft Defender、Microsoft Teams、Office 365 進階合規性附加元件、Office 365 安全性與合規性中心、Office Online、Office 專業增強版、商務用 OneDrive、Planner、Power BI、SharePoint Online、商務用 Skype |

### <a name="office-365-audits-reports-and-certificates"></a>Office 365 稽核、報告和認證

Microsoft 雲端服務會每年隨著 ISO/IEC 27001:2013 的認證程序，針對 ISO/IEC 27017:2015 工作條例規定進行一次稽核。

- [Office 365：ISO 27001、27018 和 27017 稽核評估報告](https://aka.ms/o365isoreport)

### <a name="frequently-asked-questions"></a>常見問題集

**該標準適用於誰？**

此工作條例規定可提供雲端服務提供者和雲端服務客戶的控制和實作指導方針。 它的結構格式類似於 ISO/IEC 27002:2013。

**可以在何處檢視 Microsoft 的 ISO/IEC 27017:2015 合規性資訊？**

您可以下載適用於 Azure、Intune 和 Power BI 的 [ISO/IEC 27017:2015 認證](https://aka.ms/azureiso27017)。

**我是否可以在組織的認證程序中使用 Microsoft 服務的 ISO/IEC 27017 合規性？**

是。 如果貴公司正在尋求用於在任何 Microsoft 範圍內企業雲端服務上所部署實作的認證，則可以在您的合規性評定中使用 Microsoft 的相關認證。 不過，您有責任確保處理者有參與評估合規性的實作，以及組織中的控制和程序。

**如何取得適用稽核報告的複本？**

[服務信任入口網站](https://aka.ms/stphelp)提供獨立的協力廠商稽核報告和其他相關文件。 您可以使用入口網站來下載並檢閱此文件，以獲得您自己的法規需求的協助。

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

### <a name="resources"></a>資源

- [ISO/IEC 27017:2015 工作條例規定](https://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43757)
- [Microsoft Online Services 條款](https://aka.ms/Online-Services-Terms)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
