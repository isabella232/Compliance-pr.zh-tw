---
title: 網路安全性
description: 深入瞭解 Microsoft 365 中的網路安全性
ms.author: robmazz
author: robmazz
manager: laurawi
ms.reviewer: sosstah
audience: Admin
ms.topic: article
f1.keywords:
- NOCSH
ms.service: O365-seccomp
localization_priority: Normal
ms.collection:
- Strat_O365_IP
- M365-security-compliance
- MS-Compliance
search.appverid:
- MET150
- MOE150
titleSuffix: Microsoft Service Assurance
hideEdit: true
ms.openlocfilehash: a2b153b2f2f57a011c28ee65cbe03019cbaa27a1
ms.sourcegitcommit: 024137a15ab23d26cac5ec14c36f3577fd8a0cc4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2021
ms.locfileid: "51496919"
---
# <a name="network-security-overview"></a>網路安全性概觀

## <a name="how-does-microsoft-365-secure-the-network-boundary"></a>Microsoft 365 如何保護網路界限？

Microsoft 365 採用多種策略來保護其網路界限，包括自動偵測及防護網路型攻擊、特殊防火牆裝置和 Exchange Online Protection (EOP) ，以進行反垃圾郵件和反惡意程式碼保護。 此外，Microsoft 365 會將其實際執行環境分隔成邏輯隔離的網段，只允許在區段之間進行必要的通訊。 網路流量會以邊界點為其他網路防火牆進行保護，以協助偵測、防止及緩解網路攻擊。

## <a name="how-does-microsoft-365-defend-against-ddos-attacks"></a>Microsoft 365 如何防禦 DDoS 攻擊？

Microsoft 的大型網際網路平臺服務會將其與許多分散式阻斷服務 (DDoS) 攻擊的負面影響隔離開來。 每個 Microsoft 365 服務的分散式實例，以及每個服務的多個路由，都限制對系統的 DDoS 攻擊所造成的影響。 這項重複的功能提高了 Microsoft 365 吸收 DDoS 攻擊的能力，增加了可在影響服務可用性之前，偵測及緩解 DDoS 攻擊的時間量。

除了 Microsoft 的重複系統架構之外，Microsoft 還使用複雜的偵測和緩解工具來回應 DDoS 攻擊。 特殊用途的防火牆會監視和丟棄不想要的流量，使邊界跨越網路，以減少位於網路界限內之系統的壓力。 若要進一步保護我們的雲端服務，Microsoft 會利用在 Microsoft Azure 中部署的 DDoS 防護系統。 Azure DDoS 防護系統的設計是為了經受外界和其他 Azure 承租人的攻擊。

## <a name="how-does-microsoft-365-protect-users-against-spam-and-malware-being-uploaded-or-sent-through-online-services"></a>Microsoft 365 如何針對透過線上服務上傳或傳送的垃圾郵件和惡意程式碼保護使用者？

Microsoft 365 會為服務建立反惡意程式碼保護，而這些服務可能是惡意程式碼的向量，例如 Exchange Online 和 SharePoint 線上。 Exchange Online Protection (EOP) 會掃描所有電子郵件和電子郵件附件中的惡意程式碼，以防惡意程式碼進入並退出系統，以防傳遞受感染的郵件和附件。 「高級垃圾郵件篩選」會自動套用至輸入和輸出郵件，以協助防止客戶組織接收和傳送垃圾郵件。 這種保護層會防範利用未經授權或未經授權電子郵件的攻擊，例如網路釣魚攻擊。 線上 SharePoint 會使用相同的病毒偵測引擎，選擇性地掃描上傳的檔案是否有惡意程式碼。 如果檔案標示為已感染，使用者就無法下載或同步處理該檔案，以保護用戶端端點。

## <a name="related-external-regulations--certifications"></a>相關的外部法規 & 認證

Microsoft 的線上服務會定期進行審核，以符合外部法規和認證。 請參閱下表，以驗證與網路安全性相關的控制項。

| **外部審計** | **Section** | **最新報告日期** |
|:--------------------|:------------|:-----------------------|
| [FedRAMP (Office 365) ](https://compliance.microsoft.com/compliancemanager) | SC-5：拒絕服務保護 <br> SC-7：界限保護 <br> SI-2：缺陷修正 <br> SI-3：惡意程式碼保護 <br> SI-8：垃圾郵件保護 | 2020年9月24日 |
| [SOC 1 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=90df3f9c-3aaf-4dbf-99d0-ca9f2991721b&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27：薄弱環節掃描 | 2020月24日 |
| [SOC 2 (Office 365) ](https://servicetrust.microsoft.com/ViewPage/MSComplianceGuideV3?command=Download&downloadType=Document&downloadId=a73c1738-7892-42b7-acd3-87b6371c53f6&tab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb&docTab=7027ead0-3d6b-11e9-b9e1-290b1eb4cdeb_SOC_%2F_SSAE_16_Reports) | CA-27：薄弱環節掃描 <br> CA-45：反惡意程式碼 | 2020月24日 |