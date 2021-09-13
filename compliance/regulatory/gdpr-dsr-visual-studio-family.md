---
title: GDPR 和 CCPA 的 Visual Studio 系列資料主體要求
description: 了解如何使用 Microsoft 工具管理 Visual Studio 中的家族資料主體要求，以符合 GDPR 和 CCPA。
keywords: Visual Studio、Visual Studio Code、Visual Studio for Mac、Visual Studio 文件、隱私權、GDPR、CCPA
ms.localizationpriority: high
audience: itpro
ms.prod: visual-studio-family
ms.topic: article
author: robmazz
f1.keywords:
- NOCSH
ms.author: robmazz
manager: laurawi
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
ms.workload:
- multiple
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-apr2020
hideEdit: true
ms.openlocfilehash: 4a3119ad93c0de5de96e748f7692ba6ddef42c80
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158432"
---
# <a name="visual-studio-family-data-subject-requests-for-the-gdpr-and-ccpa"></a>GDPR 和 CCPA 的 Visual Studio 系列資料主體要求

歐盟 [一般資料保護規定 (GDPR)](https://ec.europa.eu/justice/data-protection/reform/index_en.htm) 賦予人員 (在法規中稱為 _資料主體_) 管理其個人資料的權利。 依據 GDPR，個人資料的定義很廣泛，舉凡與已識別或可識別自然人相關的任何資料皆屬之。 GDPR 為資料主體提供其個人資料的特定權限；這些權限包括取得個人資料副本、要求對該資料進行更正、限制對該資料的處理、刪除該資料，或是以電子格式接收該資料。 資料主體向資料控制者 (控制個人資料的雇主或其他類型的機構或組織) 提出的對該資料主體的個人資料採取行動的正式要求稱為 _資料主體要求_ 或 DSR。

同樣地，加州消費者隱私法 (CCPA) 為加州客戶提供隱私權和義務，包括與 GDPR 資料主體權利相似的權利，例如有權刪除、存取和接收 (可攜性) 其個人資訊。  CCPA 也提供特定揭露、針對選擇行使權時的歧視提供保護，以及特定資料傳輸的「選擇退出/選擇加入」需求分類為「銷售」。 銷售的廣泛定義，包括出於有價值的考量而共用資料。 如需 CCPA 的詳細資訊，請參閱[加州消費者隱私法](offering-ccpa.md)和[常見問題集](ccpa-faq.yml)。

如需關於 GDPR 的一般資訊，請參閱[服務信任入口網站的 GDPR 區段](https://servicetrust.microsoft.com/ViewPage/GDPRGetStarted)。

## <a name="products-covered-by-this-guide"></a>本指南所涵蓋的產品

本文將討論如何使用 Microsoft 工具，將 Visual Studio 和 Visual Studio for Mac 及 Microsoft 對上述兩者與 Visual Studio Code 之擴充功能的驗證 (登入) 工作階段使用期間所收集的個人資料匯出或刪除。本指南也會說明如何針對在使用 Visual Studio 開發人員社群、NuGet.org 和 ASP.NET 網站時所收集的個人資料提出資料主體要求。這些產品可讓您使用非 Microsoft 工具和擴充功能，且 Microsoft 並非這些工具和擴充功能的資料處理者或控制者。使用者必須連絡工具或擴充功能提供者，以了解個人資料與這些工具和擴充功能的集合原則。

## <a name="additional-privacy-information"></a>其他隱私權資訊

產品隨附的 Microsoft 軟體授權條款 ([Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?LinkId=660726)和 [Microsoft 的 GDPR 承諾](/legal/gdpr)) 會描述我們的資料處理做法。

## <a name="visual-studio-visual-studio-for-mac-and-visual-studio-code"></a>Visual Studio、Visual Studio for Mac 和 Visual Studio Code

### <a name="personal-data-we-collect"></a>我們收集的個人資料

Microsoft 身為 GDPR 底下的資料處理者，會向我們要提供體驗的使用者收集所需資料，藉以改善 Visual Studio 和 Visual Studio for Mac，以及 Microsoft 對此上述兩種軟體和對 Visual Studio Code 的擴充功能。資料有兩種類別：客戶資料以及系統所產生的記錄。客戶資料包含這些產品執行其所提供服務所需的使用者識別交易和互動資料。例如，若要為使用者提供個人化體驗 (例如漫遊設定)，我們必須收集使用者帳戶資訊和設定資料。系統所產生的記錄是用來協助您找出問題並針對問題進行疑難排解的使用狀況或診斷資料，從而改善我們的產品和服務，並也可能包含關於使用者的識別資訊 (例如使用者名稱)。系統所產生記錄的保留時間不會超過 18 個月。例如，系統所產生的記錄會針對每一天的產品使用情形進行彙總，並且會包含使用日期、所使用的產品 (例如，"Visual Studio 2017")、您所採取的動作 (例如，"vs/core/packagecostsummary/solutionload")，以及採取動作的次數，如本範例中所示：

```Log
{Time":"2/23/2018 12:00:00 AM","AppName":"Visual Studio 2017","Action":"vs/core/packagecostsummary/solutionload","Target":"1 times",
"DevicePlatform":"Windows 10 Enterprise","IP":null,"InputMethod":null,
"SearchTerm":null,"SearchResult":null}

{Time":"2/23/2018 12:00:00 AM","AppName":"Visual Studio 2017","Action":"vs/ide/connected/accountmanagement/account","Target":"1 times",
"DevicePlatform": "Windows 10 Enterprise","IP":null,"InputMethod":null,
"SearchTerm":null,"SearchResult":null}

{"Time":"2/27/2018 12:00:00 AM","AppName":"Visual Studio 2017","Action":"vs/core/perf/satellitepagefileusage","Target":"23 times",
"DevicePlatform":"Windows 10 Enterprise","IP":null,"InputMethod":null,
"SearchTerm":null,"SearchResult":null}
```

如需詳細資訊，請參閱 [Visual Studio 所收集的系統所產生記錄](/visualstudio/ide/diagnostic-data-collection)。

DSR 僅針對附加到已驗證身分識別的個人資料提供服務。例如，Visual Studio Code 不支援登入，因此不會將其中的系統所產生記錄附加至已驗證的身分識別，且無法獲得服務。不過，Visual Studio Code 的某些 Microsoft 擴充功能可能會提供驗證的資料，而 DSR 可為此資料提供服務。如需詳細資訊，請參閱[ GDPR 與 Visual Studio Code](https://code.visualstudio.com/docs/supporting/faq#_gdpr-and-vs-code)。一般而言，我們不會儲存 Visual Studio 2013 及較舊版本的資料；不過，某些擴充功能和元件可能會提供附加到已驗證身分識別的資料，而 DSR 可以為其提供服務，如下所示。

### <a name="how-users-can-control-personal-data"></a>使用者如何控制個人資料

Visual Studio 2015 及更新版本、Visual Studio for Mac 和 Visual Studio Code 可提供下列方法，讓您的使用者停止資料收集，並讓您以控制者身分將已收集到的資料匯出或刪除。

#### <a name="in-app-settings"></a>應用程式內設定

使用者可以控制這些產品的隱私權設定。如需詳細資訊，請參閱下列內容

- [如何管理 Visual Studio 中的隱私權設定](/visualstudio/ide/visual-studio-experience-improvement-program)。
- [如何管理 Visual Studio for Mac 中的隱私權設定](/visualstudio/mac/visual-studio-experience-improvement-program)。
- [如何停用 Visual Studio Code 中的遙測報告](https://code.visualstudio.com/docs/supporting/faq#_how-to-disable-telemetry-reporting)。

#### <a name="exporting-or-deleting-data"></a>匯出或刪除資料

控制者可以透過兩種方法之一 (取決於他們 Visual Studio 系列產品或 Microsoft 擴充功能的註冊方式)，來管理從其資料主體收集到的客戶資料和系統所產生記錄。在某些情況下，必須同時使用這兩種方法。這兩種方法都可讓控制者下載一份受該方法管理的活動歷程記錄。關閉 AAD 或 MSA 帳戶會刪除相關聯的 Visual Studio 客戶資料，並將與這些產品相關的系統所產生記錄中的個人識別資料進行匿名。已匿名之系統所產生記錄的保留時間不會超過 18 個月。

- 使用 Azure 租用戶所支援帳戶例如，與 Azure 訂閱相關聯的 AAD 帳戶或 MSA 帳戶註冊 Visual Studio 系列產品的使用者可遵循 [GDPR 的 Azure 資料主體要求](gdpr-dsr-azure.md)中的指示。
- 未使用 Azure 租用戶所支援帳戶例如，許多使用 Microsoft 帳戶 (MSA) 的帳戶註冊 Visual Studio 系列產品的使用者，可使用透過其 Microsoft 帳戶提供的[ Web 式 Microsoft 隱私權回應中心](https://aka.ms/userprivacysite)來檢視、控制及刪除繫結至其多項 Microsoft 服務中 Microsoft 帳戶的活動資料。 在此案例中，使用者是自己個人資料的控制者。

> [!NOTE]
> 當 MSA 帳戶擁有者刪除其帳戶時，所有與這些產品相關的個人識別資料都會加以刪除 (無論帳戶是否受 Azure 租用戶所支援)，且會將系統產生的記錄加以匿名。

針對 Visual Studio 2013，我們所收集的資料會加以匿名。針對 Visual Studio 2012 與先前版本，我們在收到資料後會立即加以刪除。在這兩種情況下，稍後沒有任何內容可供檢視、匯出或刪除。

## <a name="visual-studio-developer-community"></a>Visual Studio 開發人員社群

我們透過[開發人員社群](https://developercommunity.visualstudio.com)網站支援[一般資料保護規定 (GDPR)](https://ec.europa.eu/justice/data-protection/reform/index_en.htm) 要求。您可以檢視、匯出或刪除您的意見反應資料。

### <a name="personal-data-we-collect"></a>我們收集的個人資料

Microsoft 會收集資料，以協助我們重現您使用 Visual Studio 系列產品回報的問題，並針對問題進行疑難排解。這項資料包含個人資料和公開意見反應。個人資料包括：

- 您的[開發人員社群](https://developercommunity.visualstudio.com)設定檔資訊；
- 喜好設定和通知；
- 您透過[在 Visual Studio 中回報的問題](/visualstudio/ide/how-to-report-a-problem-with-visual-studio-2017)或透過[開發人員社群](https://developercommunity.visualstudio.com)提供的附件和系統所產生記錄；
- 您的投票。

公開意見反應包含：回報的問題、註解和解決方案。

### <a name="how-users-can-control-personal-data"></a>使用者如何控制個人資料

#### <a name="view"></a>檢視

若要檢視與您意見反應相關的資料，請遵循下列步驟：

1. 登入[開發人員社群](https://developercommunity.visualstudio.com)。 從右上角按一下您的設定檔，然後選取 [設定檔和喜好設定]。
2. 按一下任一個 [設定檔]、[通知]、[活動] 和 [附件] 索引標籤來檢視提交至意見反應系統的資料。
   1. [設定檔] 是指您的[開發人員社群](https://developercommunity.visualstudio.com)設定檔，其中包含使用者名稱、電子郵件地址、關於等等。
   2. **通知是控制您接收電子郵件通知的方式。
   3. [活動] 會提供您已在使用中項目 (已張貼、已註解等) 和已執行活動的意見反應。
   4. [附件] 是您附件歷程記錄的清單，格式如 `FileName was attached to the problem "ProblemName" Tue, Apr 10, 18 2:27 PM`。

#### <a name="export"></a>匯出

您可以將您的意見反應資料匯出作為 DSR 的一部分。我們將會建立一個或多個 .zip 封存檔，當中包含：

- 您的[開發人員社群](https://developercommunity.visualstudio.com)設定檔資訊；
- 喜好設定和通知設定；
- 您透過[在 Visual Studio 中回報的問題](/visualstudio/ide/how-to-report-a-problem-with-visual-studio-2017)或透過[開發人員社群](https://developercommunity.visualstudio.com)提供的附件。

> [!NOTE]
> 我們會將您從封存檔中提供的下列公開意見反應排除：註解、解決方案、回報的問題。

若要開始匯出，請遵循下列步驟：

1. 登入[開發人員社群](https://developercommunity.visualstudio.com)。 從右上角按一下您的設定檔，然後選取 [設定檔和喜好設定]。
2. 按一下 [隱私權] 索引標籤，然後按一下 [建立封存] 以要求匯出您的資料。
3. [封存狀態] 將會更新，以顯示我們正在準備資料。資料可供使用之前的時間長度會依據我們所需匯出的資料量而定。
4. 一旦資料就緒之後，我們會傳送電子郵件給您。
5. 按一下電子郵件中的 [下載封存]，或回到 [隱私權] 索引標籤來下載您的資料。

> [!NOTE]
> - 如果您在 [通知] 索引標籤中選擇不要收到通知，我們就不會傳送電子郵件。
> - 如果您再次要求匯出，我們就會移除您的舊封存，並建立新的封存。

#### <a name="delete"></a>刪除

刪除將會從[開發人員社群](https://developercommunity.visualstudio.com)中移除下列關於您的資訊

- 設定檔資訊；
- 喜好設定和通知設定；
- 您透過[在 Visual Studio 中回報的問題](/visualstudio/ide/how-to-report-a-problem-with-visual-studio-2017)或透過[開發人員社群](https://developercommunity.visualstudio.com)提供的附件。
- 您的投票

> [!NOTE]
> 我們將不會刪除下列公開資訊，但會加以匿名：您的註解、解決方案、您所回報的問題。
>
> [!IMPORTANT]
> 刪除 AAD 或 MSA 帳戶會觸發[開發人員社群](https://developercommunity.visualstudio.com)的 [刪除] 程序。

若要開始 [刪除]，請遵循下列步驟：

1. 登入[開發人員社群](https://developercommunity.visualstudio.com)。 從右上角按一下您的設定檔，然後選取 [設定檔和喜好設定]。
2. 按一下 [隱私權] 索引標籤，然後按一下 [刪除資料與帳戶] 以開始刪除資料。
3. [確認] 畫面隨即出現。
4. 在方塊中輸入「刪除」，然後按一下 [刪除我的帳戶]。

當您按一下 [刪除帳戶]：

- 我們會將您登出。
- 我們將會刪除您的[開發人員社群](https://developercommunity.visualstudio.com)帳戶、您的個人資料和附件。
- 我們會將您的公開意見反應匿名。您的公開意見反應將仍在開發人員社群中顯示，且會指示為以匿名使用者回報。
- 我們在刪除您的帳戶之後，就不會傳送電子郵件給您，因為您將不再顯示於系統中。
- 如果您報告新的問題或登入[開發人員社群](https://developercommunity.visualstudio.com)，則系統會將您視為新的使用者。
- 如果您從[開發人員社群](https://developercommunity.visualstudio.com)中刪除您的帳戶，我們並不會將它從其他 Microsoft 服務中刪除。

## <a name="xamarin-forums"></a>Xamarin 論壇

### <a name="personal-data-we-collect"></a>我們收集的個人資料

透過 [Xamarin 論壇](https://forums.xamarin.com/)使用者社群，Microsoft 會收集您提供的資料，協助我們重現您在使用 Microsoft 產品和服務時遇到的問題並進行疑難排解。 這些資料包括個人資料和公開意見反應。 我們收集的個人資料是使用者帳戶資料 (例如，與您的 Xamarin 論壇相關聯的使用者名稱和電子郵件地址)，我們收集的公開意見反應包括您透過 Xamarin 論壇提供的錯誤、問題、註解和解決方案。

### <a name="how-you-can-control-your-data"></a>您可以控制資料的方式

#### <a name="xamarin-forums"></a>Xamarin 論壇

##### <a name="view"></a>檢視

具有有效 Xamarin 論壇帳戶的使用者可以在 Xamarin 論壇帳戶頁面中檢視其個人資料和公開意見反應 (例如，所有已張貼的對話和文章)。使用者也會透過其帳戶頁面編輯其個人資料。

##### <a name="export"></a>匯出

Xamarin 論壇是由第三方 Vanilla 論壇託管。如需要求匯出您的公開資料，使用者需連絡 forums@xamarin.com (受 Xamarin 小組監視)。接著，我們會直接與 Vanilla 論壇合作來處理此要求。

##### <a name="delete"></a>刪除

Xamarin 論壇是由第三方 Vanilla 論壇託管。如需要求刪除您的個人及公開資料，使用者需連絡 forums@xamarin.com (受 Xamarin 小組監視)。接著，我們會手動處理使用者的個人資料刪除要求。

> [!NOTE]
> Xamarin 的 Bugzilla 不再接受新問題。 前一版的 Xamarin Bugzilla 帳戶擁有者可以在下列網址檢視他們報告之所有錯誤以及新增至錯誤之所有註解的封存於 [https://xamarin.github.io/bugzilla-archives/](https://xamarin.github.io/bugzilla-archives/)。 若要要求刪除封存中所包含的個人資料，使用者可以在 [https://github.com/xamarin/bugzilla-archives/issues/new/choose](https://github.com/xamarin/bugzilla-archives/issues/new/choose) 進行歸檔和發布。 使用者張貼到 Xamarin Bugzilla 的公開意見反應 (例如錯誤、問題、註解和解決方案) 在收到刪除要求後不會被刪除。 透過移除與提交刪除要求的使用者建立之任何公開意見反應相關聯的名稱和電子郵件地址，將匿名公開意見反應。

## <a name="nuget"></a>NuGet

如需 NuGet.org 的 DSR 相關詳細資訊，請參閱 [NuGet 使用者資料要求](/nuget/policies/data-requests)。

## <a name="aspnet"></a>ASP.NET

如需 ASP.NET 網站的 DSR 相關資訊，請參閱 [ASP.NET 網站和 GDPR 資料主體要求處理](https://www.asp.net/gdpr)。

## <a name="iisnet"></a>IIS.NET

如需 IIS.NET 網站的 DSR 相關資訊，請參閱 [IIS.NET 網站和 GDPR 資料主體要求處理](https://www.iis.net/gdpr)。

## <a name="other-visual-studio-family-services"></a>其他 Visual Studio 系列服務

### <a name="survey-monkey"></a>Survey Monkey

我們會不時邀請客戶透過 Survey Monkey 提供這些產品的意見反應。 此資料在 28 天內從 Survey Monkey 中刪除。 Microsoft 得在內部保留此資料最多 18 個月。 如果問卷回應已通過驗證，則我們會在服務這些產品的資料主體要求時，將它們納入匯出和刪除資料主體要求中。

## <a name="learn-more"></a>深入了解

- [Microsoft 對公開發行企業軟體產品客戶的 GDPR 承諾](/legal/gdpr)
- [Microsoft 信任中心](https://www.microsoft.com/trust-center/privacy/gdpr-overview)
- [服務信任入口網站](https://servicetrust.microsoft.com/ViewPage/GDPRGetStarted)
- [Microsoft 隱私權儀表板](https://account.microsoft.com/privacy)
- [Microsoft 隱私權回應中心](https://aka.ms/userprivacysite)
- [GDPR 的 Azure 資料主體要求](gdpr-dsr-azure.md)
