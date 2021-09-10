---
title: 供應商管理概觀
description: 深入瞭解 Microsoft 365 中的供應商管理
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH'
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
ms.openlocfilehash: 3b0a4c7f12eba49c252f71e47eda1685fd4d41a4
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58947195"
---
# <a name="supplier-management-overview"></a>供應商管理概觀

## <a name="how-does-microsoft-manage-risk-related-to-suppliers"></a>Microsoft 如何管理與供應商相關的風險？

與協力廠商公司的 Microsoft 合作夥伴，以協助滿足客戶的需求。 這些協力廠商公司稱為供應商或 subprocessors。 在 Microsoft 的供應商安全性和隱私權由我們的 [供應商安全性和隱私權保證 (SSPA) 計畫](https://www.microsoft.com/procurement/sspa?activetab=pivot1%3aprimaryr6)，針對所有與 Microsoft 合作來提供我們線上服務之供應商的企業範圍的需求。 當 SSPA 計畫提供我們的供應商基礎的綜合控管和管理時，個別的業務單位可能會維護其供應商的其他需求。

## <a name="how-does-microsofts-supplier-security-and-privacy-assurance-sspa-program-protect-customer-data"></a>Microsoft 的供應商安全性和隱私權保證 (SSPA) 計畫是否會保護客戶資料？

SSPA 是 Microsoft 採購、公司外部和法律事務之間的合作關係，以及公司的安全性，以確保供應商遵循 Microsoft 的隱私權和安全性原則。 SSPA 的範圍涵蓋所有處理個人資料或 Microsoft 機密資料的供應商。 SSPA 計畫登記包含符合 Microsoft 的資料保護需求 (DPR) 。 DPR 是由提供者在開始與 Microsoft 開始簽約之前必須執行的安全性和隱私權控制組成。 所有已註冊的供應商會自我證明，以每年符合 DPR。

DPR 需求的適用範圍是以六種不同的資料處理類別為基礎，可在 SSPA 的登記中核准。 這些類別是用來識別與提供者提供給 Microsoft 的服務相關的風險。 供應商的資料處理設定檔會決定哪些 DPR 控制項會被視為範圍內，以提供適當的資料保護。 處理視為較高風險之資料的供應商必須符合所有的 DPR 需求，而且可能也需要提供獨立的相容性驗證。 Microsoft 購買工具會驗證所有供應商的 SSPA 狀態，包括與 DPR 適用的部分相容性，在允許該供應商的採購之前。

## <a name="what-types-of-subprocessors-provide-services-for-microsoft"></a>哪些類型的 subprocessors 可為 Microsoft 提供服務？

「Subprocessor ' 是 Microsoft 雇傭的協力廠商，其職責包含處理 Microsoft 為處理器的 Microsoft 個人資料。 Microsoft 的 subprocessors 分為三個不同的類別。 每個客戶都必須先示範 SSPA，才可代表在 Microsoft 上處理客戶資料。

- **技術** 轉包處理者會提供用來提供特定 Microsoft 線上服務的技術。 如果客戶部署其中一個服務，則針對該服務所識別的 subprocessors 可能會在協助提供該服務時處理、儲存或存取客戶資料或個人資料。
- **輔助** subprocessors 提供服務，以支援、運作及維護線上服務。 如果客戶部署其中一項服務，識別的 subprocessors 可能會處理、儲存或存取有限的客戶資料或個人資料，同時提供其輔助服務。
- **員工充實** subprocessors 採用兩種不同的形式：在這兩種情況下，個人資料只會在 microsoft 系統上，且受限於 microsoft 的原則和監督工作。

    - 員工擴充轉包處理者會提供可支援、操作和維護 Microsoft 線上服務的員工。 在履行責任的同時，這些轉包處理者可能會接觸客戶資料或個人資料。 例如，轉包處理者可能會對 Microsoft 伺服器執行遠端疑難排解，而這麼做時，他們可能會接觸伺服器損毀傾印記錄中的客戶資料片段。
    - 第二種形式的人員擴充包括 subprocessors 哪些人員與 Microsoft 全職員工共同作業，以支援、操作和維護 Microsoft 線上服務。 當這些轉包處理者與 Microsoft 全職員工一起在工作時，他們可能會接觸已使用假名的資料。

若要遵循 Microsoft 的資料保護需求 (DPR) ，必須使用技術和輔助 subprocessors 來執行存取控制。 這些需求符合或超過 Microsoft 對其客戶在線上服務條款 (OST) 中所做的合約承諾。 從事人員充實工作的供應商，必須對 Microsoft 全職員工使用相同的存取控制措施。

## <a name="how-does-microsoft-onboard-suppliers"></a>Microsoft 的板載供應商是如何？

協力廠商供應商是在上架過程中簽署 Microsoft 主要合約的必要條件。 這份合約會控制 Microsoft 與其供應商之間的關係，並確保供應商關聯性的一致性管理。 作為內架的一部分，供應商會註冊 SSPA，必須先完成所有適用的需求，才能核准任何資料處理類別。 當預訂的資料處理活動符合已核准供應商的資料處理類別時，Microsoft 商務單位只能夠與供應商建立預訂。

## <a name="how-does-microsoft-notify-customers-of-changes-to-suppliers-who-process-their-data"></a>Microsoft 如何向客戶通報處理其資料之供應商的變更？

根據 Microsoft 線上服務資料保護附錄 (DPA) ，Microsoft 對加入任何 subprocessor 進行其他有關通知期間的承諾。 請注意時間範圍取決於 subprocessor 將代表 Microsoft 處理的資料類型。 如 DPA 中所述，Microsoft 承諾向客戶提供通知，至少要有六個月的時間，任何新的 subprocessor 都會處理客戶資料。 對於任何其他個人資料，Microsoft 至少會提供30天的通知。 通知是由 [Microsoft Online Services Subprocessor 清單](https://servicetrust.microsoft.com/ViewPage/TrustDocumentsV3?command=Download&downloadType=Document&downloadId=926b2cf5-6b6e-43ca-9bc3-f73e961aad5f&tab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913&docTab=7f51cb60-3d6c-11e9-b2af-7bb9f5d2d913_Subprocessor_List)的更新所提供。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與供應商管理相關的控制項。

### <a name="azure-and-dynamics-365"></a>Azure 和 Dynamics 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|  
| [ISO 27001/27002](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=d7af5304-3a31-40e6-9abb-e26352305d41&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 15.1：供應商關聯中的資訊安全性 | 2020 年 12 月 2 日 |
| [ISO 27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a3bca0ac-867d-4204-b66b-13665f5f1e8d&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=25718a8a-f34d-41e1-a95a-c49246508787&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 15.1：供應商關聯中的資訊安全性 | 2020 年 12 月 2 日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=e9116047-f327-430c-a83f-166b7e561ad6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=00af6c3e-7f3e-4e0d-8b0e-79f45ef2cef1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br> [認證](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=56904fc3-0942-4ff5-9eef-7cabc751a25c&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) |  8.1：已轉包 PII 處理的披露 | 2020 年 12 月 2 日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=234a0f57-83c1-4afc-a586-a0e7a59592f7&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) <br> [SOC 3](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=75c8cbf6-e456-473c-a05e-34fea888ec2a&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | SOC2-25：供應商風險管理 <br> C5-2：供應商風險設定檔檢查| 2021年3月31日 |

### <a name="office-365"></a>Office 365

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|  
| [FedRAMP](https://compliance.microsoft.com/compliancemanager) | CA-3：系統互連 <br> IA-4：識別碼管理 <br> PS-6：存取協定 <br> PS-7：協力廠商個人安全性 <br> 南美-4：收購程式 <br> 南美-9：外部資訊系統服務 <br> 南美-12：供應鏈保護 | 2020年9月24日 |
| [ISO 27001/27002/27017](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) | 15.1：供應商關聯中的資訊安全性 | 2021 年 4 月 20 日 |
| [ISO 27018](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=8d625374-4f2d-49f8-9d37-a4281ba98222&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) <br><br> [適用性聲明](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=c0df4ce8-c77e-4183-84eb-c8688470d8b1&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_ISO_Reports) |  8.1：已轉包 PII 處理的披露 | 2020月24日 |
| [SOC 2](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-53：協力廠商監控 | 2020月24日 |

## <a name="resources"></a>資源

- [供應商的安全性隱私權和保證計畫](https://www.microsoft.com/procurement/sspa?activetab=pivot1%3aprimaryr6)
