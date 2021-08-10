---
title: '國防部門 (DoD) 影響層級 5 (IL5) '
description: 深入瞭解 Microsoft 如何滿足國防部門 (DoD) 影響等級 5 (IL5) 標準。
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
ms.openlocfilehash: 539a53888ec859bb3b6942b48288659f73fa4b69807ce19e063cbfe104b7072d
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54294230"
---
# <a name="department-of-defense-dod-impact-level-5-il5"></a>國防部門 (DoD) 影響層級 5 (IL5) 

## <a name="dod-il5-overview"></a>DoD IL5 概述

國防 Information Systems 機關 (DISA) 是美國國防部 (DoD) 的代理人，負責開發及維護 DoD 雲端電腦 [安全性需求指南 (SRG) ](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)。 SRG 會定義 DoD 用以評估雲端服務提供者 (CSP) 的安全性狀態的基準安全性需求，以支援 DoD 臨時授權 (PA) ，允許 CSP 主控 DoD 使命。 它包含、取代和 rescinds 先前發佈的 DoD 雲端安全性模型 (CSM) 和對應至 DoD 風險管理架構 (RMF) 。

DISA 指南 DoD 以規劃及授權使用 CSP 的機構和部門。 它也會評估與 SRG 相容性相關的 CSP 服務，這是一種授權程式，其中 Csp 可以提供檔，以概括顯示其與 DoD 標準的相容性。 在適當的情況下，它會 (PAs) DoD 臨時授權，因此 DoD 的代理商和支援組織可以使用雲端服務，而不必自行進行完整核准程式，節省時間和精力。

根據 [SRG Section 3.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#3.2InformationImpactLevels) *資訊影響層級*，IL5 資訊涵蓋：

- 受管理的未分類資訊 (CUI) 需要更高的保護層級，而不是 IL4 所具備的保護
    - [CUI](https://www.archives.gov/cui)登錄會提供由執行的分支所保護的特定資訊類別，例如， [CUI 類別清單](https://www.archives.gov/cui/registry/category-list)中包含超過20個類別群組。
    - [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *保護 Nonfederal 系統和組織中受控的未分類資訊* ，供聯邦代理商用於合約或與非聯邦組織建立的其他合約。

- 本國安全系統 (NSS) 
    - [NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf) ， *識別區域安全性系統的資訊系統* 提供 NSS 的定義。
    - [CNSSI 1253](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *Security 分類和 Control Selection 針對全國的安全性系統，針對* 聯邦機關應套用來分類全國安全性資訊的安全性標準提供指導方針。

[15 月 2014 DoD 的 CIO 備忘錄](https://www.esi.mil/contentview.aspx?id=585)，針對 *購買和使用商業性雲端計算服務的更新指導* 方針，其「FedRAMP 將充當所有 DoD 雲端服務的最低安全性基準。 SRG 會在所有資訊影響層級 (IL) 使用 FedRAMP 適中的基準，並考慮使用高基準。

[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD 使用 FedRAMP 安全性控制* ，說明 FedRAMP 的高 PA （結合 DoD 的 FedRAMP + 控制項和控制項增強功能） (C/CEs) 和 SRG 中的需求，是用來評估 awarding a IL5 的 a DoD PA。 不論使用何種 C/CE 基準做為 FedRAMP 高 PA 的基礎，在 IL5 中取得 DoD PA 之前，必須先評估並核准其他考慮和/或需求。 具體說來， [SRG Section 5.1.2](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD FedRAMP + Security Controls/強化* 狀態在表2中，除了 FedRAMP 的高基線之外，還需要10個其他 C/CES，DoD IL5 PA。

此外，根據 [SRG 區段 5.2.2.3](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL5 位置和分割性需求*，下列需求 (彼此之間的需求) 必須針對第5級的 PA 進行：

- DoD 和聯邦政府承租人/使命之間的虛/邏輯分隔性已足夠。 需要租使用者/使命系統之間的虛擬/邏輯分隔。
- 從非 DoD/非聯邦政府租使用者實際的隔離 (（也就是「公用」、「州政府租使用者) ）。
- CSP 會限制對美國公民的 CSP 員工，對 DoD 和社區資訊的潛在存取權。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- Dynamics 365 客戶服務
- 適用於端點的 Microsoft Defender (之前稱為 Microsoft Defender 進階威脅防護)
- Microsoft Graph
- Microsoft Stream
- Office 365 美國政府國防版
- Power Automate (之前稱為 Microsoft Flow)
- Power BI

## <a name="azure-dynamics-365-and-dod-il5"></a>Azure、Dynamics 365 及 DoD IL5

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [Azure DOD IL5](/azure/compliance/offerings/offering-dod-il5)service。

## <a name="office-365-and-dod-il5"></a>Office 365 和 DoD IL5

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **DoD** | 活動摘要服務，Bing 服務，Exchange Online，Exchange Online Protection，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告、商務用 OneDrive、人員卡片、SharePoint 線上、商務用 Skype Windows Ink |

### <a name="attestation-documents"></a>證明檔

我們的政府客戶可以提交套件存取要求表單，直接從[FedRAMP 的 Marketplace](https://marketplace.fedramp.gov/#!/products?sort=productName&productNameSearch=azure) Office 365 美國政府國防 FedRAMP 檔。 您必須具有 .gov 或 mil 的電子郵件地址，才能直接從 FedRAMP 存取 FedRAMP 的安全性套件。

選取 [FedRAMP 和 DoD 檔，包括系統安全性計畫 (SSP) 、連續監控報告、動作和里程碑的計畫， (POA \& M) （如果有的話），您可以從「服務信任入口網站 [審核報告-FedRAMP 報表](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3) 」區段中的 [保密協定和暫止的存取授權] 中取得客戶。 請與您的 Microsoft 客戶代表聯繫以取得協助。

### <a name="resources"></a>資源

- [Microsoft 政府解決方案](https://www.microsoft.com/enterprise/government)
- [DoD 雲端電腦安全性性需求手冊](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [FedRAMP 檔](https://www.fedramp.gov/documents/)
- [DoD 指令 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD 風險管理架構 (RMF) DoD 資訊技術* (
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *風險管理架構：資訊系統和組織：系統安全性和隱私權的系統 Life-Cycle 方式*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *的安全性和隱私權控制資訊系統和組織*
- *將資訊系統識別為全國安全性系統的* [NIST SP 800-59](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-59.pdf)指導方針
- [](https://www.dcsa.mil/portals/91/documents/ctp/nao/CNSSI_No1253.pdf) *適用于全國安全性系統的 CNSSI 1253 安全性分類和控制選項*
- [NIST SP 800-171](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) *保護 Nonfederal 系統和組織中受控未分類的資訊*
- 受管理的未分類資訊 (CUI) [Registry](https://www.archives.gov/cui) 和 CUI [類別清單](https://www.archives.gov/cui/registry/category-list)。
