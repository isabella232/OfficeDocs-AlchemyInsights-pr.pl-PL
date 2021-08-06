---
title: Uruchom Windows diagnostyki pamięci w Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922581"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Uruchom Windows diagnostyki pamięci w Windows 10

Jeśli Windows i aplikacje na komputerze pc ulegają awarii, zawieszają się lub działają niestabilnie, może wystąpić problem z pamięcią RAM komputera. Możesz uruchomić narzędzie diagnostyki Windows, aby sprawdzić, czy nie występują problemy z pamięcią RAM komputera.

W polu wyszukiwania na pasku zadań wpisz **diagnostykę** pamięci , a następnie wybierz pozycję Windows **Diagnostyka pamięci**. 

Aby uruchomić diagnostykę, komputer musi zostać uruchomiony ponownie. Masz możliwość natychmiastowego ponownego uruchomienia (zapisz najpierw swoją pracę i zamknij otwarte dokumenty i wiadomości e-mail) lub zaplanuj automatyczne uruchamianie diagnostyczne przy następnym ponownym uruchomieniu komputera:

![Windows Diagnostyka pamięci](media/windows-memory-diagnostic.png)

Po ponownym uruchomieniu komputera zostanie **automatycznie Windows Diagnostyka** pamięci. Stan i postęp będą wyświetlane jako diagnostyka, a Ty możesz anulować diagnostykę, naciskając klawisz **ESC** na klawiaturze.

Po zakończeniu diagnostyki Windows zacznie się normalnie.
Natychmiast po ponownym uruchomieniu, gdy zostanie wyświetlony pulpit, zostanie wyświetlone powiadomienie (obok ikony Centrum akcji na pasku zadań) wskazujące, czy zostały znalezione błędy pamięci.  Przykład:

Oto ikona Centrum akcji: ![Ikona Centrum akcji](media/action-center-icon.png) 

Oraz przykładowe powiadomienie: ![Brak błędów pamięci](media/no-memory-errors.png)

Jeśli przegapisz powiadomienie, możesz  wybrać ikonę Centrum akcji na  pasku zadań, aby wyświetlić Centrum akcji i wyświetlać przewijaną listę powiadomień.

Aby przejrzeć szczegółowe informacje, wpisz **zdarzenie** w polu wyszukiwania na pasku zadań, a następnie wybierz pozycję **Podgląd zdarzeń**. W **okienku podglądu** zdarzeń (po lewej stronie) przejdź do Windows **Logs > System**. W okienku po prawej stronie zeskanuj  listę w dół, patrząc na kolumnę Źródło, aż zobaczysz zdarzenia z wartością źródłową **MemoryDiagnostics-Results.** Wyróżnij każde takie zdarzenie i wyświetl informacje o wynikach w polu pod **kartą** Ogólne poniżej listy.
