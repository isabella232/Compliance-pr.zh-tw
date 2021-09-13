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
ms.localizationpriority: medium
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: b74c004e63838900f87c774a8acf84ab8aeb03d4
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158699"
---
# <a name="security-development-and-operations-overview"></a>安全性開發和作業概述

## <a name="how-does-microsoft-implement-secure-development-practices"></a>Microsoft 如何實施安全的開發做法？

Microsoft 的安全性開發生命週期 (SDL) 是一個著重於開發及操作安全軟體的安全性保證程序。 SDL 為 Microsoft 的開發人員和工程師提供了詳細且可測量的安全性需求，以降低我們產品和服務弱點的數量和嚴重性。 所有 Microsoft 軟體發展小組都必須遵循 SDL 的需求，而且我們連續更新 SDL，以反映威脅的變化環境、行業最佳作法，以及法規遵從性的法規標準。

## <a name="how-does-microsofts-sdl-improve-application-security"></a>Microsoft 的 SDL 如何改善應用程式安全性？

Microsoft 的 SDL 程式會考慮到開發的五個階段：需求、設計、執行、驗證及發行。 首先是定義軟體需求，並考量安全性。 為了達到此目的，我們會詢問有關應用程式必須完成之專案的安全性相關問題。 應用程式是否需要收集敏感性資料？ 應用程式是否會執行敏感性或重要工作？ 應用程式是否需要接受不受信任的來源提供的輸入？

找出相關的安全性需求後，我們即可設計軟體以納入符合這些需求的安全性功能。 我們的開發人員會在程式碼中實作 SDL 和設計需求，而我們可透過手動程式碼檢閱、自動化安全性工具和滲透測試，加以驗證。 最後，在發行程式碼之前，新功能和材料變更會進行最後的安全性和隱私權檢查，以確保符合所有需求。

## <a name="how-does-microsoft-test-source-code-for-common-vulnerabilities"></a>Microsoft 如何測試常見漏洞的原始程式碼？

為了支援我們的開發人員在程式碼開發期間和發行後執行安全性需求，Microsoft 提供了一套安全開發工具，可自動檢查原始程式碼中的安全性瑕疵和弱點。 Microsoft 會定義及發行開發人員使用的核准工具清單，例如編譯器和開發環境，以及內建的安全性檢查，可在 Microsoft 組建管線中自動執行。 我們的開發人員使用最新版的核准工具，以利用新的安全性功能。

在將程式碼簽入到版本分支之前，SDL 必須個別的檢閱者手動進行程式碼審查。 程式碼檢閱者會檢查程式碼錯誤，並確認程式碼變更符合 SDL 和設計需求、通過功能和安全性測試，並能確實可靠地執行。 他們也會檢查相關聯的文件、設定和相依性，以確保系統會適當地記錄程式碼變更，且不會造成非預期的副作用。 如果檢閱者在程式碼檢閱期間發現問題，他們可以要求提交者以建議的變更和其他測試重新提交程式碼。 程式碼檢閱者也可以決定完全封鎖不符合需求的程式碼簽入。 當檢閱者認為程式碼符合要求之後，檢閱者會提供核准，在程式碼可以繼續下一個部署階段之前必須先進行核准。

除了安全的開發工具和手動代碼檢查之外，Microsoft 也會使用自動化的安全性工具，強制執行 SDL 的要求。 這許多工具都是內置於認可管線中的，而且會在已存回新的組建時，自動分析安全性缺陷的程式碼。 範例包括分析內嵌機密代碼的常見安全性缺陷和認證掃描程式的靜態程式碼分析。 在新的組建可以透過安全性檢查並經過核准以進行發行之前，必須先修正由自動安全性工具所發現的問題。

## <a name="how-does-microsoft-manage-open-source-software"></a>Microsoft 如何管理開放來源軟體？

Microsoft 採用高級策略來管理開放來源安全性，其使用工具和工作流程，其設計目的是：

- 了解我們的產品和服務中使用哪種開放原始碼元件。
- 追蹤這些元件的使用位置和方式。
- 判斷這些元件是否具有任何弱點。
- 發現影響這些元件的弱點時，作出適當回應。

Microsoft 工程小組會負責產品或服務中包含的所有開放原始碼軟體的安全性。 為了在規模上達成這項安全性，Microsoft 已透過元件控管 (CG) ，將基本功能建立到工程系統中，以自動化開放來源偵測、法律需求工作流程，以及易受攻擊元件的警示。 自動 CG 工具會針對開放來源元件及相關的安全性弱點或法律義務，掃描 Microsoft 的版本。 找到的元件會註冊並提交至適當的小組，以用於商務和安全性審查。 這些審查旨在評估與開放原始碼元件相關的任何法律義務或安全性弱點，並在核准部署元件前加以解決。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與安全性開發及作業相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.2：變更管理控制措施 <br> 14.2：開發及支援流程中的安全性 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.2：變更管理控制措施 <br> 14.2：開發及支援流程中的安全性 | 2020 年 12 月 2 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=b8721ebd-af20-42fe-b22f-8332b0a19517&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | SDL-1：安全性開發生命週期 (SDL) 方法 <br> SDL-2：版本中所述的安全性控制需求 <br> SDL-4：隔離測試與實際執行環境 <br> SDL-6：以原始程式碼組建進行惡意程式碼掃描 <br> SDL7：半年 SDL 檢查 | 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | 南美-3：系統開發週期 | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 12.1.2：變更管理控制措施 <br> 14.2：開發及支援流程中的安全性 | 2021 年 4 月 20 日 |
| [SOC 1](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-03：風險管理 <br> CA-18：變更管理 <br> CA-19：變更監控 <br> CA-21：變更測試 <br> CA-38：基準設定 <br> CA-46：安全性檢查 | 2020月24日 |

## <a name="resources"></a>資源

- [Microsoft 的安全性開發週期](https://www.microsoft.com/securityengineering/sdl)
