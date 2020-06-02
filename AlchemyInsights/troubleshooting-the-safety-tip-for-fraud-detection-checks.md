---
title: Rozwiązywanie problemów z wskazówką dotyczącą bezpieczeństwa podczas kontroli wykrywania oszustw
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504993"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rozwiązywanie problemów z wskazówką dotyczącą bezpieczeństwa podczas kontroli wykrywania oszustw

Jeśli otrzymujesz wskazówkę dotyczącą bezpieczeństwa z napisem "Nadawca nie przeszedł naszych kontroli wykrywania oszustw i może nie być tym, kim wydają się być", nadawca nie przeszedł kontroli uwierzytelniania DKIM lub SPF. Najlepszą metodą rozwiązania tego problemu jest autoryzowanie przez nadawcę. Jeśli nadawca wysyła w Twoim imieniu, musisz je autoryzować, dodając adres IP nadawcy do rekordu SPF.
  
Aby uzyskać więcej informacji, zobacz [Rozwiązywanie problemów z czerwoną (podejrzaną) wskazówką dotyczącą bezpieczeństwa, aby uzyskać](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) więcej informacji.
  
Oto kilka innych linków, które mogą pomóc:
  
- [Jak firma Microsoft korzysta z struktury zasad nadawców (SPF), aby zapobiec fałszowaniu](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurowanie filtra SPF w celu zapobiegania fałszowaniu](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
