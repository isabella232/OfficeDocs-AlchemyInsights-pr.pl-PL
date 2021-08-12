---
title: Rozwiązywanie problemów z porada dotycząca bezpieczeństwa wykrywania oszustw
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955976"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rozwiązywanie problemów z porada dotycząca bezpieczeństwa wykrywania oszustw

Jeśli jest wyświetlany kod porada dotycząca bezpieczeństwa o treści "Nadawca nie sprawdzał oszustw i może nie być tym, kim są", oznacza to, że nadawca nie przejdzie testów uwierzytelniania DKIM lub SPF. Najlepszą metodą rozwiązania tego problemu jest autoryzacja siebie przez nadawcę. Jeśli nadawca wysyła w Twoim imieniu, musisz autoryzować go, dodając adres IP nadawcy do Twojego rekordu SPF.
  
Aby uzyskać więcej informacji, zobacz Rozwiązywanie problemów z [czerwonym (podejrzanym) porada dotycząca bezpieczeństwa wykrywania](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) oszustw.
  
Oto kilka innych linków, które mogą pomóc:
  
- [Jak firma Microsoft używa struktury zasad dotyczących nadawców (SPF) w celu zapobiegania fałszowania](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurowanie spf w celu zapobiegania fałszerszem](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
