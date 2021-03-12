---
title: Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań myśliwnych
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749544"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Stosowanie najlepszych rozwiązań dla zaawansowanych zapytań myśliwnych

Aby szybciej uzyskać wyniki i uniknąć limitów czasu podczas uruchamiania złożonych zapytań, zastosuj następujące najlepsze rozwiązania:

- Podczas próby nowych zapytań zawsze używaj limitu, aby uniknąć uzyskiwania bardzo dużych zestawów wyników. Ponadto skorzystaj z tej funkcji, aby dokonać wstępnej `count` oceny rozmiaru zestawu wyników.
- Najpierw użyj filtrów czasu. Najlepiej jest ograniczyć kwerendy do siedmiu dni.
- Na początku zapytania, zaraz po filtrze czasu, dodaj filtry oczekiwane do usunięcia większości danych.
- Gdy szukasz pełnych tokenów, `has` użyj operatora, a nie `contains` .
- Wyszukiwanie należy uruchomić dla określonej kolumny, a nie we wszystkich kolumnach.
- Podczas łączenia tabel najpierw określ tabelę z mniejszą liczbą wierszy.
- `project` tylko niezbędne kolumny z tabel, do których zostały sprzężenia.

Aby dowiedzieć się więcej, zobacz Najlepsze rozwiązania [dla zapytania wyszukiwania zaawansowanego.](https://go.microsoft.com/fwlink/?linkid=2144812)
