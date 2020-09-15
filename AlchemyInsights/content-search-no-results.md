---
title: Wyszukiwanie zawartości — Brak wyników
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680657"
---
# <a name="no-results-from-content-searchexports"></a>Brak wyników z wyszukiwania zawartości/eksportu

Problemy dotyczące wyszukiwania zawartości/eksportu, które nie zwracają żadnych danych, mogą być spowodowane pewnym filtrem zabezpieczeń zgodności, który został skonfigurowany przez określonego administratora i nie komunikuje go ze wszystkimi administratorami.

Aby temu zaradzić, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą powodować to:
1. Nawiązywanie połączenia z programem PowerShell w centrum zabezpieczeń i zgodności
2. Uruchom następujące commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org