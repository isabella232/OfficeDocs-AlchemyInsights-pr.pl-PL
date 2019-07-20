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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800506"
---
# <a name="no-results-from-content-searchexports"></a>Brak wyników z zawartości wyszukiwania/wywozu

Problemy z zawartości wyszukiwania/wywozu nie zwróciła żadnych danych może być spowodowane niektórych zgodności filtr zabezpieczeń, który został skonfigurowany przez administratora konkretnego i nie komunikuje się wszyscy administratorzy.

Aby rozwiązać ten problem, sprawdź, czy są wszystkie filtry zabezpieczeń zgodności, która może być przyczyną tego:
1. Podłącz do bezpieczeństwa i środowiska Powershell Centrum zgodności
2. Uruchom następujące aplety poleceń środowiska:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizacja $org