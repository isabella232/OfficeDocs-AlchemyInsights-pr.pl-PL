---
title: Korzystanie z witryny sieci Web firmy Wix z zakupionymi lub zarządzanymi domenami usługi Office 365
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708496"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korzystanie z witryny sieci Web firmy Wix z zakupionymi lub zarządzanymi domenami usługi Office 365

- [Aktualizowanie rekordów DNS w celu zachowania witryny sieci Web u bieżącego dostawcy usług hostingowych](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Artykuł Wix "Łączenie domeny z siecią Wix przy użyciu metody wskazywania" zaleca używanie wskazywania (dodawanie rekordów DNS na powyższe łącze) zamiast zmieniania serwerów nazw podczas korzystania z usługi Office 365
- Jeśli nadal zdecydujesz się zmienić serwery nazw na Wix, musisz [utworzyć rekordy DNS w Wix for Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Jeśli domena została zakupiona od firmy Microsoft, nie można zmienić serwerów nazw. Jeśli musisz zmienić nazwy serwerów, zakupiona przez firmę Microsoft domena musiałaby zostać [przeniesiona do innego dostawcy hostingu po 60 dniach](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)