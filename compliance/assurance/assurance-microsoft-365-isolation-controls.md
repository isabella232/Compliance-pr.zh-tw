---
title: Microsoft 365 隔離控制項
description: 深入瞭解 Microsoft 365 中的隔離控制項
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
ms.openlocfilehash: 0139d8182cf9e662e9985faf4a7fd6025fea363a
ms.sourcegitcommit: 61357661caf64eeb9143046b4dd66c83e1439ee3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58470806"
---
# <a name="microsoft-365-isolation-controls"></a>Microsoft 365 隔離控制項

Microsoft 持續運作，以確保多承租人架構的 Microsoft 365 支援企業級的安全性、機密性、隱私權、完整性、本機、國際和可用性[標準](https://www.microsoft.com/trust-center/compliance/compliance-overview)。 由 Microsoft 提供的服務規模和範圍，使用大量的人工互動來管理 Microsoft 365，使其非常困難且非經濟。 Microsoft 365 服務是透過全域分散式資料中心提供，每個都具有極高的自動化，需要人工觸控或任何對客戶內容的存取。 我們的員工使用自動工具和高安全性的遠端存取，支援這些服務和資料中心。

Microsoft 365 是由多種服務所組成，可提供重要的商務功能，並對整個 Microsoft 365 經驗產生貢獻。 每個服務都是自包含的，且設計為彼此整合。 Microsoft 365 是以下列原則為設計：

- 以服務為導向的架構：以互通性服務的形式設計和開發軟體，以提供完善定義的商務功能。
- [運作安全性保證](https://www.microsoft.com/securityengineering/osa)：一種架構，包含透過 microsoft 獨有的各種功能所取得的知識，包括 Microsoft [安全性開發週期](https://www.microsoft.com/sdl/default.aspx)、 [microsoft 安全回應中心](https://www.microsoft.com/msrc)，以及 cybersecurity 威脅形勢的深入認知。

Microsoft 365 服務間相互運作，但會加以設計及實施，這樣就能將它們部署並運作為自治服務，彼此獨立。 Microsoft segregates Microsoft 365 的責任和責任範圍，以降低未經授權或無意修改或誤用組織資產的機會。 Microsoft 365 小組已經定義角色，成為綜合角色存取控制機制的一部分。

## <a name="tenant-isolation"></a>租用戶隔離

雲端計算的其中一個主要優點是，許多客戶都有共同共同使用的共同基礎結構，進而可實現規模經濟效益。 Microsoft 持續努力，以確保雲端服務的多租使用者架構支援企業級安全性、機密性、隱私權、完整性和可用性標準。

Microsoft 雲端服務的設計是假設所有租使用者可能會惡意處理所有其他租使用者，並已實施安全性措施，以防止一個承租人的動作影響另一個租使用者的安全性或服務，或存取另一個租使用者的內容。

在多租使用者環境中維護租使用者隔離的兩個主要目標如下：

- 防止對承租人的客戶內容洩露或未經授權存取和
- 防止一個承租人的動作對其他租使用者的服務造成不良影響

在整個 Microsoft 365 中已實施多種保護形式，以防止客戶損妥 Microsoft 365 服務或應用程式或未經授權存取其他承租人或 Microsoft 365 系統本身的資訊，包括：

- 在每個承租人中 Microsoft 365 服務的邏輯隔離，都是透過 Azure Active Directory 授權和以角色為基礎的存取控制來達成。
- SharePoint線上提供儲存層級的資料隔離機制。
- Microsoft 使用嚴謹的實體安全性、背景篩選和多層次的加密策略，以保護客戶內容的機密性和完整性。 所有的 Microsoft 365 資料中心都具有生物統計學存取控制，大多數需要使用 palm 列印才能獲得實體存取權。 此外，所有以美國為基礎的 Microsoft 員工都必須在聘用過程中成功完成標準背景檢查。 如需 Microsoft 365 中用於管理存取之控制項的詳細資訊，請參閱[Microsoft 365 帳戶管理](assurance-microsoft-365-account-management.md)。
- Microsoft 365 使用的服務端技術會在靜止和傳輸中加密客戶內容，包括 BitLocker、每個檔案加密、傳輸層安全性 (TLS) 和網際網路通訊協定安全性 (IPsec) 。 如需 Microsoft 365 中加密的特定詳細資料，請參閱[Microsoft 365 中的資料加密技術](/microsoft-365/compliance/office-365-encryption-in-the-microsoft-cloud-overview)。

以上所列的保護功能提供了可靠的邏輯隔離控制，可提供與獨立實體隔離所提供之威脅防護和緩解同等的威脅。

## <a name="resources"></a>資源

- [Azure Active Directory 中的隔離與存取控制](/microsoft-365/enterprise/microsoft-365-isolation-in-azure-active-directory)
- [監視和測試租使用者界限](assurance-monitoring-and-testing.md)
- [Microsoft 365 中的隔離與存取控制](/microsoft-365/enterprise/microsoft-365-isolation-in-microsoft-365)
