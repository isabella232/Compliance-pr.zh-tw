---
title: 法國健康資料代管 (HDS)
description: Microsoft 雲端服務經過認證，符合健康資料代管 (Hébergeurs de Données de Santé) 標準。
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
ms.openlocfilehash: f8c99a93cac767439d157a7d709c7ed1d706c113
ms.sourcegitcommit: 16cec8f7ca799a415bfbae937b177a628a0f2987
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/24/2021
ms.locfileid: "58505936"
---
# <a name="health-data-hosting-hds-france"></a>法國健康資料代管 (HDS)

## <a name="about-hds"></a>關於 HDS

Hébergeurs de Données de Santé (HDS) 認證要求雲端服務提供者等實體，代管受法國法律管轄的個人健康資料並收集這些資料用於提供預防、診斷和其他健康服務。 HDS 法規由 [ASIP SANTÉ](https://esante.gouv.fr/) 頒布，該機構隸屬於法國衛生部，負責在法國推廣電子醫療保健解決方案。

根據法國公共衛生法 (第 L.1111-8 條) 規定，代管健康資料需受法國法律監管，其規定任何醫療保健組織 (醫院、製藥廠、實驗室) 處理個人醫療資料時，必須使用經 HDS 認證的服務提供者。 在 2018 年 4 月，公共衛生法新條款第 R1111-8-8 條至第 R1111-11 條生效，將認證程序從法國衛生部授權改為由 BSI 等授權機構認證。

HDS 認證要求服務提供者實作措施，確保病患的個人健康資料受到保護、保持機密性且易於存取。 這些措施包括增強式驗證和授權程序、強固的備份系統和功能強大的加密方法。 HDS 還指定必須包含在與雲端服務提供者簽訂之合約中的強制性條款。 無論資料儲存在何處，這些需求皆適用。

## <a name="microsoft-and-hds"></a>Microsoft 和 HDS

Microsoft Azure、Microsoft Dynamics 365 和 Microsoft Office 365 已獲健康資料代管 (Hébergeurs de Données de Santé，HDS) 認證，代管受法國法律管轄的個人健康資料的所有實體都需要有此認證。 這使 Microsoft 在儲存和處理健康資料方面成為第一個符合嚴格的法國標準的主要雲端服務提供者。 根據 2018 年法國公共衛生法修訂版的要求，此認證對代管服務和雲端提供者提出了進階安全性和隱私權要求，以確保敏感性資料的機密性和完整性受到充分保護。

Microsoft 符合 HDS 要求已通過 [BSI Group](https://www.bsigroup.com/fr-FR/) (由法國當局認可進行 HDS 審核的獨立認證機構) 的審核和認證。

HDS 認證讓法國的醫療保健提供者使用 Microsoft 雲端服務，透過提升臨床和操作效率來節省成本，並為開發最先進的創新醫療保健解決方案開啟了一扇大門。 提供者能夠開發智慧型應用程式或使用托管於 Azure 的第三方應用程式來實作預測性分析，以個人化醫療保健、遠距評估和治療病患 (遠距醫療)，以及加強治療性藥物監控。

嚴格的審核涵蓋了 Microsoft 為保護個人健康資料的安全和保護其機密性而採取的措施，包括：

- Microsoft 雲端服務的 [ISO/IEC 27001:2013 資訊安全性管理](offering-iso-27001.md)認證 (每年審核是否符合合規性)。
- 基於符合 GDPR 合規性的高層級隱私權和 [ISO/IEC 27018 實務規範以保護雲端中的個人資料](offering-iso-27018.md)。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- [Azure](https://aka.ms/AzureCompliance)。 HDS 認證適用於所列 Azure 合規性方案中符合 ISO/IEC 27001 標準以及在下列區域中佈建的 Azure 服務：
    - 法國中部 (巴黎)
    - 法國南部 (馬賽)
    - 北歐 (愛爾蘭)
    - 西歐 (荷蘭)
- Dynamics 365。 HDS 認證適用於從法國和歐盟地區佈建的 Dynamics 365 [Core Online Services](https://aka.ms/Online-Services-Terms)。
- Intune
- Microsoft 365。 HDS 認證適用於從法國和歐盟地區佈建的 Office 365 [Core Online Services](https://aka.ms/Online-Services-Terms)。
- Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中

HDS 認證不適用於 Microsoft 線上服務預覽版或發行前版本。

## <a name="audits-reports-and-certificates"></a>稽核、報告和憑證

[HDS 認證](https://esante.gouv.fr/labels-certifications/hebergement-des-donnees-de-sante)會對主控服務和雲端提供者的進階安全性和隱私權需求，以確保敏感性資料的機密性和完整性受到適當的保護。 Microsoft 雲端服務 (包含 Azure) 已授與 HDS 認證，如 [HDS 驗證主機](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-certifies)的 ASIP Santé 清單所示。

## <a name="how-to-implement"></a>實作方法

- **合約條款**：法國公共衛生法要求健康資料代管服務或雲端服務提供者與其客戶之間執行特定的合約條款。 符合資格的客戶必須與他們的 Microsoft 授權連絡窗口連絡，才能在 Microsoft 線上服務上代管健康個人資料之前，先簽訂這些特定的合約條款。
- **健康和生命科學**：協助建立 Azure 解決方案的案例概觀、解決方案指南、教學課程和其他資源。

## <a name="resources"></a>資源

- [Azure 合規性文件](/azure/compliance/)
- [Microsoft Online Services 條款](https://aka.ms/Online-Services-Terms)
- [Microsoft HDS 認證部落格](https://news.microsoft.com/2018/11/06/microsoft-1er-acteur-majeur-du-cloud-public-a-etre-certifie-hebergeur-de-donnees-de-sante-en-france/)
- [Azure 法國](https://azure.microsoft.com/global-infrastructure/france/)
- [Azure 醫療](https://azure.microsoft.com/industries/healthcare/)
- [Microsoft 的安全性](https://www.microsoft.com/security)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
