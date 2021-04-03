---
title: Microsoft 365 拒絕服務防護策略
description: 在本文中，您可以找到針對拒絕服務 (DoS) 攻擊的 Microsoft 防護策略的概述。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: None
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
ms.openlocfilehash: 5776b3eb6c0b79b5f272d6e24dd8680967ca2eb4
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51496949"
---
# <a name="microsoft-365-denial-of-service-defense-strategy"></a>Microsoft 365 拒絕服務防護策略

## <a name="core-principles-of-defense-against-denial-of-service-attacks"></a>防禦拒絕服務攻擊的核心原則

防禦網路型拒絕服務 (時，有三個核心原則 DoS) 攻擊：全部、偵測和緩解。 在偵測之前會發生吸收，必須先進行偵測，然後才能開始緩解。 如果甚至無法吸收小型的 DoS 攻擊，則服務的時間不足以偵測到攻擊。 在系統大量淹沒之前偵測攻擊，defenders 可實施回應計畫。

下列公式可協助接近 DoS 攻擊的影響時間：

  **(大小上限（以位元組/秒為單位）) /增長率 (（以位元組/秒為單位）) = 每秒影響 (的時間)**

若偵測時間的長度超過影響時間，DoS 攻擊可能會順利完成。 若偵測時間短于影響時間，則攻擊服務應保持線上，且可供緩解策略成功時存取。

因此，防禦 DoS 攻擊有兩個主要策略：

- 增加容量提高容量上限 (，進而提供更多時間來偵測攻擊) ;或
- 縮短偵測攻擊的時間。

使用 Microsoft 雲端服務的一項安全性好處是，Microsoft 服務以經濟划算的方式為雲端客戶提供強網路保護。 甚至在大規模的情況下，都必須在吸收、偵測和緩解之間達到平衡。 為了找出這種平衡點，Microsoft 調查了攻擊成長率，以估計 Microsoft 服務需要吸收的數量。

## <a name="denial-of-service-defense-strategy"></a>阻絕服務攻擊策略

針對網路型 DoS 攻擊所防禦的 Microsoft 策略，因規模和全球化等量而異。 這種規模可讓 Microsoft 利用大多數其他組織無法使用的策略及技術。 我們的 DoS 策略的基石是我們的全球平臺。 Microsoft 與網際網路提供者、對等提供者 (公開和私營) ，以及世界各地的私營公司。 這項服務可提供 Microsoft 的大量網際網路服務，讓 Microsoft 能夠吸收跨越大型 surface 區域的攻擊。

隨著 Microsoft 的 edge 容量隨著時間成長，對個別 edge 的攻擊意義會大幅降低。 由於這一降低，Microsoft 已將其 DoS 防護系統的偵測和緩解元件隔開。 Microsoft 會在地區性資料中心部署多層偵測系統，以偵測其飽和點較接近的攻擊，同時維持 edge 節點的全域緩解。 此策略可確保 Microsoft 服務可以處理多個同時進行的攻擊。

Microsoft 對 DoS 攻擊所採用的最有效且低成本的防禦措施之一，是減少服務攻擊面。 不需要的流量會在網路 edge 中斷，而不會分析、處理及清理資料內聯。

在使用公用網路的介面上，Microsoft 會針對防火牆、網路位址轉譯和 IP 篩選功能使用特殊用途的安全性裝置。 Microsoft 也會使用全域同等成本的多重路徑 (ECMP) 路由。 全域 ECMP 路由是一個網路架構，可確保有多個通用路徑可以到達服務。 針對每個服務使用多個路徑時，DoS 攻擊會限制于發起攻擊的地區。 其他地區應受到攻擊的影響，因為使用者可能會使用其他路徑來到達這些地區的服務。 Microsoft 也已開發內部 DoS 相互關聯和偵測系統，使用流程資料、效能測量及其他資訊，以快速偵測 DoS 攻擊。

若要進一步保護我們的雲端服務，Microsoft 365 會使用分散式的拒絕服務 (DDoS) 防禦系統內內置於 Microsoft Azure 的連續監控和滲透測試程式。 Azure DDoS 防護系統設計不僅可經受外部攻擊，還會為其他 Azure 承租人發起攻擊。 Azure 使用標準偵測和緩解技術，例如 SYN cookie、速率限制和連線限制，以防範 DDoS 攻擊。 為了支援我們的自動防護，跨工作負載 DoS 事件回應小組識別各小組的角色與責任、升級的準則，以及跨受影響團隊之事件處理的通訊協定。

對目標所發動的大部分 DoS 攻擊是在網路 (L3) 和傳輸 (L4) OSI (OSI [) 的層](/windows-hardware/drivers/network/windows-network-architecture-and-the-osi-model) 級。 位於 L3 和 L4 層的攻擊是專門用來淹沒網路介面或服務，其攻擊流量會淹沒資源，並拒絕回應合法流量的能力。 為了防範 L3 和 L4 攻擊，Microsoft 的 DoS 解決方案會使用資料中心路由器的流量採樣資料，以保護基礎結構及客戶目標。 流量採樣資料會由網路監控服務進行分析，以偵測攻擊。 偵測到攻擊時，自動防護機制會發起緩解攻擊，並確保客戶面臨的攻擊流量不會造成宣傳者損毀或降低其他客戶服務的網路服務品質。

## <a name="application-level-defenses"></a>應用層級防護

Microsoft 工程小組遵循 [Microsoft Operational Security 保障](https://www.microsoft.com/SDL/OperationalSecurityAssurance) 所設定的嚴格標準，協助保護客戶資料。 Microsoft 的雲端服務是專為支援高負載而建立，可協助防範應用層級的 DoS 攻擊。 Microsoft 365 的向外延展架構跨多部全球資料中心散佈服務，其相關工作負載具有區域隔離和工作負載特有的節流功能。

客戶所在的國家或地區，客戶的系統管理員會在服務的初始設定中識別該客戶資料的主要儲存位置。 根據主要/備份策略，在重複資料中心之間複製客戶資料。 主要資料中心會裝載應用程式軟體，以及軟體中所執行的所有主要客戶資料。 備份資料中心提供自動容錯移轉。 如果主要資料中心因任何原因而停止運作，則要求會重新導向到備份資料中心內的軟體和客戶資料的複本。 在任何指定的時間，都可能會在主要或備份資料中心處理客戶資料。 跨多個資料中心散佈資料，可在一部資料中心遭到攻擊時減少受影響的面範圍。 此外，受影響的資料中心內的服務可快速重新導向至次要資料中心，以便在攻擊期間維持可用性，並在緩解攻擊之後重新導向主要資料中心。

隨著 DoS 攻擊的另一項減輕，個別的工作負載包括管理資源使用狀況的內建功能。 例如，Exchange Online 和 SharePoint Online 中的節流機制都是多種階層式方法，以防禦 DoS 攻擊。
