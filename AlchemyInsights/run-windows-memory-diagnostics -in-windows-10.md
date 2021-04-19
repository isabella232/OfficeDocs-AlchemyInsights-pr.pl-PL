---
title: Uruchamianie Diagnostyki pamięci systemu Windows w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826677"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Uruchamianie Diagnostyki pamięci systemu Windows w systemie Windows 10

Jeśli system Windows i aplikacje na komputerze ulega awarii, zawieszają się lub działają niestabilnie, może wystąpić problem z pamięcią RAM komputera. Możesz uruchomić Narzędzie Diagnostyka pamięci systemu Windows, aby sprawdzić, czy nie występują problemy z pamięcią RAM komputera.

W polu wyszukiwania na pasku zadań wpisz diagnostykę pamięci **,** a następnie wybierz pozycję **Diagnostyka pamięci systemu Windows**. 

Aby uruchomić diagnostykę, komputer musi zostać uruchomiony ponownie. Masz możliwość natychmiastowego ponownego uruchomienia (zapisz najpierw swoją pracę i zamknij otwarte dokumenty i wiadomości e-mail) lub zaplanuj automatyczne uruchamianie diagnostyczne przy następnym ponownym uruchomieniu komputera:

![Diagnostyka pamięci systemu Windows](media/windows-memory-diagnostic.png)

Po ponownym uruchomieniu komputera narzędzie **Diagnostyka pamięci** systemu Windows zostanie uruchomione automatycznie. Stan i postęp będą wyświetlane jako diagnostyka, a Ty możesz anulować diagnostykę, naciskając klawisz **ESC** na klawiaturze.

Po zakończeniu diagnostyki system Windows zacznie normalnie.
Natychmiast po ponownym uruchomieniu, gdy zostanie wyświetlony pulpit, zostanie wyświetlone powiadomienie (obok ikony Centrum akcji na pasku zadań) wskazujące, czy zostały znalezione błędy pamięci.  Przykład:

Oto ikona Centrum akcji: ![Ikona Centrum akcji](media/action-center-icon.png) 

Oraz przykładowe powiadomienie: ![Brak błędów pamięci](media/no-memory-errors.png)

Jeśli przegapisz powiadomienie, możesz  wybrać ikonę Centrum akcji na  pasku zadań, aby wyświetlić Centrum akcji i wyświetlać przewijaną listę powiadomień.

Aby przejrzeć szczegółowe informacje, wpisz **zdarzenie** w polu wyszukiwania na pasku zadań, a następnie wybierz pozycję **Podgląd zdarzeń**. W **okienku podglądu** zdarzeń po lewej stronie przejdź do okna Dzienniki **systemu Windows > systemu**. W okienku po prawej stronie zeskanuj  listę w dół, patrząc na kolumnę Źródło, aż zobaczysz zdarzenia z wartością źródłową **MemoryDiagnostics-Results.** Wyróżnij każde takie zdarzenie i wyświetl informacje o wynikach w polu pod **kartą** Ogólne poniżej listy.
