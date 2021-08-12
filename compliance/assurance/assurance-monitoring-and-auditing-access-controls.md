---
title: Microsoft 365監視和審計存取控制
description: 摘要： Microsoft 365 內可用之監控和審核存取控制的摘要。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
search.appverid:
- MET150
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
f1.keywords:
- NOCSH
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: e374b22212bce461329e14764a3b35eaa76d5f27fd340e64b9b64fb26ecf35f6
ms.sourcegitcommit: af1925730de60c3b698edc4e1355c38972bdd759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54290577"
---
# <a name="monitoring-and-auditing-access-controls-in-microsoft-365"></a>監視和審計 Microsoft 365 中的存取控制

Microsoft 會對 Microsoft 365 內的所有委派、許可權和作業執行大量監控和審核。 Microsoft 365 存取控制是以最低許可權原則為基礎的自動化程式，且包含資料存取控制和審核：

- 所有允許的存取可對唯一的使用者進行追蹤。 系統管理員負責處理客戶內容。
- 會捕獲存取控制要求、核准和管理作業記錄檔，以進行安全性和惡意事件的分析。
- 存取層級會以接近即時的安全性群組成員資格來檢查，以確保只有具備授權的業務理由和符合資格需求的使用者才可以存取系統。
- Microsoft 365，其存取控制及支援服務（包括 Azure Active Directory 和實體資料中心）都會定期以獨立協力廠商進行審核，以符合[ISO/IEC 27001](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27001)、 [ISO/IEC 27018](https://www.microsoft.com/TrustCenter/Compliance/iso-iec-27018)、 [SOC](https://www.microsoft.com/TrustCenter/Compliance/SOC)、 [FedRAMP (](https://www.microsoft.com/TrustCenter/Compliance/FedRAMP)Office 365) ，以及其他[標準](https://www.microsoft.com/TrustCenter/Compliance?service=Office#Icons)。
- Microsoft 365 工程師必須進行年度安全性訓練，請流覽更高的 access 最佳程式，並認可 Microsoft 的安全性和隱私權原則，以維護服務的權利。

偵測到可疑活動時（例如短期間內的多個失敗的登入），會觸發自動提醒。 Microsoft 365 的安全性回應小組使用電腦學習和大量資料分析，以查看和分析活動、尋找不規則的存取模式，以及主動回應反常和違法的活動。 Microsoft 也採用一支專門的滲透測試小組，並在週期性的紅色小組和藍色小組練習中尋找，以找出服務中的安全性和存取控制問題。 客戶可以使用「審核報告」和 Microsoft 365 所提供的管理活動 API，來驗證存取控制系統的效能。

如需詳細資訊，請參閱 Microsoft 365 中的[Office 365 管理活動 API 參考](/office/office-365-management-api/office-365-management-activity-api-reference)和[審核與報告](assurance-auditing-and-reporting-overview.md)。
