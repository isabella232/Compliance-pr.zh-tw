---
title: Microsoft 365 中的資料復原
description: 在本文中，瞭解 Microsoft 365 中的資料恢復功能和復原的設計和原則。
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
ms.openlocfilehash: 48fe50347e7e81c7e5f8552299c04a268b8b449c
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482106"
---
# <a name="data-resiliency-in-microsoft-365"></a>Microsoft 365 中的資料恢復功能

考慮到雲端計算的複雜性質，Microsoft 很注意，如果發生問題，則不是這樣。 我們設計雲端服務，以最大化可靠性，並在發生錯誤時將負面影響降至最低。 我們已超越信賴複雜實體基礎結構的傳統策略，而且我們已直接在雲端服務中建立冗余。 我們採用複雜的實體基礎結構和更多智慧軟體的組合，將資料恢復到我們的服務中，並為我們的客戶提供高可用性。

## <a name="resiliency-and-recoverability-are-built-in"></a>恢復功能和可恢復性是內建

以恢復性和復原的方式開始，假設基礎基礎結構和程式在某些情況下會失敗：硬體 (基礎結構) 會失敗、人工會犯錯誤，軟體也會有錯誤。 雖然軟體發展人員不會考慮到雲端之前未考慮到這些事項，但在典型的 IT 實施中處理這些問題的方式是在雲端之前是不同的：

- 首先，硬體和基礎結構保護非常重要。 這種結構意味著具有99.99% 可靠性的資料中心需要大量的電源和網路冗余，而且伺服器是以硬體型集群、雙電源、雙網路介面，以及類似的方式實施。
- 其次，處理常式是極其重要的。 運作小組維護嚴格的程式、對 windows 的變更所採用的工作，而且經常會產生大量的專案管理工作負載。
- 第三，部署是以 glacial 節奏進行。 部署不含來源的程式碼表示要等候修補程式版本，主要版本版本則涉及硬體取代和大量的資本 outlay。 此外，修正問題的唯一方法是回復。 因此，大部分的 IT 組織只會部署主要版本，以避免工作維持最新狀態。
- 最後，已部署的系統規模和其 interconnectedness 的層級已遠遠小於現在。

目前，客戶預期來自 Microsoft 的連續創新，但不會降低品質，這是 Microsoft 的服務和軟體以恢復性和恢復為基礎而建立的原因之一。

## <a name="microsoft-365-data-resiliency-principles"></a>資料恢復原則 Microsoft 365

恢復性指的是雲端架構服務可經受某些類型的失敗，但仍可從客戶的觀點完全運作的能力。 資料恢復意味著不管 Microsoft 365 中發生的失敗為何，重要的客戶資料仍保持不變且不受影響。 為做到這一點，Microsoft 365 服務都是圍繞五個特定的恢復原則設計的：

- 有重要且非重要的資料。 非重要資料 (例如，郵件是否已讀取) 可以在少見的失敗案例中刪除。 重要資料 (例如，客戶資料) （例如電子郵件訊息）應以極高的成本加以保護。 在設計目標中，傳遞的郵件訊息永遠很重要，也就是郵件已讀取的情況不重要。
- 客戶資料的複本必須分割成不同的容錯區域，或盡可能多的容錯網域 (例如，資料中心，可透過單一認證 (程式、伺服器或操作員) ) 進行存取，以提供失敗隔離。 
- 必須監視重要的客戶資料，以失敗任何原子性、一致性、隔離性、耐用性 (ACID) 部分。
- 客戶資料必須受到保護，避免損毀。 必須主動掃描或監視、修復和恢復。
- 客戶動作中大部分的資料遺失結果，讓客戶可以使用 GUI 自行進行復原，讓他們能夠還原意外刪除的專案。

透過將雲端服務組建至這些原則，並結合可靠的測試和驗證，Microsoft 365 能夠符合和超過客戶的需求，同時又可確保平臺的持續創新和改進。

## <a name="related-articles"></a>相關文章

- [處理資料損毀](assurance-dealing-with-data-corruption.md)
- [惡意程式碼與勒索軟體防護](assurance-malware-and-ransomware-protection.md)
- [監視及自我修復](assurance-monitoring-and-self-healing.md)
- [Exchange資料恢復](assurance-exchange-data-resiliency.md)
