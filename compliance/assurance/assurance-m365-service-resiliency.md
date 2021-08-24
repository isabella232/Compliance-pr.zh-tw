---
title: Microsoft 365 中的內建服務彈性
description: Microsoft 365 服務恢復性的描述
author: robmazz
ms.author: robmazz
manager: laurawi
ms.reviewer: sosstah
f1.keywords:
- NOCSH
audience: ITPro
ms.topic: article
ms.service: o365-solutions
ms.localizationpriority: medium
ms.collection:
- M365-subscription-management
- Strat_O365_Enterprise
- MS-Compliance
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: 592cfcdf3da33e6c26e90d5a83fb6bcd3b4241e0
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58481915"
---
# <a name="built-in-service-resiliency-in-microsoft-365"></a>Microsoft 365 中的內建服務彈性

身為您的雲端共同作業提供者，Microsoft 意識到我們需要透過提供能一致地運作且您的使用者喜愛的解決方案，來持續獲得您的信任。 任何指定的服務無法使用時，即稱為停機時間。 每個 Microsoft 365 服務的停機時間定義可能不同，但它們通常會集中在使用者無法使用服務基本功能的任何一段時間。 例如，以下是從 Microsoft 365 服務等級協定所取得 SharePoint Online 停機時間的定義：

**「SharePoint Online 停機時間**：使用者無法讀取或寫入他們擁有適當權限的 SharePoint Online 網站集合任何部分的任何一段時間。」

您可以在[服務等級協定](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)中尋找每個服務的停機時間定義。

為了將停機時間降至最低 (無論是計劃中或非預期的)，Microsoft 365 服務的設計和運作是要高度可用並對失敗具復原能力，其方法是專注於四個區域：

## <a name="activeactive-design"></a>主動/主動設計

在 Microsoft 365 中，我們會讓所有服務以主動/主動設計來進行設計及運作，以提升復原能力。 這項設計是指執行服務的多個實例，可對使用者要求作出回應，而且會在地理位置分散的資料中心內主控。 所有使用者流量會透過 Microsoft Front Door 服務進入，並會自動路由所找到最佳的服務執行個體，並解決任何服務失敗，以防止或減少對客戶的影響。

## <a name="reduce-incident-scope"></a>減少事件範圍

服務事件的範圍是由嚴重程度、其持續時間和受影響的客戶數來衡量。 我們透過下列方式努力限制所有事件的範圍：

- 讓每個服務的多個執行個體彼此分開
- 以受控制、使用驗證環的漸進方式來部署更新，這樣一來，可能從更新引發的任何問題就可以在部署程序中及早偵測並緩和。 這項設計可在需要時進行必要的更新，並且第一次會發生在 Microsoft (內環) 內部的小群組中（如所有 140000 Microsoft 員工 (ring 2) ），然後針對初期的使用方式，所有客戶以全域方式 (ring 4) 。
- 透過自動化來使得監控獲得改善。 Microsoft 365 是大型服務，SLA 目標的執行時間很高。 在服務事件的最開始時，如果需要人員參與偵測和回應，我們便無法以夠快的速度回應來滿足 SLA。 自動化是快速且有效的服務事件偵測和回應的關鍵。 越快找到問題，便能越快解決問題。

隨著 Microsoft 365 服務架構內建的主動/主動功能，這些努力會減輕服務事件中的嚴重性、持續時間和受影響客戶數目。  

## <a name="fault-isolation"></a>錯誤隔離

正因為服務是以主動/主動的方式設計和作業，並彼此分開，以避免其中一個發生問題會影響另一個，因此服務的基礎程式碼是使用稱為錯誤隔離的類似分割準則來開發。 錯誤隔離措施是在基礎程式碼內本身進行的累加的保護。 這些措施可協助防止一個區域中的問題從串聯到其他作業區域。
故障隔離量值會在開發和服務的各個階段（包括程式碼開發、服務部署、負載平衡及資料庫複寫）上套用。

Microsoft 安全性開發生命週期 (SDL) 進一步提升復原能力，並包含一組支援安全性與合規性需求的做法。 SDL 可指引我們的開發人員建立具備復原能力、安全與合規性的服務。 SDL 的重要元素包括程式碼檢閱、威脅模型、滲透測試，以及整個 Microsoft 雲端標準化的事件回應程序。

Microsoft 365 服務是高度互連的，但是其背後的系統和技術會以一種方式來加以設計，以限制一個服務事件對其他服務之影響的 spilling。 例如，影響 Exchange Online 的問題不會影響 Teams 中的核心功能，或是 SharePoint Online 中的搜尋功能問題，也不會影響使用者上傳或下載檔案的能力。

## <a name="continuous-service-improvement"></a>持續改善服務

當我們遇到事件時，我們會認真對待。 畢竟，我們的備援雲端架構和嚴謹的內部程序目標都是要讓我們的服務保持可存取。 在事件期間，我們的監控會快速偵測受影響的服務，如果您的租使用者受到影響，您會立即透過各種管道通知您。 同時，工程師會依照定義明確的程序來對問題進行分級，並採取必要的步驟儘快恢復正常作業。 服務再次正常運作之後，我們會舉行事件後檢討，做為持續改善服務週期的一部分。 在事件後檢討期間，我們會找出事件的根本原因，以及修正問題所需的項目。 然後我們會從狀況中習得了教訓，並將它套用到我們所有產品套件的設計與運作。 透過這種知識，我們可以防止與其他服務和其他客戶產生影響相同的根本原因。
