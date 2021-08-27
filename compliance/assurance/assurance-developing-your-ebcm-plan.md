---
title: 您的企業商務持續性管理計劃的考量
description: 開發雲端感知商務持續性計劃時需考慮的事項。
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
ms.openlocfilehash: 6a44866d5c82ffa93e6c3c0d9c0ece3946651bd2
ms.sourcegitcommit: 9766d656d0e270f478437bd39c0546ad2e4d846f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/27/2021
ms.locfileid: "58676782"
---
# <a name="developing-your-business-continuity-plan"></a>開發您的業務持續性計畫

本主題提供有關開發業務持續性計畫的指導方針，該計畫會將 Microsoft 365 相依性納入考慮。 我們在這裡建議您分析商務功能及識別有哪些項目依賴 Microsoft 365 服務的方法。 您會在預期有服務失敗且您必須為這些可能性進行準備的情況下，執行這個分析。

一般來說，商務持續性規劃涉及四個層面：評定、規劃、功能驗證以及通訊與協調。

## <a name="assessment"></a>評定
首先，您必須識別貴組織中的商務功能，以及支援它們的服務和程序。 包括完成商務影響分析，其中每個商務功能會根據關鍵程度排名，並您要識別每個商務功能相依的程序和服務。 以下是範例表格，可協助您開始使用自己的評定。

**範例商務影響評定 (BIA)**

這是 `name of the service, system, process, or function` 的 BIA 文件

|BIA 欄位|描述|
|---------|---------|
|BIA 類型|`is it a business process or technology, service or system?`|
|BIA 名稱|`name of the service/system/function/process`|
|服務描述|`give a full description of the service, process, or function`|
|企業功能|`some examples: customer services; legal; marketing; risk management, security, sales, information technology, production, manufacturing`|
|會計年度|`the current fiscal year, re-evaluate these on a regular basis`|
|重要性|`develop your own classifications, but here are some examples: mission critical, important, deferrable`|
|營業單位|`name of the business unit that owns this business function`|
|程序 (服務、功能)|`the name of the process, service, or feature`|
|商務群組高層領導|`the name and contact information of the senior leader of the business group that owns this business process`|
|技術是否已建立 **內部** SLA 或 OLA？|`please explain in as much detail as possible`|
|技術是否已建立 **外部** SLA 或 OLA？|`please explain in as much detail as possible`|
|技術是否有驅動特定程序 SLA 的已知執行規定？ 如果是的話，請詳細說明。|`details here`|
|與此服務相關的資料遺失或損損是否會觸發主要事件？ 如果是的話，請詳細說明。|`details here`|
|服務是否有針對部分或所有關鍵功能的因應措施或替代方案？ 如果是的話，請詳細說明。|`details here`|
|服務是否可處理、儲存或傳輸客戶資料 (例如個人識別資訊 (PII))？ 如果是的話，請詳細說明。|`details here`|
|BIA 狀態|`develop your own status classification, here are some examples: planned, started, in-progress, complete, on-hold, expired`|
|完成日期|`the date this BIA was completed`|
|BIA 講授者|`name of the person or group who is responsible for developing and maintaining this BIA`|
|BIA 核准|`name of the person or group who is the executive sponsor of this BIA and who has responsibility for approving it.`|
|投稿人|`optional list of the people who helped develop this BIA and their contact information`|
|BIA 核准位置|`indicate where the executive approval is located, or attach proof to this document`|

## <a name="planning"></a>規劃

接下來，您要在商務程序之間巡視，以查看是否有任何階層式相依性關聯存在。 根據結果，您優先處理並且形式復原策略，然後再進行支援您策略的標準作業程序。

您可以使用 [Microsoft Service Map](/azure/azure-monitor/insights/service-map) 協助您進行這個對應。 Microsoft Service Map 會自動探索 Windows 和 Linux 系統上的應用程式元件，並且對應所有 TCP 相依性、識別連線和應用程式相依的遠端第三方系統。 它也會將相依性對應至通常是陰暗的網路區域，例如 Active Directory。

以下是您可以作為起點的範例相依性分析 (DA)。 在您的相依性分析 (DA) 中，您會識別及檢查程序相依性。 確定您包括人員、供應商、客戶、合作關係和設施。 此分析的資料將用來識別程序的復原需求與支援相依性的復原功能之間的差距。


|欄位|描述|
|---------|---------|
|程序類型|         |
|講授者|         |
|完成者|         |
|完成日期|         |
|投稿人|         |
  
## <a name="capability-validation"></a>功能驗證

當您清查商務程序，並將關係對應到其他程序和技術之後，您必須為所有程序建置驗證案例。 基本上就是要了解如何驗證您的商務程序持續性計劃。 您可能會發現某些內容更重要，而且您想要優先處理這些問題。
請記得在建立計劃之後，對員工進行事件回應和持續性措施的定期訓練相當重要。 您應該透過納入每個驗證或測試的學習，使用後續事件檢閱來增強復原策略。

![visio 的功能驗證。](../media/capability-validation-visio.png)

## <a name="incident-coordination-and-communication"></a>事件協調與通訊

在服務事件期間，一般通訊通道可能會受到影響或降級，因此您應該預先安排替代選項，在事件期間協助貴組織保持連線。 建立通訊通道、符合安全性和合規性，以及在中斷之前訓練使用者使用，非常重要。 使用者比較樂見從已知狀態到另一個已知狀態的失敗，而不是在危機當中突然出現臨機操作、未知的解決方案。

在 Microsoft，每個服務小組已建立內部備選通訊通道，以協助我們在一般通訊通道無法使用時進行協調。 其中包括備份電話和音訊會議解決方案、Yammer 群組、Teams 群組、內部服務健康狀態儀表板，以及內部事件管理軟體。

在您的業務影響分析和相依性分析期間，您會對應關鍵程序，以及它們相依的技術或服務。 在這個規劃階段期間特別注意通訊，並且思考替代方案。 下列提供一些範例。

- 如果您保持使用者和專案關係人得到通知的主要方法是使用電子郵件，而您的電子郵件服務遭到降級或無法使用，您可以使用其他服務，例如 Microsoft Teams、Yammer 或其他第三方服務作為備援。 關鍵是事先建立這些項目，並且訓練您的使用者要到哪裡使用。 如果沒有人知道它存在，或沒有任何人有加入書簽，則 Yammer 的執行緒不會有用處。  
- 如果您的內部事件管理程序依賴語音通訊來協調您的回應，請建立替代電話語音解決方案，在危機時使用。 此解決方案不需要與您的主要服務有完整的同位，但是應該提供協調您的業務持續性和事件管理小組的最小合作等級。 此外，要求使用者在「全域通訊清單」中發佈他們的行動電話號碼，可以提供多一層的備援通訊，以防萬一。
- 您可能想要建立自訂服務健康狀態儀表板或其他此類網站，可以在事件期間提供狀態更新。 事先訓練使用者要到哪裡取得資訊，可以協助減少與技術支援中心的不必要通話，並且為您的使用者加強信心，這個狀況可以快速有效率地處理。 請使用 O365 服務通訊 API，將此資訊與 Microsoft 365，以取得更高的可見度等級。  
- 讓您的商務程序性計劃和標準作業程序的位置眾所周知相當重要。 我們建議使用如 SharePoint Online 和商務用 OneDrive 的工具，並且設定自動同步到本機裝置，來維護重要文件的線上和離線複本。 若為服務/網路運作中心及其他對復原很重要的類似小組，您可能也想要在緊急狀況事件中保留可用的硬碟副本。

## <a name="know-your-external-points-of-integration"></a>了解您的外部整合點

不論商務模型為何，每家公司都有與客戶、合作夥伴及廠商的整合點。 商務價值供應鏈是建立在與外部實體的整合上。 改善業務連續性以防服務中斷時，需要考慮和保護每個整合點。  
當您分析供應鏈時，應該依照分析內部通訊的相同方式來考量外部通訊。 您的客戶是否依賴您的 Exchange Online 伺服器作為與您聯繫的唯一方法？ 您是否已建立在發生影響運作時間的事件時使用的替代通訊方法，並且讓您的供應商知悉？ 以下是建議如何組織想法的範例表格。

|外部實體名稱|影響事件案例|Microsoft 365 服務整合|替代|
|---------|---------|---------|---------|
|`vendor name`|郵件流程|Exchange Online 是與 Contoso 通訊的唯一方式|設定外部 Microsoft Teams 通道或第三方共同作業軟體          |
|`service supplier name`|聊天|Microsoft Teams|協力廠商立即訊息|
|`partner name`|語音|Microsoft Teams|行動或公用 pstn      |
|`supplier name`|檔案共用|外部共用 SharePoint 網站和 OneDrive|協力廠商檔案共用         |
