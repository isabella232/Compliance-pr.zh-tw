---
title: 資料分類 & 敏感度標籤分類法
description: 在本文中，您可以看到使用資料分類 & 敏感度標籤分類法搭配 Microsoft 365 的概況。
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
ms.custom: seo-marvel-apr2020
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: fcfe98116f4d0629f322383f2992605d2dcf19de
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51497793"
---
# <a name="data-classification--sensitivity-label-taxonomy"></a><span data-ttu-id="889a8-103">資料分類 & 敏感度標籤分類法</span><span class="sxs-lookup"><span data-stu-id="889a8-103">Data classification & sensitivity label taxonomy</span></span>

<span data-ttu-id="889a8-104">敏感性資料對於公司失竊、無意間共用或透過破壞行為公開時，會對公司帶來重大的風險。</span><span class="sxs-lookup"><span data-stu-id="889a8-104">Sensitive data presents significant risk to a company if it is stolen, inadvertently shared, or exposed through a breach.</span></span> <span data-ttu-id="889a8-105">風險因素包括 reputational 損毀、財務影響，以及競爭優勢的喪失。</span><span class="sxs-lookup"><span data-stu-id="889a8-105">Risk factors include reputational damage, financial impact, and loss of competitive advantage.</span></span> <span data-ttu-id="889a8-106">保護您的商務管理資料和資訊您的組織是頭等大事，但如果您的企業所需的內容數量非常有效率，您可能會發現您很難知道您的工作是否真的有效。</span><span class="sxs-lookup"><span data-stu-id="889a8-106">Protecting the data and information your business manages is a top priority for your organization, but you may find it difficult to know if your efforts are truly effective, given the amount of content held by your enterprise.</span></span>

<span data-ttu-id="889a8-107">除了大量之外，您的內容還會從高度機密和 impactful 到簡單且暫時性的重要性。</span><span class="sxs-lookup"><span data-stu-id="889a8-107">In addition to volume, your content may range in importance from highly sensitive and impactful to trivial and transient.</span></span> <span data-ttu-id="889a8-108">也可以是各種法規遵從性需求的 purview。</span><span class="sxs-lookup"><span data-stu-id="889a8-108">It can also be under the purview of various regulatory compliance requirements.</span></span> <span data-ttu-id="889a8-109">知道要設定優先順序及在何處套用控制項可能是一項挑戰。</span><span class="sxs-lookup"><span data-stu-id="889a8-109">Knowing what to prioritize and where to apply controls can be a challenge.</span></span> <span data-ttu-id="889a8-110">請繼續閱讀以瞭解 *資料分類*、保護內容免受盜竊、破壞或不慎毀壞的重要工具，以及 Microsoft 365 如何協助您符合資訊安全性目標。</span><span class="sxs-lookup"><span data-stu-id="889a8-110">Read on to learn about *data classification*, an important tool for protecting your content from theft, sabotage, or inadvertent destruction, and how Microsoft 365 can help you meet your information security goals.</span></span>

## <a name="what-is-data-classification"></a><span data-ttu-id="889a8-111">何謂資料分類？</span><span class="sxs-lookup"><span data-stu-id="889a8-111">What is data classification?</span></span>

<span data-ttu-id="889a8-112">[資料分類](/microsoft-365/compliance/data-classification-overview) 是 cybersecurity 和資訊管理的欄位中所用的特殊術語，用以描述根據敏感度或影響等級識別、分類及保護內容的程式。</span><span class="sxs-lookup"><span data-stu-id="889a8-112">[Data classification](/microsoft-365/compliance/data-classification-overview) is a specialized term used in the fields of cybersecurity and information governance to describe the process of identifying, categorizing, and protecting content according to its sensitivity or impact level.</span></span> <span data-ttu-id="889a8-113">在最基本的表單中，資料分類是一種方法，根據敏感或 impactful 的程度，保護您的資料不會遭到未經授權的披露、篡改或銷毀。</span><span class="sxs-lookup"><span data-stu-id="889a8-113">In its most basic form, data classification is a means of protecting your data from unauthorized disclosure, alteration, or destruction based on how sensitive or impactful it is.</span></span>

## <a name="what-is-a-data-classification-framework"></a><span data-ttu-id="889a8-114">何謂資料分類架構？</span><span class="sxs-lookup"><span data-stu-id="889a8-114">What is a data classification framework?</span></span>

<span data-ttu-id="889a8-115">通常 codified 在全企業級原則中，資料分類架構 (有時稱為「資料分類原則」 ) 通常是由3-5 分類層級所組成。</span><span class="sxs-lookup"><span data-stu-id="889a8-115">Often codified in a formal, enterprise-wide policy, a data classification framework (sometimes called a 'data classification policy') is typically comprised of 3-5 classification levels.</span></span> <span data-ttu-id="889a8-116">這通常包括三個元素：名稱、描述及實際範例。</span><span class="sxs-lookup"><span data-stu-id="889a8-116">These usually include three elements: a name, description, and real-world examples.</span></span> <span data-ttu-id="889a8-117">Microsoft 建議沒有超過五個最上層的父標籤，每個都有五個子標籤 () 25 個，以保持使用者介面 (UI) 可供管理。</span><span class="sxs-lookup"><span data-stu-id="889a8-117">Microsoft recommends no more than five top-level parent labels, each with five sub-labels (25 total) to keep the user interface (UI) manageable.</span></span> <span data-ttu-id="889a8-118">層級通常會從至少一個最敏感的組織，例如「*公用*」、「*內部*」、「*機密*」和「*高度* 
 *機密*」。</span><span class="sxs-lookup"><span data-stu-id="889a8-118">Levels are typically arranged from least to most sensitive such as *Public*, *Internal*, *Confidential*, and *Highly*
*Confidential*.</span></span> <span data-ttu-id="889a8-119">您可能會遇到的其他層級名稱變化包括 *限制*、不 *受限制* 和 *使用中受保護* 的。</span><span class="sxs-lookup"><span data-stu-id="889a8-119">Other level name variations you may encounter include *Restricted*, *Unrestricted*, and *Consumer Protected*.</span></span> <span data-ttu-id="889a8-120">Microsoft 建議的標籤名稱是自我描述的，明確強調其相對敏感性。</span><span class="sxs-lookup"><span data-stu-id="889a8-120">Microsoft recommends label names that are self-descriptive and that highlight their relative sensitivity clearly.</span></span> <span data-ttu-id="889a8-121">例如， *機密* 和 *限制* 可能會讓使用者猜測適當的標籤，而 *機密* 和 *高度機密* 會變得更清晰。</span><span class="sxs-lookup"><span data-stu-id="889a8-121">For example, *Confidential* and *Restricted* may leave users guessing which label is appropriate, while *Confidential* and *Highly Confidential* are clearer on which is more sensitive.</span></span> <span data-ttu-id="889a8-122">下表顯示資料分類架構層級的範例。</span><span class="sxs-lookup"><span data-stu-id="889a8-122">The following table shows examples of data classification framework levels.</span></span>

|<span data-ttu-id="889a8-123">**分類層級**</span><span class="sxs-lookup"><span data-stu-id="889a8-123">**Classification level**</span></span>|<span data-ttu-id="889a8-124">**描述**</span><span class="sxs-lookup"><span data-stu-id="889a8-124">**Description**</span></span>|<span data-ttu-id="889a8-125">**範例**</span><span class="sxs-lookup"><span data-stu-id="889a8-125">**Examples**</span></span>|
|:-----------------------|:--------------|:-----------|
| <span data-ttu-id="889a8-126">高度機密</span><span class="sxs-lookup"><span data-stu-id="889a8-126">Highly Confidential</span></span> | <span data-ttu-id="889a8-127">高度機密資料是由企業儲存或管理的最敏感資料類型，如果破壞或披露，可能需要法律通知。</span><span class="sxs-lookup"><span data-stu-id="889a8-127">Highly Confidential data is the most sensitive type of data stored or managed by the enterprise and may require legal notifications if breached or otherwise disclosed.</span></span> <br><br> <span data-ttu-id="889a8-128">受限制的資料需要最高級別的控制和安全性，且存取權應限制為「需要即知」。</span><span class="sxs-lookup"><span data-stu-id="889a8-128">Restricted Data requires the highest level of control and security, and access should be limited to "need-to- know."</span></span> | <span data-ttu-id="889a8-129">機密的個人身分識別資訊 (敏感 PII) </span><span class="sxs-lookup"><span data-stu-id="889a8-129">Sensitive Personally Identifiable Information (Sensitive PII)</span></span> <br> <span data-ttu-id="889a8-130">持卡人資料</span><span class="sxs-lookup"><span data-stu-id="889a8-130">Cardholder Data</span></span> <br> <span data-ttu-id="889a8-131">受保護的健康資訊 (PHI) </span><span class="sxs-lookup"><span data-stu-id="889a8-131">Protected Health Information (PHI)</span></span> <br> <span data-ttu-id="889a8-132">銀行帳戶資料</span><span class="sxs-lookup"><span data-stu-id="889a8-132">Bank Account Data</span></span> |

>[!TIP]
><span data-ttu-id="889a8-133">Microsoft 公司資料分類架構最初在試驗階段使用類別及標籤 ' Internal '，但是發現檔有合理的原因是要在外部共用檔，並將檔移至使用「一般」。</span><span class="sxs-lookup"><span data-stu-id="889a8-133">Microsoft's corporate data classification framework originally used a category and label named 'Internal' during pilot phase but found that there were legitimate reasons for a document to be shared externally and shifted to using 'General'.</span></span>

<span data-ttu-id="889a8-134">資料分類架構的另一個重要元件是與每個層級相關聯的控制項。</span><span class="sxs-lookup"><span data-stu-id="889a8-134">Another important component of a data classification framework is the controls associated with each level.</span></span> <span data-ttu-id="889a8-135">資料分類層級本身只是標籤 (或標記) ，表示內容的值或敏感度。</span><span class="sxs-lookup"><span data-stu-id="889a8-135">Data classification levels by themselves are simply labels (or tags) that indicate the value or sensitivity of the content.</span></span> <span data-ttu-id="889a8-136">為了 *保護* 該內容，資料分類框架會定義應該針對每個資料分類層級採用的控制項。</span><span class="sxs-lookup"><span data-stu-id="889a8-136">To *protect* that content, data classification frameworks define the controls that should be in place for each of your data classification levels.</span></span> <span data-ttu-id="889a8-137">這些控制項可能包含下列相關需求：</span><span class="sxs-lookup"><span data-stu-id="889a8-137">These controls may include requirements related to:</span></span>

- <span data-ttu-id="889a8-138">儲存區類型和位置</span><span class="sxs-lookup"><span data-stu-id="889a8-138">Storage type and location</span></span>
- <span data-ttu-id="889a8-139">加密</span><span class="sxs-lookup"><span data-stu-id="889a8-139">Encryption</span></span>
- <span data-ttu-id="889a8-140">存取控制</span><span class="sxs-lookup"><span data-stu-id="889a8-140">Access control</span></span>
- <span data-ttu-id="889a8-141">資料銷毀</span><span class="sxs-lookup"><span data-stu-id="889a8-141">Data destruction</span></span>
- <span data-ttu-id="889a8-142">資料外洩防護</span><span class="sxs-lookup"><span data-stu-id="889a8-142">Data loss prevention</span></span>
- <span data-ttu-id="889a8-143">公開披露</span><span class="sxs-lookup"><span data-stu-id="889a8-143">Public disclosure</span></span>
- <span data-ttu-id="889a8-144">記錄和追蹤存取</span><span class="sxs-lookup"><span data-stu-id="889a8-144">Logging and tracking access</span></span>
- <span data-ttu-id="889a8-145">如有需要，其他控制目標</span><span class="sxs-lookup"><span data-stu-id="889a8-145">Other control objectives, as needed</span></span>

<span data-ttu-id="889a8-146">您的安全性控制措施會因數據分類層級而異，如此一來，您的架構中定義的保護措施會使您的內容敏感度增加 commensurate。</span><span class="sxs-lookup"><span data-stu-id="889a8-146">Your security controls will vary by data classification level, such that the protective measures defined in your framework increase commensurate with the sensitivity of your content.</span></span> <span data-ttu-id="889a8-147">例如，您的資料儲存區需求會根據所使用的媒體，以及套用至指定內容的分類層級而有所不同。</span><span class="sxs-lookup"><span data-stu-id="889a8-147">For example, your data storage control requirements will vary depending upon the media that is being used as well as upon the classification level applied to a given piece of content.</span></span> <span data-ttu-id="889a8-148">下表顯示特定儲存類型的資料分類控制項範例：</span><span class="sxs-lookup"><span data-stu-id="889a8-148">The following table shows an example of data classification controls for a specific storage type:</span></span>

|<span data-ttu-id="889a8-149">**儲存類型**</span><span class="sxs-lookup"><span data-stu-id="889a8-149">**Storage type**</span></span>|<span data-ttu-id="889a8-150">**機密**</span><span class="sxs-lookup"><span data-stu-id="889a8-150">**Confidential**</span></span>|<span data-ttu-id="889a8-151">**內部**</span><span class="sxs-lookup"><span data-stu-id="889a8-151">**Internal**</span></span>|<span data-ttu-id="889a8-152">**無限制**</span><span class="sxs-lookup"><span data-stu-id="889a8-152">**Unrestricted**</span></span>|
|:---------------|:---------------|:-----------|:---------------|
| <span data-ttu-id="889a8-153">可拆卸儲存體</span><span class="sxs-lookup"><span data-stu-id="889a8-153">Removable Storage</span></span> | <span data-ttu-id="889a8-154">禁止</span><span class="sxs-lookup"><span data-stu-id="889a8-154">Prohibited</span></span> | <span data-ttu-id="889a8-155">除非加密，否則禁止</span><span class="sxs-lookup"><span data-stu-id="889a8-155">Prohibited unless encrypted</span></span> | <span data-ttu-id="889a8-156">不需要控制項</span><span class="sxs-lookup"><span data-stu-id="889a8-156">No control required</span></span> |

<span data-ttu-id="889a8-157">正確套用適當層級的資料分類可能會在實際的情況很複雜，有時可能會讓使用者不堪重負。</span><span class="sxs-lookup"><span data-stu-id="889a8-157">Correctly applying the right level of data classification can be complex in real-life situations and may sometimes overwhelm end users.</span></span> <span data-ttu-id="889a8-158">在建立原則或標準以定義所需的資料分類層級之後，請務必讓使用者瞭解如何在日常工作中讓此架構生命週期。</span><span class="sxs-lookup"><span data-stu-id="889a8-158">Once a policy or standard has been created that defines the required levels of data classification, it is important to guide end users on how to bring this framework to life in their daily work.</span></span> <span data-ttu-id="889a8-159">此區域是資料分類處理規則或指導方針的所在位置。</span><span class="sxs-lookup"><span data-stu-id="889a8-159">This area is where data classification handling rules or guidelines come in.</span></span>

<span data-ttu-id="889a8-160">資料分類處理指導方針會協助使用者如何適當地處理每個資料層級的特定指導方針，以供不同的儲存媒體生命週期使用。</span><span class="sxs-lookup"><span data-stu-id="889a8-160">Data classification handling guidelines will help end users with specific guidance on how to handle each level of data appropriately, for different storage media throughout their lifecycle.</span></span> <span data-ttu-id="889a8-161">這些指導方針可協助使用者正確地套用規則，例如，共用檔、傳送電子郵件，或跨不同的平臺和組織進行共同作業。</span><span class="sxs-lookup"><span data-stu-id="889a8-161">These guidelines help end users to correctly apply rules in practice, for instance when sharing documents, sending emails, or collaborating across different platforms and organizations.</span></span>

<span data-ttu-id="889a8-162">Microsoft 客戶指出，大約50% 的資訊保護專案是以業務為重點的方式，而不是技術，因此，使用者的訓練和通訊對成功率很重要。</span><span class="sxs-lookup"><span data-stu-id="889a8-162">Microsoft customers indicate that approximately 50% of an Information Protection project is business focused rather than technical, so end-user training and communication is critical to success.</span></span>
