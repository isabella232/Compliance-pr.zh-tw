---
title: 互聯網安全中心 (CIS) 基準
description: 互聯網安全中心 (CIS) 已公佈一系列適用於 Microsoft 產品和服務的基準
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
ms.openlocfilehash: 18da1f6b422327f42dc517fa0f9c8abe9c91e253
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947654"
---
# <a name="center-for-internet-security-cis-benchmarks"></a>網際網路安全性 (CIS) 中心基準

## <a name="about-cis-benchmarks"></a>關於 CIS 基準

[網際網路安全性中心](https://www.cisecurity.org/)是非營利實體，它的任務是「識別、開發、驗證、升級及維持網路防禦的最佳做法解決方案」。 它從世界各地的政府、企業和學術界，描繪網路安全性和 IT 專業人員的專業知識。 為了開發標準和最佳做法 (包括 CIS 基準、控制項和強化映像)，他們遵循共識決策模型。  
  
[CIS 基準](https://www.cisecurity.org/cis-benchmarks/)是安全地設定系統的配置基準和最佳做法。 每個指導方針建議都參照一或多個 [CIS 控制](https://www.cisecurity.org/controls/)，其開發旨在協助組織改善其網路防禦功能。 CIS 控制對應至許多已建立的標準和法規架構，包括 NIST 網路安全性架構 (CSF) 和 NIST SP 800-53、ISO 27000 系列標準、PCI DSS、HIPAA 等等。  
  
每項基準都經歷了兩個階段的共識檢閱。 第一次是在專家召集討論、建立及測試工作草稿的初始開發期間發生，直到他們達成基準的共識。 在基準發佈之後的第二個階段中，共識小組會檢閱來自網際網路社群的意見反應，以納入基準。  
  
CIS 基準提供兩種等級的安全性設定：

- **第 1 級** 建議可在任何系統上設定的必要基本安全性需求，並且對服務中斷或功能下降應該只有一點影響或者沒有影響。
- **第 2 級** 建議環境的安全性設定需要更大的安全性，可能會造成一些功能下降。

[CIS 強化映像](https://www.cisecurity.org/blog/cis-hardened-images-now-in-microsoft-azure-marketplace/)是根據 CIS 基準強化映像，安全地將虛擬機器映像設定為第 1 級或第 2 級 CIS 基準設定檔。 強化是一種程序，藉由限制讓系統容易受到網路攻擊的潛在弱點，協助保護免於未經授權的存取、拒絕服務及其他網路威脅。

## <a name="microsoft-and-the-cis-benchmarks"></a>Microsoft 和 CIS 基準

互聯網安全中心 (CIS) 已發佈適用於 Microsoft 產品和服務的基準，包括 Microsoft Azure 和 Microsoft 365 基礎基準、Windows 10 基準及 Windows Server 2016 基準。 [CIS Microsoft Azure 基礎基準](https://www.cisecurity.org/benchmark/azure/)適用於規劃開發、部署、評估或保護整合 Azure 之解決方案的客戶。 本文件提供針對 Azure 建立安全基礎組態的規範指導方針。
  
CIS 基準是國際認可的安全性標準，防禦 IT 系統和資料免於網路攻擊。 由數千個企業使用，他們提供建立安全基準組態的規範指導方針。 系統和應用程式系統管理員、安全性專家和其他使用 Microsoft 產品和服務開發解決方案的使用者，都可以使用這些最佳做法來評估和改善應用程式的安全性。  
  
就像所有的 CIS 基準，Microsoft 基準是使用共識檢閱程序所建立，這個程序是根據來自各種學科、具有多元背景 (橫跨軟體開發、稽核和合規性、安全性研究、作業、政府及法律) 專家的意見。 Microsoft 是這些 CIS 努力的整合合作夥伴。 例如，Office 365 根據列出的服務進行測試，而產生的 Microsoft 365 基礎基準涵蓋大範圍的建議，讓您設定適當的安全性原則，這些原則涵蓋帳戶與驗證、資料管理、應用程式權限、儲存空間及其他安全性策略領域。  
  
除了 Microsoft 產品和服務的基準，CIS 會[在 Azure 上發佈 CIS 的強化映像](https://www.cisecurity.org/cis-hardened-images/microsoft/)，設定為符合 CIS 基準，並可從 Microsoft Azure Marketplace 取得。 這些映像包括 Windows Server 2016 和 Windows Server 2019 以及許多 Linux 版本的 CIS 強化映像。 所有在 Azure Marketplace 中提供的 CIS 強化映像都經過認證，可在 Microsoft Azure 上執行。 如 [CIS 指出](https://www.cisecurity.org/blog/cis-hardened-images-now-in-microsoft-azure-marketplace/)，「它們已經針對整備以及與 Microsoft Azure 公用雲端、服務提供者透過雲端作業系統網路主控的 Microsoft Cloud 平台，以及由客戶管理的內部部署私人雲端 Windows Server Hyper-V 部署的相容性，經過預先測試」。

[CIS 強化映像](https://www.cisecurity.org/cis-hardened-images/)是根據 CIS 基準強化映像，安全地將虛擬機器映像設定為第 1 級或第 2 級 CIS 基準設定檔。 強化是一種程序，藉由限制讓系統容易受到網路攻擊的潛在弱點，協助保護免於未經授權的存取、拒絕服務及其他網路威脅。 您可以在 Azure 和 Azure Government 上使用 CIS 強化映像。

如需其他客戶協助，Microsoft 提供 [Azure 藍圖](https://azure.microsoft.com/services/blueprints/)，這是一項服務，可協助您使用可組合的成品(例如 Azure Resource Manager 範本)，以可重複的方式部署和更新雲端環境，以佈建資源、角色型存取控制及原則。 透過 Azure 藍圖佈建的資源遵循組織的標準、模式及規範需求。 Azure 藍圖的首要目標是協助在雲端環境中實現合規性和網絡安全性風險管理的自動化。 為了協助您針對必須實作 CIS Azure 基礎基準的任何 Azure 架構，部署一組核心原則，Microsoft 已發佈[適用於 CIS Microsoft Azure 基礎基準的 Azure 藍圖](/azure/governance/blueprints/samples/cis-azure-1-3-0)。 指派給架構時，Azure 原則會評估資源，以符合指派的原則定義。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- [Azure 和 Azure Government](https://aka.ms/AzureCompliance)
- [Office 和 Microsoft 365](https://aka.ms/o365-compliance-framework)
- SQL Server
- Windows 10
- Windows Server 2016

## <a name="audits-reports-and-certificates"></a>稽核、報告和認證

取得適用於 Microsoft 產品和服務的 [CIS 基準完整清單](https://www.cisecurity.org/cis-benchmarks/)。

- [CIS Azure 基礎基準](https://www.cisecurity.org/benchmark/azure/)
- [CIS Microsoft 365 基礎基準](https://www.cisecurity.org/benchmark/microsoft_office/)
- [Windows 10 基準](https://www.cisecurity.org/benchmark/microsoft_windows_desktop/)
- [Windows Server 2016 基準](https://www.cisecurity.org/benchmark/microsoft_windows_server/)

## <a name="how-to-implement"></a>實作方法

- [適用於 Azure 的 CIS 基準](https://azure.microsoft.com/mediahandler/files/resourcefiles/cis-microsoft-azure-foundations-security-benchmark/CIS_Microsoft_Azure_Foundations_Benchmark_v1.0.0.pdf)：取得針對 Azure 建立安全基礎組態的規範指導方針。  
- [Microsoft 365 安全性藍圖](/microsoft-365/security/office-365-security/security-roadmap)：按照此藍圖，將資料外洩或遭入侵帳戶的可能性降至最低。
- [Windows 安全性基準](/windows/security/threat-protection/windows-security-baselines)：按照這些指導方針，以有效地使用貴組織中的安全性基準。
- [CIS 控制雲端小幫手指南](https://www.cisecurity.org/white-papers/cis-controls-cloud-companion-guide/)：取得將 CIS 控制第 7 版中的安全性最佳做法套用至雲端環境的指導方針。

## <a name="frequently-asked-questions"></a>常見問題集

**遵循 CIS 基準設定是否可以確保我的應用程式的安全性？**

CIS 基準會為採用範圍內 Microsoft 產品和服務的任何人，建立基本的安全性層級。 不過，我們不應將他們視為所有可能安全性組態和架構的詳盡清單，而是作為起點。 每個組織仍然必須評估其特定狀況、工作負載和合規性需求，並相應地訂製其環境。

**CIS 基準更新頻率為何？**

修訂的 CIS 基準版本會依據開發它的 IT 專業人員社群，以及基準支援的技術發行排程，而有所變更。 CIS 會每月發佈報告，宣佈新基準和現有基準的更新。 若要接收這些內容，請在您的設定檔中註冊 [CIS Workbench](https://workbench.cisecurity.org/) (免費)，並且勾選 [接收] 電子報。

**誰參與開發 Microsoft CIS 基準？**

CIS 指出其「準則是透過主題專家、技術廠商、公用和私人 CIS 基準社群成員，以及 CIS 基準開發小組的慷慨自願付出而進行開發」。 例如，您可以在 [CIS Microsoft Azure 基礎基準 v1.0.0 現在可供使用](https://www.cisecurity.org/blog/cis-microsoft-azure-foundations-benchmark-v1-0-0-now-available/)上，找到 Azure 參與者的清單。

## <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a>使用 Microsoft 合規性管理員來評估風險

[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。 合規性管理員會提供特優範本以為此法規建立評定。 可在合規性管理員的 [評定範本] 頁面尋找範本。 瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。

## <a name="resources"></a>資源

- [Azure 合規性文件](/azure/compliance/)
- [Azure 可實現合規性世界](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Microsoft 365 合規性方案](/compliance/regulatory/offering-home)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
- [CIS Microsoft Azure 基礎基準](https://www.cisecurity.org/benchmark/azure/)會為保護 Azure 提供逐步檢查清單。
- [Microsoft Azure 上的 CIS 強化映像](https://www.cisecurity.org/cis-hardened-images/microsoft/)已驗證 Azure 並預先設定為 CIS 基準的安全性建議。  它們皆可在 Azure 和 Azure Government 上提供。
- [適用於 CIS Microsoft Azure 基礎基準的 Azure 藍圖](/azure/governance/blueprints/samples/cis-azure-1-3-0)可協助客戶針對必須實作 CIS Azure 基礎基準的任何 Azure 架構，部署一組核心原則。
- [Azure 原則建議對應](/azure/governance/policy/samples/cis-azure-1-3-0)提供上述藍圖內所含原則定義的詳細資料，以及這些原則定義如何對應至 CIS 中的合規性網域和控制項 Microsoft Azure 基礎基準。 指派給架構時，Azure 原則會以 Azure 原則評估資源，以用於與指派的原則定義不相容。
- [CIS 控制雲端小幫手指南](https://www.cisecurity.org/white-papers/cis-controls-cloud-companion-guide/)提供將 CIS 控制第 7 版中的安全性最佳做法套用至雲端環境的指導方針。
- [CIS Microsoft 365 基礎基準](https://www.cisecurity.org/benchmark/microsoft_office/)會提供為 Microsoft 365 建立安全基準組態的規範性指導方針。
- [Windows 10 安全性原則設定](/windows/security/threat-protection/security-policy-settings/security-policy-settings)
- [Windows 10 企業版安全性](/windows/security/index)
