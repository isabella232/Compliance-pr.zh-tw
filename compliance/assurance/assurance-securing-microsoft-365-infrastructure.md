---
title: 保護 Microsoft 365 基礎結構
description: 深入瞭解 Microsoft 如何保護 Microsoft 365 基礎結構。
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
ms.openlocfilehash: 224900bd60f2fd5637e7264f1aed98d5ff878b20
ms.sourcegitcommit: fb379d1110a9a86c7f9bab8c484dc3f4b3dfd6f0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53089616"
---
# <a name="securing-the-microsoft-365-infrastructure"></a>保護 Microsoft 365 基礎結構

Microsoft 365 是世界上最大的企業和消費型雲端服務之一，而且會在客戶基礎、產品及功能方面，繼續迅速成長。 客戶 Microsoft 365 不僅適用于世界一流的生產力解決方案，還能協助保護其最機密的資訊，避免不斷演變的網路威脅環境。 這是 Microsoft 最重要的頭等大事，可讓客戶資料安全，並維護客戶信任。

保護此規模和複雜性的系統是不可能的，如果安全性是事後的，則只有在初始設計程式內整合安全性時，才會有效。 它需要可靠的威脅偵測系統，並提供來自自動化系統和高素質工程師的提示回應。 連續評估和驗證這些系統是非常重要的，可確保安全設定保持不變，且會識別先前未知的漏洞。

## <a name="core-security-principles"></a>核心安全性原則

七項安全性原則為我們的架構奠定了基礎，以 Microsoft 365 *防禦* 威脅、偵測 *和回應* 任何威脅，以及根據評估的結果不斷 *評估* 安全性狀況及改善服務。

- **資料隱私權**：客戶擁有其資料，而 Microsoft 是保管人。 Microsoft 365 服務，除非客戶明確要求和核准，否則設計為無需使用工程師存取客戶資料。
- **假設** 損等：會以實際的方式處理個人和服務。
- **最低許可權**：對資源的存取權和許可權，只限于執行必要工作所需的工作。
- **違反界限**：一個界限內的身分識別和基礎結構，會與其他界限中的資源隔離。 損迭一個界限不應導致遭到其他威脅。
- **Service fabric 整合安全性**：安全優先級和需求已內置於新功能與功能的設計中，確保強大的安全性狀況可隨每個服務一起縮放。
- **自動化和自動**： Microsoft 著重于開發耐用的產品和架構，可讓您智慧化及自動強制執行服務安全性，同時讓 Microsoft 工程師能夠以規模的方式安全地管理回應安全性威脅。
- **自我調整安全性**： Microsoft 的安全性功能可透過機器教學模型、常式滲透測試及自動化評估加以增強。

## <a name="protection"></a>保護

### <a name="access-control"></a>存取控制

根據預設，負責開發及維護 Microsoft 365 服務的人員，在服務基礎結構中 (ZSA) 具有零的存取權。 Microsoft 致力於只雇用最佳的工程師和嚴格的背景檢查，但 Microsoft 不會假設在運作服務中預設受信任。 此外，當核准人員進行特殊許可權存取時，他們只會獲得有限期限的存取權，只會對特定範圍的服務基礎結構執行必要的動作。 Microsoft 會將這些原則視為即時 (JIT) 和足夠的存取 (JEA) ，該是透過一名為密碼箱的系統來執行。

若要取得更高的許可權，Microsoft 工程師會送出特定任務的要求，並指定執行它的時間範圍。 一旦核准，密碼箱便會產生專用的 JIT 帳戶，只具備執行所要求之工作的能力。 動作通常採取自動化工作流程的形式，以安全地執行所需的任何疑難排解或復原。 在極少數的情況下，必須直接存取基礎結構時，嚴格監控的特殊許可權存取工作站 (PAWs) 是必要的。

惡意使用者和遭破壞的帳戶在任何組織中都有實際的可能性，而且我們的存取控制系統是為了防範這些威脅而設計的。

如需存取控制的詳細資訊，請參閱 [Identity and access management 一覽](assurance-identity-and-access-management.md)。

### <a name="encryption"></a>加密

雖然存取控制在防護 Microsoft 365 服務中提供重要的角色，但整個資料生命週期都使用加密，以進一步保護 Microsoft 客戶的機密性和隱私權。

用戶端電腦、Microsoft 365 伺服器和非 Microsoft 365 伺服器之間傳輸的資料會使用 TLS 1.2 加密。 我們會定期查看使用中的密碼和通訊協定，並在必要時新增已改進的通訊協定，並移除較弱的通訊協定。

Microsoft server 上的客戶內容會在大量使用 BitLocker 的磁片區層級加密。 另外，您也可以使用由 Microsoft 或客戶管理的金鑰來套用應用層級加密。 只有透過 JIT 和 JEA 處理常式授權和核准時，才可以存取 Microsoft 受管理的金鑰。

如需 Microsoft 365 中加密的相關資訊，請參閱[encryption and key management 概述](assurance-encryption.md)。

### <a name="network-isolation"></a>網路隔離

根據最低許可權的原則，Microsoft 365 會限制服務基礎結構不同部分之間的通訊，只會限制運作的必要部分。 根據預設，會拒絕所有網路流量，但只會明確定義所允許的通訊。 這種限制會在整個基礎結構中建立違規界限。 若要將新的網路路徑新增至其服務以容納新功能的 Teams，必須先評估並核准要求，才能開啟此要求。

如需 Microsoft 365 中的網路隔離的詳細資訊，請參閱[Microsoft 365 隔離控制項](/microsoft-365/enterprise/microsoft-365-isolation-controls)。

## <a name="detection--response"></a>偵測 & 回應

### <a name="security-monitoring"></a>安全性監視

Microsoft 大規模的安全性監控只有透過使用自動雲端式解決方案產生高準確性的警示時，才有可能。 從整個核心基礎結構收集的每一個服務和遙測資料中的審計記錄會傳送至專屬的「集中近即時處理及警示」解決方案。

盡可能使用自動觸發的動作修正偵測到的威脅。 當自動方案未成功或無法解決問題時，Microsoft 工程師會立即採取行動來緩解威脅。

如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[安全性監視概述](assurance-security-monitoring.md)。

## <a name="assessment"></a>評估

### <a name="automated-assessments"></a>自動評估

不論系統的設計方式為何，安全性狀況都會因故意和無意間的設定偏差隨著時間而降低。 自動工具會持續評估尋找未修補及配置錯誤之服務的 Microsoft 365 系統。 這種評估通常稱為「修補」、「反病毒」、「弱點」和「設定掃描」 (PAVC) 。

我們也會經常驗證我們的架構，以找出未使用的開啟埠和具有管理存取權的帳戶等實例。 任何從預先定義的所需狀態偏差的服務都會自動重新排列成對齊。

如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[弱點管理概述](assurance-vulnerability-management.md)。

### <a name="attack-simulation-and-penetration-testing"></a>攻擊模擬和滲透測試

Microsoft 365 的最大優先順序是防止攻擊 infiltrating 防禦。 Microsoft 365 擁有一支專門的安全性專家小組，這些專家會持續進行模擬攻擊，識別先前未知的漏洞，並提供大量資料流程，以改善安全性監控功能。 這些模擬型攻擊採用一種頻繁的自動小型攻擊和專家導向的深度 dives。 在這些活動中，Microsoft 會評估偵測、回應及逐出攻擊者的能力。

如需 Microsoft 365 中安全性監視的詳細資訊，請參閱[Microsoft 365 中的攻擊模擬](assurance-monitoring-and-testing.md)。

## <a name="resources"></a>資源

[在幕後：保護 Microsoft 365 服務電源的基礎結構](https://download.microsoft.com/download/c/4/5/c45b197e-f0d9-4f40-bd5f-ed8fc7d0cd8c/M365DCSecurityIntro_Whitepaper.pdf)
