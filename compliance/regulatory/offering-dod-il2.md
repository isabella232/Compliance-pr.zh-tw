---
title: '國防部門 (DoD) 影響等級 2 (IL2) '
description: 深入瞭解 Microsoft 如何滿足國防部門的 (DoD) 影響等級 2 (IL2) 標準。
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
ms.openlocfilehash: c57183a53c563fffa2bb3eb1cedb2fca23db26f4
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947663"
---
# <a name="department-of-defense-dod-impact-level-2-il2"></a>國防部門 (DoD) 影響等級 2 (IL2) 

## <a name="dod-il2-overview"></a>DoD IL2 概述

國防 Information Systems 機關 (DISA) 是美國國防部 (DoD) 的代理人，負責開發及維護 DoD 雲端電腦 [安全性需求指南 (SRG) ](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)。 SRG 會定義 DoD 用以評估雲端服務提供者 (CSP) 的安全性狀態的基準安全性需求，以支援 DoD 臨時授權 (PA) ，允許 CSP 主控 DoD 使命。 它包含、取代和 rescinds 先前發佈的 DoD 雲端安全性模型 (CSM) 和對應至 DoD 風險管理架構 (RMF) 。

DISA 指南 DoD 以規劃及授權使用 CSP 的機構和部門。 它也會評估與 SRG 相容性相關的 CSP 服務，這是一種授權程式，其中 Csp 可以提供檔，以概括顯示其與 DoD 標準的相容性。 在適當的情況下，它會 (PAs) DoD 臨時授權，因此 DoD 的代理商和支援組織可以使用雲端服務，而不必自行進行完整核准程式，節省時間和精力。

[15 月 2014 DoD 的 CIO 備忘錄](https://www.esi.mil/contentview.aspx?id=585)，針對 *購買和使用商業性雲端計算服務的更新指導* 方針，其「FedRAMP 將充當所有 DoD 雲端服務的最低安全性基準。 SRG 會在所有資訊影響層級 (IL) 使用 FedRAMP 適中的基準，並考慮使用高基準。

[SRG Section 5.1.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5SECURITYREQUIREMENTS) *DoD 使用 FedRAMP 安全性控制* ，表明 IL2 資訊可能會主控于一個 CSP 中，該 CSP 最少保留 FedRAMP 適中的 Pa 及 DoD 層級2的 pa，遵循 Section 5.6.2 中所述的人員安全性需求。 不過，此方法不會將 CSP 從其他安全性和整合需求，當作使命擁有者的要求來緩解。 根據 [SRG 區段 5.2.2.1](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html#5.2LegalConsiderations) *IL2 位置和分割性需求*，FedRAMP 適中的 pa 會充分涵蓋 DoD IL2 pa，這樣就不會進一步評估 IL2 PA 的需求。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- Dynamics 365
- Microsoft Cloud App Security
- 適用於端點的 Microsoft Defender
- Microsoft Graph
- Microsoft Intune
- Microsoft Stream
- Office 365美國政府，Office 365 美國政府-高
- Power Apps
- 電源自動化
- Power BI

## <a name="azure-dynamics-365-and-dod-il2"></a>Azure、Dynamics 365 及 DoD IL2

如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [Azure DOD IL2](/azure/compliance/offerings/offering-dod-il2)service。

## <a name="office-365-and-dod-il2"></a>Office 365 和 DoD IL2

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **GCC** | 活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告，商務用 OneDrive，人員卡片，SharePoint 線上，商務用 Skype，Windows Ink |
| **GCC High** | 活動摘要服務，Bing 服務，Delve，Exchange Online Protection，Exchange Online，智慧服務，Microsoft Teams，Office 365 客戶入口網站，Office 線上，Office 服務基礎結構，Office 使用狀況報告，商務用 OneDrive，人員卡片，SharePoint 線上，商務用 Skype，Windows Ink |

### <a name="resources"></a>資源

- [Microsoft 政府解決方案](https://www.microsoft.com/enterprise/government)
- [DoD 雲端電腦安全性性需求手冊](https://dl.dod.cyber.mil/wp-content/uploads/cloud/SRG/index.html)
- [FedRAMP 檔](https://www.fedramp.gov/documents/)
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) *風險管理架構：資訊系統和組織：系統安全性和隱私權的系統 Life-Cycle 方式*
- [NIST SP 800-53](https://csrc.nist.gov/Projects/risk-management/sp800-53-controls/release-search#!/800-53) *的安全性和隱私權控制資訊系統和組織*
- [DoD 指令 8510.01](https://www.esd.whs.mil/Portals/54/Documents/DD/issuances/dodi/851001p.pdf) *DoD 風險管理架構 (RMF) DoD 資訊技術* (
