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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930143"
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
