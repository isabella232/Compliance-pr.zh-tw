---
title: 安全性開發和作業概述
description: 深入瞭解 Microsoft 365 中的安全性開發和作業
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
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
ms.openlocfilehash: 7c6752b84470eebbdb6ad78c212361156dea957b
ms.sourcegitcommit: 626b0076d133e588cd28598c149a7f272fc18bae
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/30/2020
ms.locfileid: "49506243"
---
# <a name="security-development-and-operations-overview"></a>安全性開發和作業概述

## <a name="how-does-microsoft-implement-secure-development-practices"></a>Microsoft 如何實施安全的開發做法？

Microsoft 的安全性開發生命週期 (SDL) 是一種安全性保證程式，主要是開發及作業安全的軟體。 SDL 為 Microsoft 的開發人員和工程師提供詳細的、可測量的安全性需求，以降低產品和服務中的漏洞數量和嚴重性。 所有 Microsoft 軟體發展小組都必須遵循 SDL 的需求，而且我們連續更新 SDL，以反映威脅的變化環境、行業最佳作法，以及法規遵從性的法規標準。

## <a name="how-does-microsofts-sdl-improve-application-security"></a>Microsoft 的 SDL 如何改善應用程式安全性？

Microsoft 的 SDL 程式會考慮到開發的五個階段：需求、設計、執行、驗證及發行。 其開始的方式是定義具有安全性的軟體需求。 為做到這一點，我們會詢問有關應用程式必須完成之專案的安全性相關問題。 應用程式是否需要收集機密資料？ 應用程式是否會執行敏感或重要的任務？ 應用程式是否需要接受來自不受信任來源的輸入？

識別相關的安全性需求之後，我們會設計軟體，以包含符合這些需求的安全性功能。 我們的開發人員會在程式碼中執行 SDL 和設計需求，我們會透過手動程式碼檢查、自動化的安全性工具和滲透測試來驗證。 最後，在發行程式碼之前，新功能和材料變更會進行最後的安全性和隱私權檢查，以確保符合所有需求。

## <a name="how-does-microsoft-test-source-code-for-common-vulnerabilities"></a>Microsoft 如何測試常見漏洞的原始程式碼？

為了支援我們的開發人員在程式碼開發期間和發行之後實施安全性需求，Microsoft 提供了一套安全的開發工具，以自動檢查原始程式碼中的安全性缺陷和弱點。 Microsoft 會定義及發行開發人員使用的核准工具清單，例如編譯器和開發環境，以及內建的安全性檢查，可在 Microsoft 組建管線中自動執行。 我們的開發人員使用最新版的已核准工具，利用新的安全性功能。

在將程式碼簽入到版本分支之前，SDL 必須個別的檢閱者手動進行程式碼審查。 程式碼檢閱者會檢查是否有編碼錯誤，並確認程式碼變更符合 SDL 和設計需求、傳遞功能和安全性測試，以及可靠執行。 他們也會檢查相關的檔、驗證和相依性，以確保代碼變更已適當地記錄，而且不會造成非預期的副作用。 如果檢閱者在程式碼檢查期間發現問題，他們可以要求提交者以建議的變更和其他測試重新提交程式碼。 程式碼檢閱者可能也會決定完全封鎖不符合需求的程式碼。 當檢閱者認為程式碼符合要求之後，檢閱者會提供核准，在程式碼可以繼續下一個部署階段之前必須先進行核准。

除了安全的開發工具和手動代碼檢查之外，Microsoft 也會使用自動化的安全性工具，強制執行 SDL 的要求。 這許多工具都是內置於認可管線中的，而且會在已存回新的組建時，自動分析安全性缺陷的程式碼。 範例包括分析內嵌機密代碼的常見安全性缺陷和認證掃描程式的靜態程式碼分析。 在新的組建可以透過安全性檢查並經過核准以進行發行之前，必須先修正由自動安全性工具所發現的問題。

## <a name="how-does-microsoft-manage-open-source-software"></a>Microsoft 如何管理開放來源軟體？

Microsoft 採用高級策略來管理開放來源安全性，其利用工具和工作流程的設計：

- 瞭解產品和服務中使用哪些開放來源元件。
- 追蹤這些元件的使用場合和方式。
- 判斷這些元件是否有任何弱點。
- 在發現會影響這些元件的漏洞時會正確回應。

Microsoft 工程小組會為產品或服務中包含的所有開放來源軟體的安全性維護責任。 為做到這一點，Microsoft 已透過 CG 將基本功能建立到工程系統中，以自動化開放來源偵測、法律需求工作流程，以及對易受攻擊元件的警示。 自動 CG 工具會針對開放來源元件及相關的安全性弱點或法律義務，掃描 Microsoft 的版本。 已探索的元件會註冊並提交至適當的小組以進行商務及安全性檢查。 這些檢查的設計目的是要評估與開放來源元件相關的任何法律義務或安全性弱點，並在核准元件進行部署之前加以解決。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與安全性開發及作業相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | 南美-3：系統開發週期 | 2020年9月24日 |
| [ISO 27001/27002 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=1e84a14a-2468-45ac-9412-5e53250d57ec&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.2：變更管理控制措施 <br> 14.2：開發及支援流程中的安全性 | 2020 年 2 月 22 日 |
| [ISO 27017 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7864d4f-e053-4cc4-a964-fa526d07c3be&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuide?command=Download&downloadType=Document&downloadId=8ee1e46b-2ada-4e7b-bb7d-4c55a8cb6fcd&docTab=4ce99610-c9c0-11e7-8c2c-f908a777fa4d_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=70de0999-5451-43a3-9ef4-761e8fbfb1a3&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.2：變更管理控制措施 <br> 14.2：開發及支援流程中的安全性 | 2020 年 2 月 22 日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b07c0f7b-6bd5-4544-8255-7a5f14bf914a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA-03：風險管理 <br> CA-18：變更管理 <br> CA-19：變更監控 <br> CA-21：變更測試 <br> CA-38：基準設定 <br> CA-46：安全性檢查 | 2019 年 9 月 30 日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=fa062990-e758-4ddc-ace3-7fb21a301d09&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Rep-11e9-b9e1-290b1eb4cdeb_SOC_/_SSAE_16_Reports) | CA-03：風險管理 <br> CA-18：變更管理 <br> CA-19：變更監控 <br> CA-21：變更測試 <br> CA-38：基準設定 <br> CA-46：安全性檢查 | 2019 年 9 月 30 日 |

## <a name="resources"></a>資源

- [Microsoft 的安全性開發週期](https://www.microsoft.com/securityengineering/sdl)
