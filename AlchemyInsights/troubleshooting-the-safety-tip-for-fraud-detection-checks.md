---
title: Rozwiązywanie problemów z poradami w zakresie bezpieczeństwa podczas sprawdzania wykrywania oszustw
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834741"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rozwiązywanie problemów z poradami w zakresie bezpieczeństwa podczas sprawdzania wykrywania oszustw

Jeśli jest wyświetlana porada o bezpieczeństwie z treścią informacji "Nadawca zakończył testy wykrywania oszustw i może nie być tym, kto tak jest", oznacza to, że nadawca nie przejdzie testów uwierzytelniania DKIM lub SPF. Najlepszą metodą rozwiązania tego problemu jest autoryzacja siebie przez nadawcę. Jeśli nadawca wysyła w Twoim imieniu, musisz autoryzować go, dodając adres IP nadawcy do Twojego rekordu SPF.
  
Aby uzyskać więcej informacji, zobacz Rozwiązywanie problemów dotyczących [czerwonej (podejrzanej) porady](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) dotyczącej bezpieczeństwa w przypadku wykrywania oszustw.
  
Oto kilka innych linków, które mogą pomóc:
  
- [Jak firma Microsoft używa struktury zasad dotyczących nadawców (SPF) w celu zapobiegania fałszowania](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurowanie spf w celu zapobiegania fałszerszem](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
