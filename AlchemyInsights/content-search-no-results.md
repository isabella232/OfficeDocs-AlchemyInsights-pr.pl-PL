---
title: Brak wyników wyszukiwania zawartości
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816858"
---
# <a name="no-results-from-content-searchexports"></a>Brak wyników wyszukiwania/eksportu zawartości

Problemy z wyszukiwaniem/eksportem zawartości, które nie zwracają żadnych danych, mogą być spowodowane pewnym filtrem zabezpieczeń zgodności, który został określony przez określonego administratora i nie jest przekazywania go wszystkim administratorom.

Aby rozwiązać ten problem, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą być przyczyną tego problemu:
1. Nawiązywanie połączenia z Centrum zabezpieczeń i zgodności w programie PowerShell
2. Uruchom następujące polecenia:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter — Organizacja $org