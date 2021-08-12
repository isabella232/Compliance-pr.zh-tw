---
title: 架構概觀
description: 深入瞭解 Microsoft 365 中的架構
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
ms.openlocfilehash: ca26f1cb12fd7440b143ec27f7abfb1977acc0a2addc71baa3e265d262aeb57a
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54289241"
---
# <a name="architecture-overview"></a>架構概觀

## <a name="what-are-microsoft-online-services"></a>什麼是 Microsoft online 服務？

Microsoft 線上服務參考 Microsoft 所提供的雲端架構服務，其中包含 Azure、Dynamics 365 和 Microsoft 365。  每個服務都會針對一般商務作業和生產力需求提供獨特的解決方案，為全球各地的客戶提供服務，而不是從小型企業到大型企業和政府。 由 Microsoft 獨立管理的網路基礎結構所連接的全域分散式資料中心，可充當支援線上服務的主幹，可提供幾乎所有狀況的功能，並可承受廣泛的全球需求。

所有的 Microsoft 線上服務都有相同的目標，可保護其所管理的服務基礎結構及其客戶的資料，但是每個線上服務都是由個別的業務單位運作。 在許多情況下，安全性控制是以相同的方式在所有服務上實施，但在某些情況下，他們採取不同的方法來滿足其客戶承諾和合規性義務。

## <a name="what-is-azure"></a>何謂 Azure？

Microsoft Azure 是一種雲端計算平臺，可透過 Microsoft 和協力廠商受管理的資料中心網路來建立、部署和管理應用程式。 它支援平臺為服務 (PaaS) 和基礎結構作為服務 (IaaS) 雲端服務模型，並啟用整合雲端服務與客戶內部部署資源的混合式解決方案。 Microsoft Azure 支援許多客戶、合作夥伴和政府組織，跨越各種產品和服務、地理和行業。 Microsoft Azure 的設計是為了符合安全性、機密性及規範的需求。

## <a name="what-is-dynamics-365"></a>何謂 Dynamics 365？

Dynamics 365 是一種線上商務應用程式套件，可整合客戶關係管理 (CRM) 功能及其分機，Enterprise 資源規劃 (ERP) 功能。 這些端對端商務應用程式可協助客戶將關聯性轉化為收入、贏得客戶，並加速業務成長。 Dynamics 365 是一種服務 (SaaS) 套件內建于 Azure 基礎結構上，而且透過全球分散資料中心透過全球客戶提供給世界各地的客戶。

## <a name="what-is-microsoft-365"></a>什麼是 Microsoft 365？

Microsoft 365 是雲端電源、訂閱 Office、Windows 10、Enterprise Mobility + Security 及規範的版本。 Microsoft 365 客戶取得 Outlook 和 Windows 之類的用戶端，也會受益于 Microsoft 裝載的服務，例如 Exchange Online、Microsoft Teams 和 SharePoint 線上。 服務的所有元件都會定期更新為訂閱模式的一部分，讓我們的客戶擁有「長綠」的產品。 Microsoft 會代表客戶管理服務基礎結構，這表示 Microsoft 負責保護儲存客戶資料的基礎結構。

根據規模的角度來看，Microsoft 目前使用近達一百萬台電腦來為 Microsoft 365 服務供電。 針對這些服務的基礎結構，在 Azure、Windows 和 Linux 以及多承租人和專用平臺的服務特定硬體和虛擬化環境上有很大的差異。 Microsoft 365 是全球性商品，我們的基礎結構分散於世界各地的資料中心，可讓客戶符合資料落地和主權需求。

## <a name="how-do-microsoft-online-services-ensure-isolation-between-customer-tenants"></a>Microsoft online services 如何確保客戶承租人間的隔離？

Microsoft 的雲端服務是以假設所有租使用者可能會敵意所有其他租使用者所組成。 為了正確地將承租人彼此隔離，Microsoft 會執行各種隔離技術和控制。 這些控制項的設計目的是為了避免資訊洩露或未經授權存取跨承租人的客戶資料，並防止一個承租人的動作對其他租使用者的服務造成不良影響。

在使用 Azure Active Directory (Azure AD) 的承租人內，客戶內容會以邏輯方式隔離。 Microsoft online services 中的使用者驗證不僅會驗證使用者身分識別，還會驗證使用者帳戶所屬的承租人身分識別，以防止使用者存取其租使用者環境以外的資料。 若要對 Azure AD 的邏輯隔離進行補充，客戶內容會永遠在靜止時加密，並可在傳輸中加密。 個別服務也可能會提供額外的租使用者隔離層，例如在個別的加密資料庫中 SharePoint 線上隔離租使用者資料。

## <a name="how-do-microsoft-online-services-engineer-resilient-services-that-avoid-single-points-of-failure"></a>Microsoft online services 工程師如何彈性服務以避免單點失敗？

Microsoft 設計並組建雲端服務，以最大限度地提升可靠性，並將對客戶面臨的負面影響降至最低，以應對一般作業的錯誤和挑戰。 此策略的開始是連接地理位置分散的資料中心網路的網路設計。 Microsoft 的網路架構包括直接互連和多個網路路徑。 Microsoft online services 使用此冗余，自動路由傳送失敗的流量，以提升服務品質。

在任何情況下，Microsoft 線上服務都會以自動化服務狀況監視方式部署在主動/主動設定中，允許服務偵測和復原許多常見的錯誤和失敗，而不需要人工干預。 除了主動/主動設定之外，Microsoft 線上服務會確保服務部署在不同的容錯區域中，以避免一個區域中的錯誤影響其他區域的可用性，以提升容錯能力。

資料恢復功能會保護 Microsoft online services 中的資料完整性與可用性，以補充服務彈性。 我們的服務使用本機儲存裝置冗余和地域冗余，將客戶資料的複本複寫到不同的容錯區域。 如果資料在一個錯誤區域中損毀或遺失，您可以在另一個錯誤區域中存取這些資料，而不會失去可用性。 自動完整性檢查會自動還原由許多實體或邏輯損毀所影響的資料。 Microsoft 也會為客戶提供工具，以在 Exchange Online 和 SharePoint 線上等服務中，將客戶意外刪除或修改的資料復原。

## <a name="how-do-microsoft-online-services-track-dependencies-and-prevent-unauthorized-external-system-connections"></a>Microsoft online services 如何追蹤相依性，以及如何防止未經授權的外部系統連線？

Microsoft online services 小組會識別重要的系統元件及其相依性，以作為商務持續性管理的一部分。 此外，Microsoft 檔和追蹤所有外部系統連線，以確保網路防火牆設定只允許授權的連線。 Microsoft online services 系統、相依性及外部連線會記錄在 Microsoft online services 的資訊安全性架構中。 資訊安全架構和對應的資料流程圖都會至少每年進行檢查及更新，而且每當對系統進行重大變更時，也會進行更新。

Microsoft online services 架構會定期進行驗證，並自動使用雲端架構工具來驗證與安全性原則的搭配，並持續測試隔離和恢復功能。 架構驗證可讓您自動識別目前服務的目前狀態已正軌至所需狀態的實例，並會標記出任何偏差以進行審閱與緩解。 架構驗證的目標是確保服務基礎結構的安全性功能仍可如預期的方式運作。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與架構相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 6：資訊安全性的組織 <br> 13.1：網路安全性管理 <br> 17.2：冗余 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 6：資訊安全性的組織 <br> 13.1：網路安全性管理 <br> 17.2：冗余 | 2020 年 12 月 2 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | BC-1：商務持續性計畫 <br> BC-3： BCDR 程式 <br> BC-4： BCDR 測試 <br> BC-5：業務連續性風險評估 <br> BC-6：協力廠商商務持續性 <br> BC-7：資料中心商務持續性程式 <br> BC-8：資料中心商務持續性測試 <br> BC-9：資料中心恢復性評估 <br>  DS-6：重要元件的冗余 <br> DS-7：客戶資料的複寫 <br> DS-14：客戶服務的還原 <br> DS-16：客戶資料隔離 | 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | AC-4：資訊流執行 <br> CP-9：資訊系統備份 <br> PL-8：資訊安全架構 <br> SC-7：界限保護 <br> SC-22：架構與布建 | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 6：資訊安全性的組織 <br> 13.1：網路安全性管理 <br> 17.2：冗余 | 2021 年 4 月 20 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-37：租使用者隔離 <br> CA-49：備份原則 <br> CA-51：資料複寫 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-05：資料流程圖 <br> CA-37：租使用者隔離 <br> CA-49：備份原則 <br> CA-51：資料複寫 | 2020月24日 |