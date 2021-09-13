---
title: 2002 年沙賓法案 (SOX)
description: 金融服務公司可以使用 Microsoft 規範報告來處理其與 Sarbanes-Oxley 法案的相容性。
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
ms.openlocfilehash: 375f7a58db675f3f14bd98ff580919ef40f603f1
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158868"
---
# <a name="sarbanes-oxley-act-of-2002-sox"></a>2002 年沙賓法案 (SOX)

## <a name="sox-overview"></a>SOX 概述

2002 (SOX) 的[Sarbanes-Oxley 法案](https://www.congress.gov/bill/107th-congress/house-bill/3763)是由[證券和 Exchange 傭金](https://www.sec.gov/) (SEC) 所管理的美國聯邦法律。 除此之外，SOX 也需要上市公司的內部控制結構，以驗證其財務報告是否正確反映其財務結果。 SOX 對客戶的內部程式影響很大，尤其是在財務報告的控制項時。 例如，SOX 需求包含內部客戶控制，供您準備及審查財務報表，尤其會影響與財務報告相關的實質性變更的準確性、完整性、效能及公開披露的控制項。

SEC 不會定義或強加 SOX 認證程式。 相反地，它提供公開交易公司的廣泛指導方針，以決定如何遵守 SOX 報表需求。

## <a name="microsoft-and-sox"></a>Microsoft 和 SOX

Microsoft cloud services 客戶遵循 Sarbanes-Oxley 法案 (SOX) 可使用從獨立審核事務所接收的 SOC 1 Type 2 證明，以解決其專屬的 SOX 合規性責任。 這種認證適用于透過財務報告內部控制的報告。

雖然雲端服務提供者沒有任何 SOX 憑證或驗證，但 Microsoft 可協助客戶滿足其 SOX 義務。 例如，SOX 需要內部控制財務報表的準備和審查，尤其會影響財務報告相關材料變更的準確性、完整性、有效性及公開披露的控制項。 為了協助公司，Microsoft 會維護第2級的 SOC 1 類型的證明，以用於報告大量服務，以用於建立大量的應用程式。 它是以美國簽定的公開會計會計師為基礎， (AICPA) 說明認證合約 18 (SSAE 18) 和國際標準的保證合約否。 3402 (ISAE 3402)。  (此認證取代 SAS 70。 ) 

由協力廠商審核公司所產生的「審核報告」會證實 Microsoft 控制項已正確設計，在指定日期的作業中，並在指定的時間週期內有效運作。 客戶可以查看報告，以瞭解 Microsoft control 目標和其控制項的效能，並取得補充性控制項的存取權。

在 Microsoft，我們共同分享與我們客戶相符的責任。 我們提供規範計畫的詳細資料，您可以從驗證協力廠商要求詳細的審計結果來驗證。 不過，最後，您可以決定我們的服務是否符合適用于您公司的特定法律和規定。 例如，有與 SOX 相關的安全性控制措施（例如，使用者存取雲端資源）是您的責任：您的組織必須在您的 SOX 法規遵從性的情況下，開發這些控制項的適當審核。

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure
- [Dynamics 365](https://aka.ms/d365-compliance-list)
- Intune
- Office 365
- Power BI 雲端服務 (可作為獨立服務或包含在 Office 365 品牌方案或套件中)

## <a name="azure-dynamics-365-and-sox"></a>Azure、Dynamics 365 和 SOX

隨著雲端採用的發展勢頭，越來越多的客戶在探索如何遷移應用程式和工作負載，以遵守對雲端的 SOX 合規性義務。 即使雲端服務提供者沒有任何 SOX 憑證或驗證，Azure 仍可協助您符合您的 SOX 義務。

如果您遵守 SOX 合規性義務，您應該檢查 Azure [SOC 1 Type 2 認證](./offering-soc-1.md)，其執行依據如下：

- SSAE 第 18 號，證明標準：釐清與重新編纂，其中包括 AT-C 第 320 節 *與使用者實體對財務報告之內部控制相關的服務組織控制措施檢查報告* (AICPA，專業標準)。
- SOC 1 報告在服務組織中與使用者實體對財務報告之內部控制相關的控制措施檢查 (AICPA 指南)

AICPA SSAE 18 standard 取代 SAS 70，其適用于與財務報告上的使用者實體相關的服務組織中的控制項報告。 這是正式的審計，您可以針對技術服務提供者的協力廠商檢查，針對您在 Azure 上部署的資產進行您自己的行業特定合規性義務。 它包含審計員對控制效能的觀點，以在指定的監控期間達成相關的控制目標。

此外，Azure 已產生 [指導檔](https://azure.microsoft.com/resources/microsoft-azure-guidance-for-sarbanes-oxley-sox/) ，可協助您在解決您自己的 SOX 法規遵從性義務時使用 Azure 的現有相容性報告。 它會在內部 Microsoft 經驗上使用將 SOX 相關應用程式遷移至 Azure。 此外，本指南提供遷移的最佳作法，包括 SOX 合規性影響、兩個公開提供案例研究的評論，以及 Microsoft 內部遷移專案的經驗教訓。

## <a name="office-365-and-sox"></a>Office 365 和 SOX

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | 擴充迴圈、自動替代文字、Azure 資訊保護、二進位轉換服務、預約、Delve 檔專案、編輯器、Exchange Online、表單、[插入線上媒體]、[Insights]、[Kaizala]、[microsoft Analytics]、[microsoft 預約]、[microsoft Graph]、[Microsoft Teams]、[MyAnalytics]、[Office 365 雲端 App 安全性]、Office 365 的影片、Office 365、商務用 OneDrive、Power Apps PowerApps、Power Automate、Power BI PowerPoint  |

### <a name="audits-reports-and-certificates"></a>稽核、報告和認證

[SOC 1 Type 2](offering-SOC.md) 報告：

- Azure 和 Power BI
- Dynamics 365
- Office 365

### <a name="frequently-asked-questions"></a>常見問題集

**如何使用 Microsoft SOX 法規遵從性來協助組織的規範處理常式？**

當您將應用程式和資料移轉至涵蓋的 Microsoft 雲端服務時，您可以建立 Microsoft 所持的 attestations 和認證。 獨立的審計員報告證明 Microsoft 已實現的控制項效能，以協助維護資料的安全性和隱私權。 不過，您完全負責確保您的組織符合所有適用的法律和規定。

### <a name="resources"></a>資源

- [Azure 合規性文件](/azure/compliance/)
- [Azure 可實現合規性世界](https://azure.microsoft.com/resources/azure-enables-a-world-of-compliance/)
- [Microsoft 365 合規性方案](/compliance/regulatory/offering-home)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
- [2002 (SOX 的 Sarbanes-Oxley 法案](https://www.congress.gov/bill/107th-congress/house-bill/3763)) 
- [證券和 Exchange 傭金](https://www.sec.gov/) (秒) 
- [Microsoft 雲端金融服務資源](https://servicetrust.microsoft.com/viewpage/financialservicesoverview)
- [Microsoft 雲端金融服務規範計畫](https://aka.ms/FSCP-Print)
- [雲端計演算法規原則和 Microsoft online services 的合規性地圖](https://servicetrust.microsoft.com/ViewPage/TrustDocuments?command=Download&downloadType=Document&downloadId=5b483567-00b0-4d86-96ae-ee887dadb61c&docTab=6d000410-c9e9-11e7-9a91-892aae8839ad_Compliance_Guides)
- [Microsoft Cloud 中金融機構的風險評估與規範指南](https://azure.microsoft.com/resources/risk-assessment-and-compliance-guide-for-financial-institutions-in-the-microsoft-cloud-/)
- [金融服務行業使用案例](/azure/industry/financial/)
