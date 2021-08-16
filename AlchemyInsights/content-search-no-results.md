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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058012"
---
# <a name="no-results-from-content-searchexports"></a>Brak wyników wyszukiwania/eksportu zawartości

Problemy z wyszukiwaniem/eksportem zawartości, które nie zwracają żadnych danych, mogą być spowodowane pewnym filtrem zabezpieczeń zgodności, który został określony przez określonego administratora i nie jest przekazywania go wszystkim administratorom.

Aby rozwiązać ten problem, sprawdź, czy istnieją filtry zabezpieczeń zgodności, które mogą być przyczyną tego problemu:
1. Połączenie do Centrum zabezpieczeń i zgodności w programie PowerShell
2. Uruchom następujące polecenia:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter — Organizacja $org