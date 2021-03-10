---
title: Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań łowiecki
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696088"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań łowiecki

Aby szybciej uzyskać wyniki i uniknąć limitów czasu podczas uruchamiania złożonych zapytań, zastosuj poniższe najlepsze rozwiązania:

- Podczas próby nowych zapytań zawsze używaj limitu, aby uniknąć bardzo dużych zestawów wyników. Ponadto skorzystaj `count` z tej funkcji, aby dokonać wstępnej oceny rozmiaru zestawu wyników.
- Najpierw użyj filtrów czasu. Najlepiej jest ograniczyć kwerendy do siedmiu dni.
- Na początku zapytania, zaraz po filtrze czasu, dodaj filtry, które mają usunąć większość danych.
- Gdy szukasz pełnych tokenów, użyj `has` operatora, a nie `contains` .
- Uruchom wyszukiwanie dla określonej kolumny, a nie we wszystkich kolumnach.
- Podczas dołączania do tabel najpierw określ tabelę z mniejszą liczbą wierszy.
- `project` tylko niezbędne kolumny z tabel, które zostały sprzężenia.

Aby dowiedzieć się więcej, zobacz najlepsze rozwiązania [dotyczące zapytań wyszukiwania zaawansowanego.](https://go.microsoft.com/fwlink/?linkid=2144812)
