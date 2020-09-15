---
title: Rozwiązywanie problemów z poradami dotyczącymi bezpieczeństwa dla kontroli wykrywania nadużyć
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658420"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rozwiązywanie problemów z poradami dotyczącymi bezpieczeństwa dla kontroli wykrywania nadużyć

Jeśli otrzymasz poradę dotyczącą bezpieczeństwa, na której znajduje się komunikat "nadawca nie mógł sprawdzić, czy nasze testy wykrywania nadużyć finansowych, i może nie być", oznacza to, że nadawca nie przeszedł testów uwierzytelniania DKIM lub SPF. Najlepszym sposobem na rozwiązanie tego problemu jest udzielenie nadawcy autoryzacji. Jeśli nadawca wysyła dane w Twoim imieniu, trzeba je autoryzować, dodając adres IP nadawcy do rekordu SPF.
  
Zobacz [Rozwiązywanie problemów z czerwonymi (podejrzanymi) wskazówkami dotyczącymi wykrywania nadużyć](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) , aby uzyskać więcej informacji.
  
Oto kilka innych linków, które mogą pomóc:
  
- [Jak firma Microsoft używa struktury zasad nadawców (SPF) w celu zapobiegania podszywaniu się](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurowanie SPF w celu zapobiegania podszywaniu się](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
