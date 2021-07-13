---
title: 聯邦資訊處理標準 (FIPS) 發佈140-2
description: Microsoft 證明其密碼模組符合聯邦資訊處理標準。
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
ms.openlocfilehash: 2c51979122aaedda90bac74740e95c9d1265de74
ms.sourcegitcommit: 9b0c8852e73e2be54a0f9c6570da67f4964f616c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/12/2021
ms.locfileid: "53385003"
---
# <a name="federal-information-processing-standard-fips-publication-140-2"></a><span data-ttu-id="120e6-104">聯邦資訊處理標準 (FIPS) 發佈140-2</span><span class="sxs-lookup"><span data-stu-id="120e6-104">Federal Information Processing Standard (FIPS) Publication 140-2</span></span>

## <a name="fips-140-2-standard-overview"></a><span data-ttu-id="120e6-105">FIPS 140-2 standard 一覽</span><span class="sxs-lookup"><span data-stu-id="120e6-105">FIPS 140-2 standard overview</span></span>

<span data-ttu-id="120e6-106">聯邦資訊處理標準 (FIPS) 發佈140-2 是一種美國政府標準，可定義資訊技術產品中的加密模組最低安全性需求，如資訊技術管理改革的1996法案第5131中所定義。</span><span class="sxs-lookup"><span data-stu-id="120e6-106">The Federal Information Processing Standard (FIPS) Publication 140-2 is a U.S. government standard that defines minimum security requirements for cryptographic modules in information technology products, as defined in Section 5131 of the Information Technology Management Reform Act of 1996.</span></span>

<span data-ttu-id="120e6-107">「 [加密模組驗證](https://csrc.nist.gov/Projects/cryptographic-module-validation-program) 」 (CMVP) （美國國家標準和技術研究院 (NIST) 的共同工作，以及網路安全性 (CCCS) 的加拿大中心），會驗證加密模組的 *安全性需求，以取得加密模組* 標準 (（如 FIPS 140-2) 和相關的 FIPS 密碼編譯標準）。</span><span class="sxs-lookup"><span data-stu-id="120e6-107">The [Cryptographic Module Validation Program](https://csrc.nist.gov/Projects/cryptographic-module-validation-program) (CMVP), a joint effort of the U.S. National Institute of Standards and Technology (NIST) and the Canadian Centre for Cyber Security (CCCS), validates cryptographic modules to the *Security Requirements for Cryptographic Modules* standard (i.e., FIPS 140-2) and related FIPS cryptography standards.</span></span> <span data-ttu-id="120e6-108">FIPS 140-2 的安全性需求涵蓋11個與加密模組設計及實施相關的區域。</span><span class="sxs-lookup"><span data-stu-id="120e6-108">The FIPS 140-2 security requirements cover 11 areas related to the design and implementation of a cryptographic module.</span></span> <span data-ttu-id="120e6-109">NIST Information 技術實驗室會運作相關的程式，以驗證模組中的 FIPS 核准的加密演算法。</span><span class="sxs-lookup"><span data-stu-id="120e6-109">The NIST Information Technology Laboratory operates a related program that validates the FIPS approved cryptographic algorithms in the module.</span></span>

## <a name="microsofts-approach-to-fips-140-2-validation"></a><span data-ttu-id="120e6-110">Microsoft 的 FIPS 140-2 驗證方法</span><span class="sxs-lookup"><span data-stu-id="120e6-110">Microsoft's approach to FIPS 140-2 validation</span></span>

<span data-ttu-id="120e6-111">Microsoft 會維持積極的承諾，以滿足140-2 需求，因為標準是在2001內開始已驗證的加密模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-111">Microsoft maintains an active commitment to meeting the 140-2 requirements, having validated cryptographic modules since the standard's inception in 2001.</span></span> <span data-ttu-id="120e6-112">Microsoft 會在國家安全局) [加密模組驗證計畫](https://csrc.nist.gov/Projects/cryptographic-module-validation-program) (CMVP) 的標準及 (技術研究院下驗證其加密模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-112">Microsoft validates its cryptographic modules under the National Institute of Standards and Technology (NIST) [Cryptographic Module Validation Program](https://csrc.nist.gov/Projects/cryptographic-module-validation-program) (CMVP).</span></span> <span data-ttu-id="120e6-113">多個 Microsoft 產品（包含許多雲端服務）使用這些加密模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-113">Multiple Microsoft products, including many cloud services, use these cryptographic modules.</span></span>

<span data-ttu-id="120e6-114">如需 Microsoft Windows 加密模組的技術資訊、每個模組的安全性原則，以及 CMVP 憑證詳細資料的目錄，請參閱[Windows 和 Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud)。</span><span class="sxs-lookup"><span data-stu-id="120e6-114">For technical information on Microsoft Windows cryptographic modules, the security policy for each module, and the catalog of CMVP certificate details, see the [Windows and Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud).</span></span>

## <a name="microsoft-in-scope-cloud-platforms--services"></a><span data-ttu-id="120e6-115">Microsoft in 範圍內的雲端平臺 & 服務</span><span class="sxs-lookup"><span data-stu-id="120e6-115">Microsoft in-scope cloud platforms & services</span></span>

<span data-ttu-id="120e6-116">目前的 CMVP FIPS 140-2 實現指導方針會排除雲端服務本身的 FIPS 140-2 驗證，但雲端服務提供者可以選擇針對組成其雲端服務的計算元素，選擇取得並運作 FIPS 140 驗證的密碼模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-116">While the current CMVP FIPS 140-2 implementation guidance precludes a FIPS 140-2 validation for a cloud service itself; cloud service providers can choose to obtain and operate FIPS 140 validated cryptographic modules for the computing elements that comprise their cloud service.</span></span> <span data-ttu-id="120e6-117">Microsoft online services （包括已驗證 FIPS 140-2 的元件）包含下列各種：</span><span class="sxs-lookup"><span data-stu-id="120e6-117">Microsoft online services that include components, which have been FIPS 140-2 validated include, among others:</span></span>

- <span data-ttu-id="120e6-118">Azure 和 Azure Government</span><span class="sxs-lookup"><span data-stu-id="120e6-118">Azure and Azure Government</span></span>
- <span data-ttu-id="120e6-119">Dynamics 365 和 Dynamics 365 政府</span><span class="sxs-lookup"><span data-stu-id="120e6-119">Dynamics 365 and Dynamics 365 Government</span></span>
- <span data-ttu-id="120e6-120">Office 365、Office 365 美國政府和 Office 365 美國政府國防版</span><span class="sxs-lookup"><span data-stu-id="120e6-120">Office 365, Office 365 U.S. Government, and Office 365 U.S. Government Defense</span></span>

## <a name="azure-dynamics-365-and-fips-140-2"></a><span data-ttu-id="120e6-121">Azure、Dynamics 365 和 FIPS 140-2</span><span class="sxs-lookup"><span data-stu-id="120e6-121">Azure, Dynamics 365, and FIPS 140-2</span></span>

<span data-ttu-id="120e6-122">如需 Azure、Dynamics 365 及其他線上服務規範的詳細資訊，請參閱 [AZURE FIPS 140-2 產品](/azure/compliance/offerings/offering-fips-140-2)。</span><span class="sxs-lookup"><span data-stu-id="120e6-122">For more information about Azure, Dynamics 365, and other online services compliance, see the [Azure FIPS 140-2 offering](/azure/compliance/offerings/offering-fips-140-2).</span></span>

## <a name="office-365-and-fips-140-2"></a><span data-ttu-id="120e6-123">Office 365 和 FIPS 140-2</span><span class="sxs-lookup"><span data-stu-id="120e6-123">Office 365 and FIPS 140-2</span></span>

### <a name="office-365-cloud-environments"></a><span data-ttu-id="120e6-124">Office 365 雲端環境</span><span class="sxs-lookup"><span data-stu-id="120e6-124">Office 365 cloud environments</span></span>

[!INCLUDE [Office 365 offering intro](../includes/o365-offering-introduction.md)]

### <a name="office-365-applicability-and-in-scope-services"></a><span data-ttu-id="120e6-125">Office 365 適用性和範圍內服務</span><span class="sxs-lookup"><span data-stu-id="120e6-125">Office 365 applicability and in-scope services</span></span>

<span data-ttu-id="120e6-126">請使用下表來決定 Office 365 服務和訂閱的適用性：</span><span class="sxs-lookup"><span data-stu-id="120e6-126">Use the following table to determine applicability for your Office 365 services and subscription:</span></span>

| <span data-ttu-id="120e6-127">**適用性**</span><span class="sxs-lookup"><span data-stu-id="120e6-127">**Applicability**</span></span> | <span data-ttu-id="120e6-128">**範圍內的服務**</span><span class="sxs-lookup"><span data-stu-id="120e6-128">**In-scope services**</span></span> |
|:------------------|:----------------------|
| <span data-ttu-id="120e6-129">Office 365，GCC，GCC High，DoD</span><span class="sxs-lookup"><span data-stu-id="120e6-129">Office 365, GCC, GCC High, DoD</span></span> | <span data-ttu-id="120e6-130">請參閱 [FIPS 140-2 驗證](/windows/security/threat-protection/fips-140-validation)</span><span class="sxs-lookup"><span data-stu-id="120e6-130">See [FIPS 140-2 Validation](/windows/security/threat-protection/fips-140-validation)</span></span> |

### <a name="frequently-asked-questions"></a><span data-ttu-id="120e6-131">常見問題集</span><span class="sxs-lookup"><span data-stu-id="120e6-131">Frequently asked questions</span></span>

<span data-ttu-id="120e6-132">**「FIPS 140 驗證」與「FIPS 140 相容」有何差異？**</span><span class="sxs-lookup"><span data-stu-id="120e6-132">**What is the difference between 'FIPS 140 Validated' and 'FIPS 140 compliant'?**</span></span>

<span data-ttu-id="120e6-133">「FIPS 140 驗證」表示加密模組或嵌入模組的產品已驗證 CMVP 為滿足 FIPS 140-2 的需求 ( ' 已驗證」 ) 。</span><span class="sxs-lookup"><span data-stu-id="120e6-133">'FIPS 140 Validated' means that the cryptographic module, or a product that embeds the module has been validated ('certified') by the CMVP as meeting the FIPS 140-2 requirements.</span></span> <span data-ttu-id="120e6-134">「FIPS 140 相容」是 IT 產品的行業術語，其適用于已驗證 FIPS 140 的產品以取得加密功能。</span><span class="sxs-lookup"><span data-stu-id="120e6-134">'FIPS 140 compliant' is an industry term for IT products that rely on FIPS 140 Validated products for cryptographic functionality.</span></span>

<span data-ttu-id="120e6-135">**Microsoft 何時使用 FIPS 140 驗證？**</span><span class="sxs-lookup"><span data-stu-id="120e6-135">**When does Microsoft undertake a FIPS 140 validation?**</span></span>

<span data-ttu-id="120e6-136">開始模組驗證的節奏，與 Windows 10 和 Windows 伺服器的功能更新相符。</span><span class="sxs-lookup"><span data-stu-id="120e6-136">The cadence for starting a module validation aligns with the feature updates of Windows 10 and Windows Server.</span></span> <span data-ttu-id="120e6-137">隨著軟體行業的演化，作業系統的發行頻率也會隨每月軟體更新。</span><span class="sxs-lookup"><span data-stu-id="120e6-137">As the software industry evolved, operating systems are released more frequently, with monthly software updates.</span></span> <span data-ttu-id="120e6-138">Microsoft undertakes 的功能版本驗證，但在兩個版本之間，尋找最小化加密模組的變更。</span><span class="sxs-lookup"><span data-stu-id="120e6-138">Microsoft undertakes validation for feature releases, but in between releases, seeks to minimize the changes to the cryptographic modules.</span></span>

<span data-ttu-id="120e6-139">**FIPS 140 驗證中包含哪一部電腦？**</span><span class="sxs-lookup"><span data-stu-id="120e6-139">**Which computers are included in a FIPS 140 validation?**</span></span>

<span data-ttu-id="120e6-140">Microsoft 會在執行 Windows 10 和 Windows 伺服器的硬體設定範例上，驗證加密模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-140">Microsoft validates cryptographic modules on a representative sample of hardware configurations running Windows 10 and Windows Server.</span></span> <span data-ttu-id="120e6-141">在環境使用硬體時（類似于驗證程式使用的範例），常見的行業作法是接受此 FIPS 140-2 驗證。</span><span class="sxs-lookup"><span data-stu-id="120e6-141">It is common industry practice to accept this FIPS 140-2 validation when an environment uses hardware, which is similar to the samples used for the validation process.</span></span>

<span data-ttu-id="120e6-142">**NIST 網站上列出了許多模組。如何知道哪一種適用于我的代理人？**</span><span class="sxs-lookup"><span data-stu-id="120e6-142">**There are many modules listed on the NIST website. How do I know which one applies to my agency?**</span></span>

<span data-ttu-id="120e6-143">如果您需要使用透過 FIPS 140-2 驗證的加密模組，您必須確認您所用的版本會出現在 [驗證] 清單中。</span><span class="sxs-lookup"><span data-stu-id="120e6-143">If you are required to use cryptographic modules validated through FIPS 140-2, you need to verify that the version you use appears on the validation list.</span></span> <span data-ttu-id="120e6-144">CMVP 和 Microsoft 會維護已驗證的加密模組清單，依產品版本加以組織，以及識別在 Windows 系統上安裝哪些模組的指示。</span><span class="sxs-lookup"><span data-stu-id="120e6-144">The CMVP and Microsoft maintain a list of validated cryptographic modules, organized by product release, along with instructions for identifying which modules are installed on a Windows system.</span></span> <span data-ttu-id="120e6-145">如需設定系統相容性的詳細資訊，請參閱[Windows 和 Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud)。</span><span class="sxs-lookup"><span data-stu-id="120e6-145">For more information on configuring systems to be compliant, see the [Windows and Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud).</span></span>

<span data-ttu-id="120e6-146">**「在 FIPS 模式中運作」在憑證上的意義為何？**</span><span class="sxs-lookup"><span data-stu-id="120e6-146">**What does 'When operated in FIPS mode' mean on a certificate?**</span></span>

<span data-ttu-id="120e6-147">這項警告會告訴讀者，必須遵循必要的設定及安全性規則，以符合其 FIPS 140-2 安全性原則的方式使用加密模組。</span><span class="sxs-lookup"><span data-stu-id="120e6-147">This caveat informs the reader that required configuration and security rules must be followed to use the cryptographic module in a way that is consistent with its FIPS 140-2 security policy.</span></span> <span data-ttu-id="120e6-148">每個模組都有其自己的安全性原則（其運作所依據的安全性規則的確切規格），並採用核准的加密演算法、加密金鑰管理和驗證技術。</span><span class="sxs-lookup"><span data-stu-id="120e6-148">Each module has its own security policy — a precise specification of the security rules under which it will operate — and employs approved cryptographic algorithms, cryptographic key management, and authentication techniques.</span></span> <span data-ttu-id="120e6-149">安全性規則是定義于每個模組的安全性原則中。</span><span class="sxs-lookup"><span data-stu-id="120e6-149">The security rules are defined in the security policy for each module.</span></span> <span data-ttu-id="120e6-150">如需詳細資訊，包括透過 CMVP 驗證之每個模組的安全性原則連結，請參閱[Windows 和 Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud)。</span><span class="sxs-lookup"><span data-stu-id="120e6-150">For more information, including links to the security policy for each module validated through the CMVP, see the [Windows and Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud).</span></span>

<span data-ttu-id="120e6-151">**FedRAMP 是否需要 FIPS 140-2 驗證？**</span><span class="sxs-lookup"><span data-stu-id="120e6-151">**Does FedRAMP require FIPS 140-2 validation?**</span></span>

<span data-ttu-id="120e6-152">是的，「聯邦風險和授權管理」方案 (FedRAMP) 取決於 [NIST SP 800-53 Revision 4](https://nvd.nist.gov/800-53/Rev4/)所定義的控制基準，包含 [SC-13 加密保護](https://nvd.nist.gov/800-53/Rev4/control/SC-13) ，使用 FIPS 驗證的密碼編譯或 NSA 核准的密碼編譯。</span><span class="sxs-lookup"><span data-stu-id="120e6-152">Yes, the Federal Risk and Authorization Management Program (FedRAMP) relies on control baselines defined by the [NIST SP 800-53 Revision 4](https://nvd.nist.gov/800-53/Rev4/), including [SC-13 Cryptographic Protection](https://nvd.nist.gov/800-53/Rev4/control/SC-13) mandating the use of FIPS-validated cryptography or NSA-approved cryptography.</span></span>

<span data-ttu-id="120e6-153">**我是否可以在代理人的認證程式中使用 Microsoft 遵守 FIPS 140-2 的功能？**</span><span class="sxs-lookup"><span data-stu-id="120e6-153">**Can I use Microsoft's adherence to FIPS 140-2 in my agency's certification process?**</span></span>

<span data-ttu-id="120e6-154">若要遵守 FIPS 140-2，您的系統必須設定為在作業的 FIPS 核准模式中執行，包括確保密碼模組只使用 FIPS 核准的演算法。</span><span class="sxs-lookup"><span data-stu-id="120e6-154">To comply with FIPS 140-2, your system must be configured to run in a FIPS approved mode of operation, which includes ensuring that a cryptographic module uses only FIPS-approved algorithms.</span></span> <span data-ttu-id="120e6-155">如需設定系統相容性的詳細資訊，請參閱[Windows 和 Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud)。</span><span class="sxs-lookup"><span data-stu-id="120e6-155">For more information on configuring systems to be compliant, see the [Windows and Windows Server FIPS 140-2 content](https://aka.ms/AA6ehud).</span></span>

<span data-ttu-id="120e6-156">**FIPS 140-2 與通用準則之間的關係為何？**</span><span class="sxs-lookup"><span data-stu-id="120e6-156">**What is the relationship between FIPS 140-2 and Common Criteria?**</span></span>

<span data-ttu-id="120e6-157">這些是兩個不同的安全性標準，但相互互補。</span><span class="sxs-lookup"><span data-stu-id="120e6-157">These are two separate security standards with different, but complementary, purposes.</span></span> <span data-ttu-id="120e6-158">FIPS 140-2 是專門設計用來驗證軟體和硬體密碼模組，而一般的準則是用來評估 IT 軟體和硬體產品中的安全性功能。</span><span class="sxs-lookup"><span data-stu-id="120e6-158">FIPS 140-2 is designed specifically for validating software and hardware cryptographic modules, while the Common Criteria is designed to evaluate security functions in IT software and hardware products.</span></span> <span data-ttu-id="120e6-159">常見的準則評估通常會依靠 FIPS 140-2 驗證，以確保基本的加密功能已正確地執行。</span><span class="sxs-lookup"><span data-stu-id="120e6-159">Common Criteria evaluations often rely on FIPS 140-2 validations to provide assurance that basic cryptographic functionality is implemented properly.</span></span>

### <a name="resources"></a><span data-ttu-id="120e6-160">資源</span><span class="sxs-lookup"><span data-stu-id="120e6-160">Resources</span></span>

- [<span data-ttu-id="120e6-161">FIPS Pub 140-2 加密模組的安全性需求</span><span class="sxs-lookup"><span data-stu-id="120e6-161">FIPS Pub 140-2 Security Requirements for Cryptographic Modules</span></span>](https://csrc.nist.gov/publications/fips/fips140-2/fips1402.pdf)
- [<span data-ttu-id="120e6-162">NIST 加密模組驗證程式</span><span class="sxs-lookup"><span data-stu-id="120e6-162">NIST Cryptographic Module Validation Program</span></span>](https://csrc.nist.gov/groups/STM/cmvp/index.html)
- [<span data-ttu-id="120e6-163">Windows、Windows 伺服器及 FIPS 140-2</span><span class="sxs-lookup"><span data-stu-id="120e6-163">Windows, Windows Server, and FIPS 140-2</span></span>](/windows/security/threat-protection/fips-140-validation)
- [<span data-ttu-id="120e6-164">Microsoft 信任中心的合規性</span><span class="sxs-lookup"><span data-stu-id="120e6-164">Compliance on the Microsoft Trust Center</span></span>](https://www.microsoft.com/trust-center/compliance/compliance-overview)
