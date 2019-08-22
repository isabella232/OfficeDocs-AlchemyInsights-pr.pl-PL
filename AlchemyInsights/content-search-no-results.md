---
title: Nie wyników wyszukiwania zawartości
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516789"
---
# <a name="no-results-from-content-searchexports"></a>Brak wyników z zawartości wyszukiwania/wywozu

Problemy z zawartości wyszukiwania/wywozu nie zwróciła żadnych danych może być spowodowane niektórych zgodności filtr zabezpieczeń, który został skonfigurowany przez administratora konkretnego i nie komunikuje się wszyscy administratorzy.

Aby rozwiązać ten problem, sprawdź, czy są wszystkie filtry zabezpieczeń zgodności, która może być przyczyną tego:
1. Podłącz do bezpieczeństwa i środowiska Powershell Centrum zgodności
2. Uruchom następujące aplety poleceń środowiska:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizacja $org