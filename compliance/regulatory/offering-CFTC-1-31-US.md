---
title: 商品先期傭金 (CFTC) 規則 1.31 (c-d) 美國
description: 獨立評估公司已驗證，Azure 和 Office 365 可協助財務公司符合 CFTC 規則1.31 記錄保留和不可變的儲存需求。
keywords: Microsoft 365, 合規性, 方案
ms.localizationpriority: medium
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmazz
manager: laurawi
audience: itpro
ms.collection:
- M365-security-compliance
- MS-Compliance
hideEdit: true
titleSuffix: Microsoft Compliance
ms.openlocfilehash: 8bb9f380d57e932576c969f10512f508de7c6ada
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158740"
---
# <a name="commodity-futures-trading-commission-cftc-rule-131c-d-united-states"></a>商品先期傭金 (CFTC) 規則 1.31 (c-d) 美國

## <a name="about-cftc-rule-13c-d"></a>關於 CFTC 規則 1.3 (3-d) 

[商品先期交易委員會](https://www.cftc.gov/) (CFTC) （一個獨立的美國聯邦代理商）來調節商品先期備貨和選項市場，以及最近的換購市場。  
  
長期 CFTC 規則1.31 會定義由 SEC Rule 17a-4 (f) 所建立的記錄保留需求。 此外，它會指定必須維護電子記錄五年，而且原始的兩年內保留「可隨時存取」，而且在整個保留期間內，可供傭金或美國司法部門進行檢查。  
  
在2017中， [CFTC 修訂其規則](https://www.cftc.gov/sites/default/files/idc/groups/public/@lrfederalregister/documents/file/2017-11014a.pdf)，修正並現代化其保留規定，以採用較少的規範性標準，可提供更多彈性以維護記錄的方式。 此修訂版會使規則的技術中立，讓規定的實體可以選擇最適合其業務的技術，同時維護保證保留程式之可靠性的保護措施。 修改後的規則會從兩年內移除組織維護原始記錄的需求，但保留5年期的維護期間，這兩個公司的 harmonizes 做法是由 CFTC 和 SEC 管制。

## <a name="microsoft-and-cftc-rule-131c-d"></a>Microsoft 和 CFTC 規則 1.31 (3-d) 

金融服務客戶（如世界上最受管制的行業之一）受到複雜的置備，例如保留金融交易和相關通訊的非擦除和不可修改的狀態。 其中一個最具規範性的規則1.31 是美國商品先期傭金 (CFTC) ，可 stipulates 對管制實體的嚴格需求，以選擇在電子化儲存介質上保留書籍和記錄。 儲存的記錄必須防篡改，但不能變更或刪除，直到指定的保留期間為止。 Microsoft Azure使用具有保留鎖定之原則鎖定和 Microsoft Office 365 的「不可變的 Blob 儲存體，可協助金融機構符合 CFTC 規則 1.31 (3-d) 的儲存需求。

### <a name="microsoft-azure"></a>Microsoft Azure

若要評估 Azure 與 CFTC 規則1.31 的相容性 (3-d) 中，Microsoft 保留了專門從事記錄管理和資訊管理、Cohasset 關聯的獨立評估事務所。 在產生的報告中， [CFTC 1.31 (c)  (d) 合規性評估： Microsoft Azure 儲存體](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)，Cohasset 會驗證[Azure 永恆 blob 儲存體](/azure/storage/blobs/storage-blob-immutable-storage)時使用原則鎖定選項，當用來保留以不可讀寫的 blob 和不可讀寫的 blob （ (格式）時，會符合 CFTC 規則的原則型需求。 每個 Blob (記錄) 都會受到保護，無法進行修改、覆寫或刪除，直到必要的保留期間到期併發行任何關聯的合法保留期間為止。 具有敏感工作負載的軟體提供者和合作夥伴現在可以依靠 Azure 不可篡改的 Blob 儲存體做為記錄保留的一站式雲端方案。 金融機構現在可以組建自己的應用程式，利用這些功能，並保持不相容。

### <a name="microsoft-365"></a>Microsoft 365

針對[CFTC 1.31 (c)  (d) ](/microsoft-365/compliance/retention-regulatory-requirements#sec-17a-4f-finra-4511c-and-cftc-131c-d)需求，Cohasset 驗證 Microsoft 365 包含封存功能，可讓受管制的客戶（包括經紀人代理商）儲存資料，以協助其遵守記錄保留的 SEC 需求。 Microsoft 365 中的保留功能可協助保留廣泛的資料，包括電子郵件、語音信箱、共用檔、立即訊息和協力廠商資料。 尤其是，在 Microsoft 365 中封存可讓客戶設定全域或細微的郵件保留原則，以儲存定義期間內的資料，而不是以不可重寫、不可讀寫的格式使用。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- [Azure](https://aka.ms/AzureCompliance)
- [Office 365](https://aka.ms/o365-compliance-framework)

## <a name="audits-reports-and-certificates"></a>稽核、報告和認證

- [Azure & CFTC 規則1.31： SEC 17a-4 (f) & CFTC 1.31 (c-d) 相容性評估 Azure 儲存體](https://azure.microsoft.com/resources/azure-immutable-storage-assessment-for-sec-17a-4f-by-cohasset/)
- Office 365 & CFTC 規則1.31： Office 365、資料保留和 SEC 規則17a-4 規範中的封存

## <a name="how-to-implement"></a>實作方法

- [金融服務法規](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)：適用于雲端計算和 Microsoft online 服務之重要的 US 規章原則的符合性地圖。
- [風險評定與合規性指南](https://aka.ms/RiskGovernanceGuide)：建立 Microsoft 雲端服務風險評定的監管模型和調整通知。
- [金融使用案例](/azure/industry/financial/)：使用案例概覽、課程及其他資源建立適用於金融服務的 Azure 解決方案。

## <a name="resources"></a>資源

- [Microsoft 金融服務合規性計劃](https://aka.ms/FSCP-Print)
- [Microsoft 商務用雲端服務與金融服務](https://www.microsoft.com/trustcenter/cloudservices/financialservices)
- [Azure 的金融服務合規性](https://azure.microsoft.com/resources/videos/azurecon-2015-financial-services-compliance-in-azure/)
- [Microsoft Office 365保留原則](/office365/securitycompliance/retention-policies)
- [Microsoft 金融服務部落格](https://techcommunity.microsoft.com/t5/Financial-Services-Blog/bg-p/FinancialServicesBlog)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
