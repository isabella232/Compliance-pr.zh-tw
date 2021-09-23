---
title: NEN 7510
description: 荷蘭組織必須依照 NEN 7510 標準，證明對患者健康狀況資料的控制權。
keywords: Microsoft 365, 合規性, 方案
ms.localizationpriority: high
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
ms.openlocfilehash: b43e882bc23523929a3bbcf7e0c9f667a2ab783f
ms.sourcegitcommit: cb0b058800d3a8f04921066b4c59fb427eb9c268
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2021
ms.locfileid: "59486260"
---
# <a name="nen-7510"></a>NEN 7510

## <a name="nen-7510-overview"></a>NEN 7510 概觀

處理患者健康狀況資訊的荷蘭組織必須證明對該資料及其組織的控制權與在 NEN 7510 標準中設定的需求一致。 Microsoft 本身不受 NEN 7510 的約束，但是醫療保健部門的雲端客戶必須證實他們在基於 Microsoft Cloud 建置的解決方案方面，遵循 NEN 7510。 Microsoft 雲端服務會經歷各種週期性的認證和稽核，其中一部分包含與 NEN 7510 中所指定需求緊密相關的元素。

## <a name="microsoft-and-nen-75102011"></a>Microsoft 和 NEN 7510:2011

Microsoft 已經分析我們目前的認證與保證聲明，並建立 [NEN 7510 涵蓋範圍報告](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=15d5a5fa-fbb6-4ea6-8126-2a2c684ae789&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_GRC_Assessment_Reports) (可在服務信任平台上取得)，這會針對 Microsoft 身為雲端服務提供者而負責的 NEN 7510 控制措施，對應這些認證和保證聲明。 本文件可協助客戶判斷他們必須實作哪些其他控制措施，以確保他們使用 Microsoft 雲端服務儲存或處理的患者健康狀況資訊符合 NEN 7510。

了解如何使用 Azure 安全性與合規性藍圖加快 NEN 7510 部署：[下載 Microsoft Cloud — Azure 和 Office 365 NEN7510-2011 標準涵蓋範圍使用者指南 \(英文\)](https://aka.ms/Azure-NEN7510-2011)

## <a name="microsoft-in-scope-cloud-platforms--services"></a>Microsoft 範圍內雲端平台與服務

- Azure 和 Azure Government
- Intune
- Office 365

## <a name="office-365-and-iso-27001"></a>Office 365 和 ISO 27001

### <a name="office-365-cloud-environments"></a>Office 365 雲端環境

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a>Office 365 適用性和範圍內服務

使用下表判斷 Office 365 服務和訂閱的適用性：

| **適用性** | **範圍內服務** |
|:------------------|:----------------------|
| **商業** | Azure 資訊保護、Bookings、Delve、Exchange Online、Exchange Online Protection、Kaizala、Microsoft Analytics、Microsoft Booking、Microsoft Graph、Microsoft Teams、網頁版 Microsoft To-Do、MyAnalytics、Office 365 雲端 App 安全性、Office 365 群組、商務用 OneDrive、Planner、Power Apps、Power Automate、Power BI for Office 365、PowerApps、SharePoint Online、商務用 Skype、StaffHub、Stream、Sway、Yammer Enterprise |

## <a name="audits-reports-and-certificates"></a>稽核、報告和憑證

- [Azure 和 Office 365 NEN 7510:2011 標準涵蓋範圍](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=15d5a5fa-fbb6-4ea6-8126-2a2c684ae789&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_GRC_Assessment_Reports) \(英文\)

## <a name="frequently-asked-questions"></a>常見問題集

**使用 Microsoft 雲端服務的客戶是否符合 NEN 7510 規範？**

證明 NEN 合規性是醫療保健組織 (「客戶」)的責任。 使用雲端服務廠商時，客戶通常需要廠商的保證，並加入自己的 (其他) 技術和組織決策、選擇和流程。 這會導致客戶對其 NEN 7510 合規性的整體評估，可以將其提交給第三方稽核者以進行檢閱或認證。 NEN 7510 涵蓋範圍報告可深入了解 Microsoft 雲端服務所涵蓋的 NEN 7510 控制措施，但不涵蓋端對端的合規性。

**Microsoft 是否符合 NEN 7510 規範？**

NEN 7510 合規性的責任適用於荷蘭醫療保健組織。 它會要求組織實作資訊安全管理系統，並使用適當的技術和組織措施處理風險。 對於其角色為雲端服務提供者的 Microsoft 而言，NEN 7510 合規性並非目標，在技術上也不可行。 當客戶實作或使用 Microsoft 雲端服務時，這些服務可能處於 NEN 7510 評估範圍內。 不過，組織必須加入屬於整體 NEN 7510 評估一部分的自己的 (其他) 控制措施、選擇和流程。 此報告的目標是證明醫療保健實體可以透過符合 NEN 7510 規範的方式，採用 Microsoft 雲端服務。

**此報告未顯示 100% 的涵蓋範圍。NEN 7510 合規性是否不可行？**

Microsoft 雲端服務提供許多控制措施，可協助荷蘭醫療保健組織符合 NEN 7510 合規性需求。 不過，組織必須以其自身的實作選擇、其他技術控制措施及系統管理程序來補充廠商的保證。 此報告顯示，在適用控制措施的完整清單中已經有超過 94% 的直接涵蓋範圍。 對於其餘的控制措施，Microsoft 會在報告中，針對如何證明這些控制措施的合規性，提供指導方針。

> [!NOTE]
> 實作完整的控制措施清單並非 NEN 7510 的主要用途 (但是 Microsoft Online Services 的大型涵蓋範圍的確可提供協助)。 NEN 7510 會委託實作風險型資訊安全系統，組織可以使用這個系統來判斷適用的控制措施。

**NEN 7510 涵蓋範圍報告是具法律效力的文件嗎？**

否。 這是客戶內部 NEN 7510 保證程序的支援工具，可協助您建立對 NEN 7510 合規性可行的信心和信任。 此報告 (由獨立稽核者 KPMG 所建立) 具備描述性狀態，且包含法律聲明。

**Microsoft 是否支付此報告的費用？**

Microsoft 在其全域保證與 NEN 7510 標準中的控制措施之間建立了對應。 接著，Microsoft 聘請 KPMG (獨立稽核者)，針對控制措施與 NEN 7510 的對應執行獨立審查，從而產生報告。

**我們可以分享這份報告嗎？**

該報告是根據保密協議 (NDA) 提供給您，其依據是該報告僅供客戶參考之用，而且不會透過 Microsoft 服務信任入口網站以外的其他通道加以複製或披露。

客戶可以在他們的合規性或保證流程中，與他們自己的內部或外部稽核者分享報告。

## <a name="resources"></a>資源

- [關於 NEN](https://www.nen.nl/About-NEN.htm)
- [NEN 7510:2011 標準](https://www.nen.nl/NEN-Shop-2/Standard/NEN-75102011-nl.htm)
- [Microsoft 信任中心的合規性](https://www.microsoft.com/trust-center/compliance/compliance-overview)
