---
title: " (CJIS) 安全性原則的刑事審判資訊服務"
description: Microsoft 政府雲端服務遵循美國刑事審判資訊服務安全性原則。
keywords: Microsoft 365、合規性、方案
localization_priority: None
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
ms.openlocfilehash: 896202ea1f51d88d1871a2c7ff81f4ee1e620d17
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385363"
---
# <a name="criminal-justice-information-services-cjis-security-policy"></a><span data-ttu-id="6f037-104"> (CJIS) 安全性原則的刑事審判資訊服務</span><span class="sxs-lookup"><span data-stu-id="6f037-104">Criminal Justice Information Services (CJIS) Security Policy</span></span>

## <a name="cjis-overview"></a><span data-ttu-id="6f037-105">CJIS 概述</span><span class="sxs-lookup"><span data-stu-id="6f037-105">CJIS overview</span></span>

<span data-ttu-id="6f037-106">刑事司法 Information Services (CJIS 美國聯邦局調查 () FBI 的) 分公司，提供州、地方及聯邦法律強制執行與刑事審判機關的存取權司法司法資訊 (CJI) （例如，指紋記錄及刑事記錄）。</span><span class="sxs-lookup"><span data-stu-id="6f037-106">The Criminal Justice Information Services (CJIS) Division of the US Federal Bureau of Investigation (FBI) gives state, local, and federal law enforcement and criminal justice agencies access to criminal justice information (CJI) — for example, fingerprint records and criminal histories.</span></span> <span data-ttu-id="6f037-107">美國的法律強制執行和其他政府代理商必須確定其使用雲端服務以進行 CJI 的傳輸、儲存或處理，遵循 [CJIS 安全性原則](https://aka.ms/cjis-security-policy)，它會建立最低的安全性需求和控制，以保護 CJI。</span><span class="sxs-lookup"><span data-stu-id="6f037-107">Law enforcement and other government agencies in the United States must ensure that their use of cloud services for the transmission, storage, or processing of CJI complies with the [CJIS Security Policy](https://aka.ms/cjis-security-policy), which establishes minimum security requirements and controls to safeguard CJI.</span></span>

<span data-ttu-id="6f037-108">CJIS 安全性原則會整合總統和 FBI 指令、聯邦法律和刑事審判社區的諮詢原則董事會決策，以及國家安全局)  (NIST 的指導方針。</span><span class="sxs-lookup"><span data-stu-id="6f037-108">The CJIS Security Policy integrates presidential and FBI directives, federal laws, and the criminal justice community's Advisory Policy Board decisions, along with guidance from the National Institute of Standards and Technology (NIST).</span></span> <span data-ttu-id="6f037-109">原則會定期更新，以反映不斷演變的安全性需求。</span><span class="sxs-lookup"><span data-stu-id="6f037-109">The Policy is periodically updated to reflect evolving security requirements.</span></span>

<span data-ttu-id="6f037-110">CJIS 安全性原則定義13個私人承包商（如雲端服務提供者）必須評估，以判斷其使用雲端服務是否可與 CJIS 需求一致。</span><span class="sxs-lookup"><span data-stu-id="6f037-110">The CJIS Security Policy defines 13 areas that private contractors such as cloud service providers must evaluate to determine if their use of cloud services can be consistent with CJIS requirements.</span></span> <span data-ttu-id="6f037-111">這些區域會嚴格對應 NIST 800-53，也就是 [聯邦風險和授權管理計畫的基礎 (FedRAMP) ](offering-FedRAMP.md)，這是 Microsoft 已針對其政府雲端服務認證的程式。</span><span class="sxs-lookup"><span data-stu-id="6f037-111">These areas correspond closely to NIST 800-53, which is also the basis for the [Federal Risk and Authorization Management Program (FedRAMP)](offering-FedRAMP.md), a program under which Microsoft has been certified for its Government Cloud offerings.</span></span>

<span data-ttu-id="6f037-112">此外，處理 CJI 的所有私人承包商必須簽署 CJIS 安全性附錄，這是由美國律師一般核准的統一合約，可協助確保安全性原則所需的安全性和機密性。</span><span class="sxs-lookup"><span data-stu-id="6f037-112">In addition, all private contractors who process CJI must sign the CJIS Security Addendum, a uniform agreement approved by the US Attorney General that helps ensure the security and confidentiality of CJI required by the Security Policy.</span></span> <span data-ttu-id="6f037-113">它也會承諾承包商維護安全計畫與聯邦和州法律、法規和標準的一致性，並限制 CJI 使用，以供政府代理商使用的目的。</span><span class="sxs-lookup"><span data-stu-id="6f037-113">It also commits the contractor to maintaining a security program consistent with federal and state laws, regulations, and standards, and limits the use of CJI to the purposes for which a government agency provided it.</span></span>

## <a name="microsoft-and-cjis-security-policy"></a><span data-ttu-id="6f037-114">Microsoft 和 CJIS 安全性原則</span><span class="sxs-lookup"><span data-stu-id="6f037-114">Microsoft and CJIS Security Policy</span></span>

<span data-ttu-id="6f037-115">Microsoft 會以含 CJIS 資訊協定的狀態，簽署 CJIS 安全性附錄。</span><span class="sxs-lookup"><span data-stu-id="6f037-115">Microsoft signs the CJIS Security Addendum in states with CJIS Information Agreements.</span></span> <span data-ttu-id="6f037-116">這些指示州法律強制執行機構負責遵循 CJIS 安全性原則 Microsoft 的雲端安全性控制措施可協助保護整個資料生命週期，並確保適當的後臺篩選工作人員，以存取 CJI。</span><span class="sxs-lookup"><span data-stu-id="6f037-116">These tell state law enforcement authorities responsible for compliance with CJIS Security Policy how Microsoft's cloud security controls help protect the full lifecycle of data and ensure appropriate background screening of operating personnel with access to CJI.</span></span> <span data-ttu-id="6f037-117">Microsoft 繼續與州政府合作，以輸入 CJIS 資訊協定。</span><span class="sxs-lookup"><span data-stu-id="6f037-117">Microsoft continues to work with state governments to enter into CJIS Information Agreements.</span></span>

<span data-ttu-id="6f037-118">Microsoft 已評估 Microsoft Azure 政府、Microsoft Office 365 美國政府和 Microsoft Dynamics 365 美國政府的運作原則和程式，並將證明其在適當服務合約中的能力，以符合使用內部範圍內服務的 FBI 需求。</span><span class="sxs-lookup"><span data-stu-id="6f037-118">Microsoft has assessed the operational policies and procedures of Microsoft Azure Government, Microsoft Office 365 U.S. Government, and Microsoft Dynamics 365 U.S. Government, and will attest to their ability in the applicable services agreements to meet FBI requirements for the use of in-scope services.</span></span>

<span data-ttu-id="6f037-119">深入瞭解 Microsoft Cloud 上的 CJIS 安全性原則的優點： [閱讀 Genetec 如何清除刑事調查](https://customers.microsoft.com/story/genetec)</span><span class="sxs-lookup"><span data-stu-id="6f037-119">Learn about the benefits of CJIS Security policy on the Microsoft Cloud: [Read how Genetec cleared criminal investigations](https://customers.microsoft.com/story/genetec)</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="6f037-120">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="6f037-120">Microsoft in-scope cloud platforms & services</span></span>

- <span data-ttu-id="6f037-121">Azure 政府</span><span class="sxs-lookup"><span data-stu-id="6f037-121">Azure Government</span></span>
- <span data-ttu-id="6f037-122">美國政府的 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6f037-122">Dynamics 365 U.S. Government</span></span>
- <span data-ttu-id="6f037-123">Office 365美國政府</span><span class="sxs-lookup"><span data-stu-id="6f037-123">Office 365 U.S. Government</span></span>
- <span data-ttu-id="6f037-124">Power BI 雲端服務可作為獨立服務或包含在 Office 365 品牌方案或套件中</span><span class="sxs-lookup"><span data-stu-id="6f037-124">Power BI cloud service either as a standalone service or as included in an Office 365 branded plan or suite</span></span>

## <a name="azure-dynamics-365-and-cjis"></a><span data-ttu-id="6f037-125">Azure、Dynamics 365 和 CJIS</span><span class="sxs-lookup"><span data-stu-id="6f037-125">Azure, Dynamics 365, and CJIS</span></span>

<span data-ttu-id="6f037-126">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE CJIS 服務](/azure/compliance/offerings/offering-cjis)。</span><span class="sxs-lookup"><span data-stu-id="6f037-126">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure CJIS offering](/azure/compliance/offerings/offering-cjis).</span></span>

## <a name="office-365-and-cjis"></a><span data-ttu-id="6f037-127">Office 365 和 CJIS</span><span class="sxs-lookup"><span data-stu-id="6f037-127">Office 365 and CJIS</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="6f037-128">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="6f037-128">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="6f037-129">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="6f037-129">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="6f037-130">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="6f037-130">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="6f037-131">**適用性**</span><span class="sxs-lookup"><span data-stu-id="6f037-131">**Applicability**</span></span> | <span data-ttu-id="6f037-132">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="6f037-132">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="6f037-133">**GCC**</span><span class="sxs-lookup"><span data-stu-id="6f037-133">**GCC**</span></span> | <span data-ttu-id="6f037-134">Azure Active Directory，合規性管理員，Delve，Exchange Online，表單，Microsoft Defender for Office 365，Microsoft Teams，MyAnalytics，Office 365 進階合規性附加元件，Office 365 安全性 & 規範中心，Office 線上，Office Pro，商務用 OneDrive，PowerApps 線上，Power Automate，Power BI</span><span class="sxs-lookup"><span data-stu-id="6f037-134">Azure Active Directory, Compliance Manager, Delve, Exchange Online, Forms, Microsoft Defender for Office 365, Microsoft Teams, MyAnalytics, Office 365 Advanced Compliance add-on, Office 365 Security & Compliance Center, Office Online, Office Pro Plus, OneDrive for Business, Planner, PowerApps, Power Automate, Power BI, SharePoint Online, Skype for Business, Stream</span></span> |

### <a name="office-365-audits-reports-and-certificates"></a><span data-ttu-id="6f037-135">Office 365 審核、報告和憑證</span><span class="sxs-lookup"><span data-stu-id="6f037-135">Office 365 audits, reports, and certificates</span></span>

<span data-ttu-id="6f037-136">FBI 不會提供符合 CJIS 需求的 Microsoft 認證。</span><span class="sxs-lookup"><span data-stu-id="6f037-136">The FBI does not offer certification of Microsoft compliance with CJIS requirements.</span></span> <span data-ttu-id="6f037-137">相反地，microsoft 證明包含在 Microsoft 和州的 CJIS 機關，以及 Microsoft 及其客戶之間的協定中。</span><span class="sxs-lookup"><span data-stu-id="6f037-137">Instead, a Microsoft attestation is included in agreements between Microsoft and a state's CJIS authority, and between Microsoft and its customers.</span></span>

[<span data-ttu-id="6f037-138">Microsoft CJIS 雲端需求</span><span class="sxs-lookup"><span data-stu-id="6f037-138">Microsoft CJIS Cloud Requirements</span></span>](https://aka.ms/MicrosoftCJISCloudRequirements)

### <a name="cjis-status-in-the-united-states-current-as-of-1152020"></a><span data-ttu-id="6f037-139">美國 (目前為11/5/2020 的州的 CJIS 狀態) </span><span class="sxs-lookup"><span data-stu-id="6f037-139">CJIS status in the United States (current as of 11/5/2020)</span></span>

<span data-ttu-id="6f037-140">45州和哥倫比亞含管理合約的地區，在綠色地圖上以綠色反白顯示：</span><span class="sxs-lookup"><span data-stu-id="6f037-140">45 states and the District of Columbia with management agreements, highlighted on the map in green include:</span></span>

<span data-ttu-id="6f037-141">Alabama，阿拉斯加，亞利桑那，Arkansas，加州，科羅拉多，Connecticut，佛羅里達，格魯吉亞，夏威夷，Idaho，Illinois，印地安那州 Iowa、Kansas、Kentucky、Maine、麻塞諸塞、密歇根、Minnesota、Mississippi、Missouri、Montana、Nebraska、Nevada、New Hampshire、New Jersey、New 墨西哥、紐約、北卡羅萊納州、北 Dakota、Oklahoma、德克薩斯、猶他州、Rhode、南部卡羅萊納州、華盛頓、德克薩斯、Tennessee、Vermont、Wisconsin、、</span><span class="sxs-lookup"><span data-stu-id="6f037-141">Alabama, Alaska, Arizona, Arkansas, California, Colorado, Connecticut, Florida, Georgia, Hawaii, Idaho, Illinois, Indiana, Iowa, Kansas, Kentucky, Maine, Massachusetts, Michigan, Minnesota, Mississippi, Missouri, Montana, Nebraska, Nevada, New Hampshire, New Jersey, New Mexico, New York, North Carolina, North Dakota, Oklahoma, Oregon, Pennsylvania, Rhode Island, South Carolina, Tennessee, Texas, Utah, Vermont, Virginia, Washington, West Virginia, Wisconsin, and the District of Columbia.</span></span>

<span data-ttu-id="6f037-142">Microsoft 致力於會議適用的 CJIS 管制控制措施，允許刑事審判組織執行雲端式方案，並遵循 CJIS 安全性原則5.9。</span><span class="sxs-lookup"><span data-stu-id="6f037-142">Microsoft's commitment to meeting the applicable CJIS regulatory controls allows Criminal Justice organizations to implement cloud-based solutions and be compliant with CJIS Security Policy V5.9.</span></span>

### <a name="frequently-asked-questions"></a><span data-ttu-id="6f037-143">常見問題集</span><span class="sxs-lookup"><span data-stu-id="6f037-143">Frequently asked questions</span></span>

<span data-ttu-id="6f037-144">**我可以在哪裡要求規範資訊？**</span><span class="sxs-lookup"><span data-stu-id="6f037-144">**Where can I request compliance information?**</span></span>

<span data-ttu-id="6f037-145">請與您的 Microsoft 帳戶代表聯繫，以取得您感興趣之司法轄區的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="6f037-145">Contact your Microsoft account representative for information on the jurisdiction you are interested in.</span></span> <span data-ttu-id="6f037-146">相關 <cjis@microsoft.com> 資訊，以取得目前可用服務的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="6f037-146">Contact <cjis@microsoft.com> for information on which services are currently available in which states.</span></span>

<span data-ttu-id="6f037-147">**Microsoft 如何示範其雲端服務是否可以符合我的狀態需求？**</span><span class="sxs-lookup"><span data-stu-id="6f037-147">**How does Microsoft demonstrate that its cloud services enable compliance with my state's requirements?**</span></span>

<span data-ttu-id="6f037-148">Microsoft 會以州 CJIS 系統代理商 (CSA) 來簽署資訊協定;您可以從您的狀態 CSA 索取副本。</span><span class="sxs-lookup"><span data-stu-id="6f037-148">Microsoft signs an Information Agreement with a state CJIS Systems Agency (CSA); you may request a copy from your state's CSA.</span></span> <span data-ttu-id="6f037-149">此外，Microsoft 還提供客戶深入的安全性、隱私權和規範資訊。</span><span class="sxs-lookup"><span data-stu-id="6f037-149">In addition, Microsoft provides customers with in-depth security, privacy, and compliance information.</span></span> <span data-ttu-id="6f037-150">客戶也可以查看獨立審計員所準備的安全性和符合性報告，讓他們能夠驗證 Microsoft 是否已實現安全性控制 (例如 ISO 27001) 適當于相關的審計範圍。</span><span class="sxs-lookup"><span data-stu-id="6f037-150">Customers may also review security and compliance reports prepared by independent auditors so they can validate that Microsoft has implemented security controls (such as ISO 27001) appropriate to the relevant audit scope.</span></span>

<span data-ttu-id="6f037-151">**從何處開始，我的代理人的合規性**</span><span class="sxs-lookup"><span data-stu-id="6f037-151">**Where do I start with my agency's compliance effort?**</span></span>

<span data-ttu-id="6f037-152">[CJIS 安全性原則](https://aka.ms/cjis-security-policy) 涵蓋您的代理人保護 CJI 所必須採取的防範措施。</span><span class="sxs-lookup"><span data-stu-id="6f037-152">[CJIS Security Policy](https://aka.ms/cjis-security-policy) covers the precautions that your agency must take to protect CJI.</span></span> <span data-ttu-id="6f037-153">此外，您的 Microsoft 帳戶代表可讓您與熟悉司法需求的人員保持聯繫</span><span class="sxs-lookup"><span data-stu-id="6f037-153">In addition, your Microsoft account representative can put you in touch with those familiar with the requirements of your jurisdiction</span></span>

### <a name="use-microsoft-compliance-manager-to-assess-your-risk"></a><span data-ttu-id="6f037-154">使用 Microsoft 合規性管理員來評估風險</span><span class="sxs-lookup"><span data-stu-id="6f037-154">Use Microsoft Compliance Manager to assess your risk</span></span>

<span data-ttu-id="6f037-155">[Microsoft 合規性管理員](/microsoft-365/compliance/compliance-manager)是 [Microsoft 365 合規性中心](/microsoft-365/compliance/microsoft-365-compliance-center)的功能，可協助您了解組織的合規性狀況，並採取行動以協助降低風險。</span><span class="sxs-lookup"><span data-stu-id="6f037-155">[Microsoft Compliance Manager](/microsoft-365/compliance/compliance-manager) is a feature in the [Microsoft 365 compliance center](/microsoft-365/compliance/microsoft-365-compliance-center) to help you understand your organization's compliance posture and take actions to help reduce risks.</span></span> <span data-ttu-id="6f037-156">合規性管理員會提供特優範本以為此法規建立評定。</span><span class="sxs-lookup"><span data-stu-id="6f037-156">Compliance Manager offers a premium template for building an assessment for this regulation.</span></span> <span data-ttu-id="6f037-157">可在合規性管理員的 [評定範本] 頁面尋找範本。</span><span class="sxs-lookup"><span data-stu-id="6f037-157">Find the template in the **assessment templates** page in Compliance Manager.</span></span> <span data-ttu-id="6f037-158">瞭解如何[在合規性管理員中建立評估](/microsoft-365/compliance/compliance-manager-assessments)。</span><span class="sxs-lookup"><span data-stu-id="6f037-158">Learn how to [build assessments in Compliance Manager](/microsoft-365/compliance/compliance-manager-assessments).</span></span>

### <a name="resources"></a><span data-ttu-id="6f037-159">資源</span><span class="sxs-lookup"><span data-stu-id="6f037-159">Resources</span></span>

- [<span data-ttu-id="6f037-160">刑事審判資訊服務</span><span class="sxs-lookup"><span data-stu-id="6f037-160">Criminal Justice Information Services</span></span>](https://aka.ms/cjis)
- [<span data-ttu-id="6f037-161">CJIS 安全性原則</span><span class="sxs-lookup"><span data-stu-id="6f037-161">CJIS Security Policy</span></span>](https://aka.ms/cjis-security-policy)
- [<span data-ttu-id="6f037-162">Microsoft 通用控制措施中樞合規性架構</span><span class="sxs-lookup"><span data-stu-id="6f037-162">Microsoft Common Controls Hub Compliance Framework</span></span>](https://www.microsoft.com/trustcenter/common-controls-hub)
- [<span data-ttu-id="6f037-163">Microsoft 政府雲端</span><span class="sxs-lookup"><span data-stu-id="6f037-163">Microsoft Government Cloud</span></span>](https://go.microsoft.com/fwlink/?linkid=2087246)
- [<span data-ttu-id="6f037-164">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="6f037-164">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
