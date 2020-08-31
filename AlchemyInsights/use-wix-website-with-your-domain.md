---
title: Używanie witryny sieci Web WIX z zakupionymi lub zarządzanymi domenami pakietu Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300726"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Używanie witryny sieci Web WIX z zakupionymi lub zarządzanymi domenami pakietu Office 365

- [Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u bieżącego dostawcy hostingu](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- WIX artykuł "łączenie domeny z WIX za pomocą metody wskazywania" zalecane używanie funkcji wskazywania (Dodawanie rekordów DNS na powyższym łączu) zamiast zmieniania serwerów nazw podczas korzystania z pakietu Office 365
- Jeśli nadal chcesz zmienić serwery nazw na WIX, konieczne będzie [utworzenie rekordów DNS w witrynie WIX dla firmy Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide) .
- Jeśli Twoja domena została zakupiona w firmie Microsoft, nie można zmienić serwerów nazw. Jeśli trzeba zmienić serwery nazw, zakupiona domena firmy Microsoft musi zostać  [przeniesiona do innego dostawcy hostingu po upływie 60 dni](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)