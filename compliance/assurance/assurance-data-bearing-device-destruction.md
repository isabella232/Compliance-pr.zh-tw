---
title: 資料承載裝置毀壞
description: 在本文中，您將會看到 Microsoft 資料中心的資料貼上裝置銷毀處理常式的概述。
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: ITPro
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
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
ms.openlocfilehash: 6a26334b805be069298302d3ad1e8e5b9e728150
ms.sourcegitcommit: 997dd3f66f65686c2e38b7e30e67add426dce5f3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2021
ms.locfileid: "58946935"
---
# <a name="data-bearing-device-destruction"></a>資料承載裝置毀壞

## <a name="data-destruction-overview"></a>資料銷毀概述

Microsoft 有資料貼上裝置 (DBD) 指導方針、原則、安全性需求，以及在 Microsoft 資料中心內 DBDs 處理及管理的程式。

DBD 是可以儲存客戶或專有 Microsoft 資料的任何儲存裝置：

- 硬碟磁碟機 (磁片磁碟機) 
- 實體狀態磁片磁碟機 (SSD) 
- USB 磁片磁碟機
- IO 加速卡
- SD/壓縮快閃記憶體卡
- HSM 卡片
- PCIe SSD 卡
- NVDIMM (非易變雙行記憶體模組) 

在資料中心校園內，會審核和銷毀在 Microsoft 資料中心內使用的失敗 DBDs。 所有從服務撤銷的資產都會以 commensurate 的方式，評估其安全性/隱私權需求和資產分類，並依照任何適用的規則、法律和法規進行處置。

Microsoft 使用三種資料淨化類別，針對 DBDs 和包含資料的資產：

- **Clear**：相關的邏輯技術，可協助清理所有使用者定址儲存位置中的資料，以防範簡單非破壞性的資料復原技術。 這些技術通常是透過標準讀取和寫入命令套用至儲存裝置，例如使用新的值進行重新寫入，或使用功能表選項，將裝置重設為出廠狀態，而不支援重新寫入 () 。
- **清除**：與使用一流的實驗技術所呈現目標資料復原的實體或邏輯技術相關。
- **銷毀**：使用一流的實驗技術，呈現目標資料復原不可行，而且會導致後續無法使用媒體儲存資料。

清除和銷毀淨化是透過安全性群組所核准的工具和程式來執行。 記錄會保留資產的擦除和銷毀。 無法完成 clear 的裝置會順利 degaussed (針對磁性媒體) 、多 pin 打孔 (，以供 Ssd) 或損毀的 chipped。

## <a name="clear"></a>Clear

若評估並認定已報廢的資產無法存取，則已核准的資料 eradication 解決方案會將其清除。 Microsoft 資料中心使用 NIST SP-800-88 clear 指導方針。

## <a name="purge"></a>清除

根據網站上的設定和裝置可用性而定，某些裝置會在銷毀之前清除。 清除裝置包含針對磁性介質的 NSA 核准 degaussers，以及用於固態媒體的多針沖孔裝置。 Microsoft 資料中心使用 NIST SP-2-800-88 清除指導方針。

## <a name="destroy"></a>摧毀

若評估並認定已報廢的資產可供存取，則會使用符合 NIST SP-2-800-88 指導方針的核准標準作業程式，銷毀現場。 這些 DBDs 會以實際和邏輯方式追蹤，以維護透過最後處置的保管鏈。

每個 Microsoft 資料中心都使用現場流程來淨化及處理失敗及已撤銷的 DBDs。 在此程式中，Microsoft 人員確定整個處置過程中維護的保管階層。

## <a name="resources"></a>資源

- [NIST 特殊出版物800-88](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf)
