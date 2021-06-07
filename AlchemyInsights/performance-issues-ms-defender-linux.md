---
title: Problemy z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794002"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemy z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux

Ten artykuł przeprowadzi Cię przez kolejne etapy identyfikowania problemów z wydajnością programu Microsoft Defender dla punktu końcowego w systemie Linux.

Najpierw należy sprawdzić, czy problem, który występuje, został rozwiązany za pomocą [najnowszej wersji](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Aby rozpocząć badanie, zobacz Rozwiązywanie problemów z wydajnością [programu Microsoft Defender dla punktu końcowego w systemie Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Wykluczenia

Wykluczenia mogą pomóc zminimalizować problemy z wydajnością. Przed rozpoczęciem przejrzyj swoje wykluczenia, aby sprawdzić i udokumentować wszelkie dodatkowe zagrożenia.

Aby uzyskać więcej informacji, zobacz Konfigurowanie i weryfikowanie wykluczeń programu [Microsoft Defender dla punktu końcowego w systemie Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Jeśli masz wiele plików, & wykluczyć, a wszystkie są w tym samym punkcie instalacji, łatwiej będzie wykluczyć punkt instalacji. Od lutego w wersji 101.22.80 można wykluczyć cały punkt instalacji.

Jeśli na przykład /mnt/backup jest punktem instalacji, możesz dodać polecenie /mnt/backup do listy wykluczeń, uruchamiając to polecenie:

`$ mdatp exclusion folder add –path /mnt/backup`

**Uwaga:** Dodanie wykluczeń zwiększa ryzyko, że złośliwe oprogramowanie nie jest wykrywane, a jego obsługa i wdrożenie należy zachować ostrożność.

## <a name="need-help"></a>Potrzebujesz pomocy?

Aby pomóc w najskuteczniejszy sposób, zbierz dane diagnostyczne przed otwarciem sprawy pomocy technicznej.
