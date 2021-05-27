---
title: Rozwiązywanie problemów zbierania elektronicznych materiałów dowodowych zawiera błędy
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676278"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Rozwiązywanie problemów zbierania elektronicznych materiałów dowodowych zawiera błędy

Występują problemy z zbierania elektronicznych materiałów dowodowych? Oto kilka najlepszych rozwiązań do rozważenia:

- Sprawdź stan dystrybucji wstrzymaj.  Jeśli stan jest **Wł. (Oczekiwanie)** lub Wyłączony **(oczekiwanie),** poczekaj na zakończenie rozpowszechniania wstrzymywania.
- Scal aktualizacje zbierania elektronicznych materiałów dowodowych w jedno żądanie zbiorcze, zamiast wielokrotnie aktualizować zasady dla każdej transakcji.
- Uruchom Set-CaseHoldPolicy <policyname> -RetryDistribution w programie PowerShell Centrum zabezpieczeń i zgodności. Aby uzyskać szczegółowe informacje, [Połączenie się z Centrum zabezpieczeń & w programie PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Aby uzyskać instrukcje dotyczące sprawdzania tych ustawień i dodatkowych najlepszych rozwiązań związanych z ograniczaniem i rozwiązywaniem problemów dotyczących zbierania elektronicznych materiałów dowodowych, zobacz Rozwiązywanie problemów z błędami blokady zbierania [elektronicznych materiałów dowodowych.](/microsoft-365/compliance/hold-distribution-errors)
Aby uzyskać informacje na temat rozwiązywania innych typowych problemów zbierania elektronicznych materiałów dowodowych, zobacz Badanie, rozwiązywanie i rozwiązywanie typowych problemów [zbierania elektronicznych materiałów dowodowych.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
