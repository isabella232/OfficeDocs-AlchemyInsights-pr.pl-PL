---
title: Rozwiązywanie problemów-wskazówka bezpieczeństwa dla wykrywania oszustw sprawdza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533205"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Rozwiązywanie problemów-wskazówka bezpieczeństwa dla wykrywania oszustw sprawdza

Jeśli jesteś coraz wskazówka bezpieczeństwa, który mówi, "nadawca nie powiodło się nasze kontroli wykrywania nadużyć finansowych i nie może być kto wydają się być", a następnie nadawca nie można przekazać DKIM lub SPF uwierzytelniające. Najlepszym sposobem rozwiązania tego problemu jest dla nadawcy do autoryzowania sami. Jeśli nadawca wysyła w Twoim imieniu, musisz autoryzować ich przez dodanie adresu IP nadawcy do rekordu SPF.
  
Aby uzyskać więcej informacji, zobacz [Rozwiązywanie problemów-wskazówka czerwony bezpieczeństwa (podejrzane) dla wykrywania oszustw sprawdza](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Oto niektóre łącza, które mogą pomóc:
  
- [Jak Office 365 używa struktury zasad dotyczących nadawców (SPF), aby zapobiec podszywaniu](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Konfigurowanie funkcji SPF w usłudze Office 365 w celu zapobiegania fałszowaniu](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
