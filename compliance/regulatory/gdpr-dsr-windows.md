---
title: 適用於 GDPR 和 CCPA 的 Windows 診斷資料處理者設定資料主體要求
description: 了解如何使用 Microsoft 產品、服務及系統管理工具，尋找並處理個人資料以回應 DSR 要求。
keywords: Microsoft 365、Microsoft 365 教育版, Microsoft 365 文件, GDPR
ms.localizationpriority: high
ROBOTS: NOINDEX, NOFOLLOW
ms.prod: microsoft-365-enterprise
ms.topic: article
f1.keywords:
- NOCSH
ms.author: robmazz
author: robmaz
manager: laurawi
ms.reviewer: delinat
audience: itpro
ms.collection:
- GDPR
- M365-security-compliance
- MS-Compliance
hideEdit: true
ms.openlocfilehash: 202b8aa75d3dd6fc94025a1a30f922563fc73e7b
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/12/2021
ms.locfileid: "59158436"
---
# <a name="windows-diagnostic-data-processor-configuration-data-subject-requests-for-the-gdpr-and-ccpa"></a>適用於 GDPR 和 CCPA 的 Windows 診斷資料處理者設定資料主體要求

>[!NOTE]
>本主題適用於 Windows 10 企業版、專業版和教育版 (版本 1809，2021 年 7 月更新及更新版本)。

## <a name="introduction-to-data-subject-requests-dsrs"></a>資料主體要求 (DSR) 簡介

歐盟一般資料保護規定 (GDPR) 賦予人們 (在此法規中稱為 _資料主體_) 權利來管理雇主或其他類型的代理機構或組織 (稱為 _資料控制者_ 或僅稱為 _控制者_) 所收集的個人資料。 依據 GDPR，個人資料的定義很廣泛，舉凡與已識別或可識別自然人相關的任何資料皆屬之。 GDPR 為資料主體提供其個人資料的特定權限；這些權限包括取得個人資料副本、要求對該資料進行更正、限制對該資料的處理、刪除該資料，或是以電子格式接收該資料以移至另一個控制者。 由資料主體向控制者提出以對其個人資料採取行動的正式要求，稱為 _資料主體要求_ 或 DSR。

同樣地，加州消費者隱私法 (CCPA) 為加州消費者提供隱私權和義務，包括與 GDPR 資料主體權利相似的權利，例如，刪除、存取和接收 (可攜性) 其個人資訊的權利。 CCPA 也提供特定揭露、針對選擇行使權時的歧視提供保護，以及特定資料傳輸的「選擇退出/選擇加入」需求分類為「銷售」。 銷售的廣泛定義，包括出於有價值的考量而共用資料。 如需 CCPA 的詳細資訊，請參閱[加州消費者隱私法](/microsoft-365/compliance/offering-ccpa)和[常見問題集](/microsoft-365/compliance/ccpa-faq)。

本指南會討論如何使用 Microsoft 產品、服務及系統管理工具，協助我們的控制者客戶找出並處理個人資料，以回應 DSR。具體來說，這包括如何在啟用 Windows 診斷資料處理者設定時，在 Microsoft 所收集的 Windows 診斷資料中尋找、存取及處理個人資料。以下是本指南中所述程序的快速概觀：

1. **存取**－擷取與資料主體相關聯的 Windows 診斷資料，並在要求時製作可供資料主體使用的副本。
2. **刪除**－永久移除與資料主體相關聯的 Windows 診斷資料。
3. **匯出**—將 Windows 診斷資料的電子副本 (以機器可讀取的格式) 提供給資料主體。

CCPA 中的個人資訊是任何與已識別或可識別個人相關的資訊。 個人的私人、公開或工作角色之間沒有區別。 定義的「個人資訊」一詞大致與 GDPR 下的「個人資料」對應。 不過，CCPA 也包含家庭和家用資料。 如需 CCPA 的詳細資訊，請參閱[加州消費者隱私法](/microsoft-365/compliance/offering-ccpa)和[常見問題集](/microsoft-365/compliance/ccpa-faq)。

本指南的每一章節概述資料控制者組織在啟用 Windows 診斷資料處理者設定時，可針對 Microsoft 所收集的 Windows 診斷資料採取以回應 DSR 的技術程式。

## <a name="terminology"></a>術語

以下清單提供與本指南相關的詞彙定義。

* _控制者_：自然人或法人、公家機關、局處或其他機構，不論單獨或與其他單位聯合，會決定處理個人資料的用途以及方式，其中此類處理的用途以及方式的判斷是根據聯盟與成員國法律，控制者人選或提名控制者的特定準則可由聯盟與成員國法律提供。

* _個人資料和資料主體_：表示與已識別或可識別之自然人 (以下稱為「資料主體」) 相關的任何資訊；可識別的自然人是可以直接或間接識別的人員，尤其是藉由參照如名稱、身分證號碼、位置資料、線上識別碼，或特定於該自然人的身體、生理、基因、心理、經濟、文化或社會身分等一個或多個識別碼來識別。

* _處理者_：代表控制者處理個人資料的自然人或法人、公務機關、局處或其他機構。

* _客戶資料_：由客戶本身或客戶代表，透過企業服務所提供給 Microsoft 的所有資料，包括所有文字、音訊、視訊或影像檔案和軟體。 

* _Windows 診斷資料_：來自 Windows 裝置的技術資料，那些資料和裝置以及 Windows 與相關軟體的執行狀況有關。 它用來讓 Windows 保持最新狀態、安全、可靠、高效能，以及改善產品。 Windows 診斷資料的一些範例是使用的硬體類型、按其各自用途安裝的應用程式以及裝置驅動程式上的可靠性資訊。 某些 Windows 元件及應用程式會直接連線到 Microsoft 服務，但是它們交換的資料並非 Windows 診斷資料。 例如，交換使用者位置以取得當地的天氣或新聞，並不是 Windows 診斷資料的範例。

## <a name="how-to-use-this-guide"></a>如何使用本指南

當您啟用 Windows 診斷資料處理者設定時，您會成為從裝置收集之 Windows 診斷資料的控制者。 如需此設定的詳細資訊，請參閱 [設定貴組織中的 Windows 診斷資料](/windows/privacy/configure-windows-diagnostic-data-in-your-organization)。

## <a name="windows-diagnostic-data"></a>Windows 診斷資料

Microsoft 提供您功能以存取、刪除及匯出與使用者以 Windows 診斷資料處理者設定啟用的裝置相關聯的 Windows 診斷資料。

> [!IMPORTANT]
> 某些 Windows 診斷資料僅與裝置識別碼相關聯，且未與特定使用者相關聯。 此類型的裝置層級資料不會匯出，且在 30 天內會從我們的系統中刪除。<br><br>
> 不支援修正 Windows 診斷資料的功能。 Windows 診斷資料構成了 Windows 中所進行的實際動作，對這類資料的修改會危害動作的歷程記錄，並增加安全性風險並危害可靠性。

下一章節提供如何執行與 Azure Active Directory (AAD) 使用者識別碼相關聯之 Windows 診斷資料的資料主體要求步驟。 如需詳細資訊，請參閱 [Windows 10 & 隱私權合規性：適用於 IT 和合規性專業人員的指南。](/windows/privacy/windows-10-and-privacy-compliance)

## <a name="executing-dsrs-against-windows-diagnostic-data"></a>針對 Windows 診斷資料執行 DSR

Microsoft 透過 Azure 入口網站以及直接透過現有的應用程式開發介面 (API)，提供了存取、刪除及匯出特定 Windows 診斷資料的功能。

### <a name="step-1-access"></a>步驟 1：存取

Microsoft 提供一種方式，讓貴組織中的租用戶系統管理員存取與特定使用者使用以 Windows 診斷資料處理者設定啟用的裝置相關聯之 Windows 診斷資料。針對存取要求所擷取的資料會透過匯出，以機器可讀取的格式提供，並以檔案的形式提供，讓使用者知道與資料相關聯的是哪些裝置與服務。如上所述，所擷取的資料不會包含可能造成 Windows 裝置安全性或穩定性受損的資料。

Azure 入口網站提供企業客戶的租用戶系統管理員管理 DSR 存取要求的功能。 [Azure DSR，第 2 部分，步驟 3：匯出](/microsoft-365/compliance/gdpr-dsr-azure#step-3-export)說明如何透過匯出，在 Azure 入口網站中執行適用於 Windows 診斷資料的 DSR 存取要求。

### <a name="step-2-delete"></a>步驟 2：刪除

Microsoft 提供了一種根據特定使用者的 Azure Active Directory 物件，執行基於使用者的 DSR 刪除要求的方法。

針對以使用者為基礎的刪除要求，Microsoft 提供兩種解決方案。  可提供入口網站體驗，讓企業客戶的租用戶系統管理員有能夠管理 DSR 刪除要求的功能。 [Azure DSR，第 1 部分，步驟 5：刪除](/microsoft-365/compliance/gdpr-dsr-azure#step-5-delete)說明如何透過刪除使用者和相關聯的資料，在 Azure 入口網站中執行適用於 Windows 診斷資料的 DSR 刪除要求。

Microsoft 還能夠透過預先存在的應用程式開發介面 (API) 直接刪除使用者，進而刪除 Windows 診斷資料。 詳細資料請參閱 [API 參考文件](/graph/api/directory-deleteditems-delete)。

>[!IMPORTANT]
>刪除收集的資料並不會停止從裝置的進一步收集。 若要關閉資料收集，請按照 [各自服務的參考文件](/windows/privacy/configure-windows-diagnostic-data-in-your-organization#enterprise-management)中所述的程序。

### <a name="step-3-export"></a>步驟 3：匯出

租用戶系統管理員是貴組織中唯一可以存取與特定使用者使用以 Windows 診斷資料處理者設定啟用的裝置相關聯之 Windows 診斷資料的人員。 針對匯出要求所擷取的資料會以機器可讀取的格式提供；且會以檔案的形式提供，讓使用者知道與資料相關聯的是哪些裝置與服務。 如上所述，所擷取的資料不會包含可能造成 Windows 裝置安全性或穩定性受損的資料。 [Azure DSR，第 2 部分，步驟 3：匯出](/microsoft-365/compliance/gdpr-dsr-azure#step-3-export)說明如何透過 Azure 入口網站執行適用於 Windows 診斷資料的 DSR 匯出要求。

Microsoft 還能夠直接透過預先存在的應用程式開發介面 (API) 匯出 Windows 診斷資料。 詳細資料請參閱 [API 參考文件](/graph/api/user-exportpersonaldata)。

## <a name="notify-us-about-exporting-or-deleting-issues"></a>通知我們有關匯出或刪除的問題

如果您從 Azure 入口網站匯出或刪除 Windows 診斷資料時遇到問題，請前往 Azure 入口網站 **[協助 + 支援]** 刀鋒視窗，並在 **[訂閱管理 > 訂閱的隱私權和法規遵循要求> 隱私權刀鋒視窗和 GDPR 要求]** 下提交新票證。

>[!NOTE]
>最多可能需要 5 天才能完成 Windows 診斷資料匯出要求。 如果您遇到問題，請在開啟支援票證前至少允許 7 天。
