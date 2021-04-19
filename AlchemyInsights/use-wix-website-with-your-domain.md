---
title: Korzystanie z witryny internetowej Wix z domenami kupionymi lub zarządzanymi przez usługę Office 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825957"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korzystanie z witryny internetowej Wix z domenami kupionymi lub zarządzanymi przez usługę Office 365

- [Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u obecnego dostawcy hostingu](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix article "Connecting a Domain to Wix Using the Pointing Method" recommending using pointing (dodawanie rekordów DNS za pomocą powyższego linku), zamiast zmieniać serwery nazw podczas korzystania z usługi Office 365
- Jeśli mimo to zdecydujesz się na zmianę serwerów nazw na Wix, konieczne będzie utworzenie rekordów  [DNS w witrynie Wix dla firmy Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Jeśli domena została zakupiona od firmy Microsoft, nie można zmienić serwerów nazw. Jeśli po upływie [60](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host) dni musisz zmienić serwery nazw, do których kupiono domenę firmy Microsoft, należy przetransferować usługę do innego dostawcy hostingu