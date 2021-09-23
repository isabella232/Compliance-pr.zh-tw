---
title: Microsoft 拒絕服務防禦策略
description: 在本文中，您可以找到針對拒絕服務 (DoS) 攻擊的 Microsoft 防護策略的概述。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: e1613765d3ffb7b43b80d07823fe8aef45719b70
ms.sourcegitcommit: cb0b058800d3a8f04921066b4c59fb427eb9c268
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2021
ms.locfileid: "59486190"
---
# <a name="microsoft-denial-of-service-defense-strategy"></a>Microsoft 拒絕服務防禦策略

## <a name="denial-of-service-defense-strategy"></a>阻絕服務攻擊策略

Microsoft 對於防禦網路型分散式阻斷服務) DDoS (的策略是唯一的，因為這是一種全球的廣泛佔用，所以可讓 Microsoft 利用大多數其他組織無法使用的策略及技術。 此外，Microsoft 還會針對廣泛的威脅情報網絡（包括 Microsoft 合作夥伴和更廣泛的 internet 安全性社區）所匯總的集合知識進行貢獻和繪製。 這種情報，以及從線上服務和 Microsoft 全域客戶群收集的資訊，可持續改善 Microsoft 的 DDoS 防護系統，以保護所有的 Microsoft 線上服務資產。

Microsoft 的 DDoS 策略的基石是全域目前狀態。 Microsoft 與網際網路提供者、對等提供者 (公開和私營) ，以及世界各地的私營公司。 這項服務可提供 Microsoft 的大量網際網路服務，讓 Microsoft 能夠吸收跨越大型 surface 區域的攻擊

隨著 Microsoft 的 edge 容量隨著時間成長，對個別 edge 的攻擊意義會大幅降低。 由於這一降低，Microsoft 已將其 DDoS 防護系統的偵測和緩解元件隔開。 Microsoft 會在地區性資料中心部署多層偵測系統，以偵測其飽和點較接近的攻擊，同時維持 edge 節點的全域緩解。 此策略可確保 Microsoft 服務可以處理多個同時進行的攻擊。

Microsoft 對 DDoS 攻擊所採用的最有效且低成本的防禦措施之一，是減少服務攻擊面。 不需要的流量會在網路 edge 中斷，而不會分析、處理及清理資料內聯。

在使用公用網路的介面上，Microsoft 會針對防火牆、網路位址轉譯和 IP 篩選功能使用特殊用途的安全性裝置。 Microsoft 也會使用全域同等成本的多重路徑 (ECMP) 路由。 全域 ECMP 路由是一個網路架構，可確保有多個通用路徑可以到達服務。 針對每個服務使用多個路徑時，DDoS 攻擊會限制于發起攻擊的地區。 其他地區應受到攻擊的影響，因為使用者可能會使用其他路徑來到達這些地區的服務。 Microsoft 也已開發內部 DDoS 相互關聯和偵測系統，使用流程資料、效能測量及其他資訊，以快速偵測 DDoS 攻擊。

為了進一步保護雲端服務，Microsoft 使用 Azure DDoS 保護，這是一種內置於 Microsoft Azure 連續監控和滲透測試程式中的 DDoS 防護系統。 Azure DDoS 保護不僅設計用於抵禦外部攻擊，還設計來自其他 Azure 承租人的攻擊。 Azure 使用標準偵測和緩解技術，例如 SYN cookie、速率限制和連線限制，以防範 DDoS 攻擊。 若要支援自動防護，跨工作負載 DDoS 事件回應小組會識別各小組的角色與責任、升級的準則，以及跨受影響團隊之事件處理的通訊協定。

對目標所發動的大部分 DDoS 攻擊是在網路 (L3) 和傳輸 (L4) OSI (OSI [) 的層](/windows-hardware/drivers/network/windows-network-architecture-and-the-osi-model) 級。 位於 L3 和 L4 層的攻擊是專門用來淹沒網路介面或服務，其攻擊流量會淹沒資源，並拒絕回應合法流量的能力。 為了防範 L3 和 L4 攻擊，Microsoft 的 DDoS 解決方案會使用資料中心路由器的流量採樣資料，以保護基礎結構及客戶目標。 流量採樣資料會由網路監控服務進行分析，以偵測攻擊。 偵測到攻擊時，自動防護機制會發起緩解攻擊，並確保客戶面臨的攻擊流量不會造成宣傳者損毀或降低其他客戶服務的網路服務品質。

Microsoft 也採用攻擊性的方法來 DDoS 防衛。 Botnets 是一種常見的命令和控制來源，用來執行 DDoS 攻擊 amplify 攻擊及維護匿名。 Microsoft 數位犯罪單位 (DCU) 著重于識別、調查及中斷惡意程式碼發佈和通訊基礎結構，以降低 botnets 的規模和影響。

## <a name="application-level-defenses"></a>應用層級防護

Microsoft 工程小組遵循 [Microsoft Operational Security 保障](https://www.microsoft.com/SDL/OperationalSecurityAssurance) 所設定的嚴格標準，協助保護客戶資料。 Microsoft 的雲端服務是專為支援高負載而建立，可協助您防範應用層級的 DDoS 攻擊。 Microsoft 的向外延展架構跨多部全球資料中心分配服務，其相關工作負載具有區域隔離和工作負載特有的節流功能。

客戶在初始設定服務期間所識別的每一個客戶國家或地區，會決定該客戶資料的主要儲存位置。 根據主要/備份策略，在重複資料中心之間複製客戶資料。 主要資料中心會裝載應用程式軟體，以及軟體中所執行的所有主要客戶資料。 備份資料中心提供自動容錯移轉。 如果主要資料中心因任何原因而停止運作，則要求會重新導向到備份資料中心內的軟體和客戶資料的複本。 在任何指定的時間，都可能會在主要或備份資料中心處理客戶資料。 跨多個資料中心散佈資料，可在一部資料中心遭到攻擊時減少受影響的面範圍。 此外，受影響的資料中心內的服務可快速重新導向至次要資料中心，以便在攻擊期間維持可用性，並在緩解攻擊之後重新導向主要資料中心。

隨著 DDoS 攻擊的另一項減輕，個別的工作負載包括管理資源使用狀況的內建功能。 例如，Exchange Online 和 SharePoint Online 中的節流機制，都是多種階層式方法，以防禦 DDoS 攻擊。

Azure SQL Database 會以閘道服務（稱為 DoSGuard 的閘道服務）形式進行額外的安全性層級，以根據 IP 位址追蹤失敗的登入嘗試。 若到達來自相同 IP 的失敗登入嘗試閾值，DoSGuard 會封鎖預先確定的時間長度。

## <a name="resources"></a>資源

- [Azure DDoS 保護標準概述](/azure/ddos-protection/ddos-protection-overview)
- [Azure DDoS 保護標準基本最佳作法](/azure/ddos-protection/fundamental-best-practices)
- [DDoS 回應策略的元件](/azure/ddos-protection/ddos-response-strategy)
