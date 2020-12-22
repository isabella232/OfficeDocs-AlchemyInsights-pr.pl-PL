---
title: W trakcie wyszukiwania i eksportowania zawartości nie są zwracane żadne wyniki
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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727233"
---
# <a name="no-results-returned-during-content-searchexport"></a>W trakcie wyszukiwania i eksportowania zawartości nie są zwracane żadne wyniki

Jeśli występują problemy z następującymi scenariuszami zbierania elektronicznych materiałów dowodowych:

- Funkcja wyszukiwania zawartości/eksportowania nie zwraca żadnych danych lub nieoczekiwanych danych
- Błąd wyszukiwania lub eksportu zbierania elektronicznych materiałów dowodowych

Może to być spowodowane pewnymi filtrami zabezpieczeń zgodności, które zostały skonfigurowane przez określonego administratora i nie są przekazywane do wszystkich administratorów.

Aby to naprawić, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą powodować następujące problemy:

1. Nawiązywanie połączenia z programem PowerShell w centrum zabezpieczeń i zgodności
2. Uruchom następujące commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Aby uzyskać dodatkowe informacje na temat filtrów zabezpieczeń zgodności, zobacz [filtrowanie uprawnień do wyszukiwania zawartości](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
