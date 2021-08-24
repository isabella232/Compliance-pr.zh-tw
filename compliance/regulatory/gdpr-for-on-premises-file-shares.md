---
title: 適用於內部部署檔案共用的 GDPR
description: 瞭解如何解決內部部署 Windows Server 檔案共用中的一般資料保護規定 (GDPR) 需求。
f1.keywords:
- NOCSH
ms.author: mikeplum
author: MikePlumleyMSFT
manager: pamgreen
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: high
titleSuffix: Microsoft GDPR
ms.custom: seo-marvel-apr2020
ms.collection: MS-Compliance
hideEdit: true
ms.openlocfilehash: 9c281b6096512f65f20286948addc32127278b98
ms.sourcegitcommit: 4c00fd65d418065d7f53216c91f455ccb3891c77
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58482326"
---
# <a name="gdpr-for-on-premises-windows-server-file-shares"></a>適用於內部部署 Windows Server 檔案共用的 GDPR

對於檔案共用的基本建議方法是：

-   使用 Azure 資訊保護來標記機密資料。

-   使用 Azure 資訊保護掃描器來尋找資料。

檔案共用的建議方法包括下列步驟：

1.  **安裝及設定 Azure 資訊保護掃描器。**

    -   決定要使用哪個機密資料類型。

    -   指定要使用的本機資料夾和網路共用。

2.  **完成探索循環。**

    -   在探索模式中執行掃描器，並且驗證結果。

    -   視需要最佳化條件和機密資訊類型。

    -   評估自動套用標籤的預期影響。

3.  **執行 Azure 資訊保護掃描器以將標籤套用至符合資格的文件**。

4.  **針對保護：**

    -   設定 Exchange 資料外洩防護規則，保護具有所需標籤的文件。

    -   請務必使用權限來限制可以存取檔案的人員。

5.  **針對監視，整合 Windows Server 記錄與 SIEM 工具。**

    -   若要針對資料主體要求尋找個人資料，請使用 Azure 資訊保護掃描器。您也可以設定 SharePoint Server 搜尋來對檔案共用進行編目。

如需有關使用 Azure 資訊保護掃描器來找出個人資料並加上標籤的詳細資訊，請參閱[部署 AIP 掃描程式](/azure/information-protection/deploy-aip-scanner)。

如需有關針對條件設定掃描器，以及使用 Office 365 資料外洩防護 (DLP) 機密資訊類型的詳細資訊，請參閱＜[如何針對 Azure 資訊保護的自動和建議分類設定條件](/information-protection/deploy-use/configure-policy-classification)＞。請注意，新的 Office 365 機密資訊類型無法立即與掃描器搭配使用，且自訂機密資訊類型無法與掃描器搭配使用。
