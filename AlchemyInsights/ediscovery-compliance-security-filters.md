---
title: Podczas przeszukiwania/eksportowania zawartości nie są zwracane żadne wyniki
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101276"
---
# <a name="no-results-returned-during-content-searchexport"></a>Podczas przeszukiwania/eksportowania zawartości nie są zwracane żadne wyniki

Jeśli występują problemy z następującymi scenariuszami zbierania elektronicznych materiałów dowodowych:

- Wyszukiwanie/eksportowanie zawartości nie zwraca żadnych danych ani nieoczekiwanych danych
- Wyszukiwanie zbierania elektronicznych materiałów dowodowych lub eksportowanie kończy się niepowodzeniem

Może to być spowodowane niektórymi filtrami zabezpieczeń zgodności, które zostały skonfigurować przez określonego administratora i nie zostały przekazane wszystkim administratorom.

Aby rozwiązać ten problem, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą powodować następujące problemy:

1. Połączenie do Centrum zabezpieczeń i zgodności w programie PowerShell
2. Uruchom następujące polecenia:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Aby uzyskać dodatkowe informacje na temat filtrów zabezpieczeń zgodności, zobacz [Filtrowanie uprawnień dla wyszukiwania zawartości.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
