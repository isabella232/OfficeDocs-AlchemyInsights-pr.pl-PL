---
title: Uruchamianie diagnostyki pamięci systemu Windows w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357786"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Uruchamianie diagnostyki pamięci systemu Windows w systemie Windows 10

Jeśli system Windows i aplikacje na komputerze ulegają awarii, zamrożeniu lub działają w niestabilny sposób, może to spowodować problem z pamięcią (RAM) komputera. Można uruchomić diagnostykę pamięci systemu Windows, aby sprawdzić, czy nie występują problemy z pamięcią RAM komputera.

W polu wyszukiwania na pasku zadań wpisz polecenie **Diagnostyka pamięci,** a następnie wybierz pozycję **Diagnostyka pamięci systemu Windows**. 

Aby uruchomić diagnostykę, komputer musi zostać ponownie uruchomiony. Możesz natychmiast ponownie uruchomić ponownie (zapisz najpierw swoje prace i zamknij otwarte dokumenty i wiadomości e-mail) lub zaplanuj automatyczne uruchomienie diagnostyki przy następnym ponownym uruchomieniu komputera:

![Diagnostyka pamięci systemu Windows](media/windows-memory-diagnostic.png)

Po ponownym uruchomieniu komputera **narzędzie diagnostyki pamięci systemu Windows** zostanie uruchomione automatycznie. Stan i postęp będą wyświetlane jako uruchomienie diagnostyki i masz możliwość anulowania diagnostyki, naciskając klawisz **ESC** na klawiaturze.

Po zakończeniu diagnostyki system Windows zostanie uruchomiony normalnie.
Natychmiast po ponownym uruchomieniu komputera zostanie wyświetlone powiadomienie (obok **ikony Centrum akcji** na pasku zadań), aby wskazać, czy zostały znalezione błędy pamięci. Przykład:

Oto ikona Centrum akcji: ![Ikona Centrum akcji](media/action-center-icon.png) 

I przykładowe powiadomienie: ![Brak błędów pamięci](media/no-memory-errors.png)

Jeśli powiadomienie nie zostanie odebrane, możesz wybrać ikonę **Centrum akcji** na pasku zadań, aby wyświetlić **Centrum akcji** i wyświetlić przewijaną listę powiadomień.

Aby przejrzeć szczegółowe informacje, wpisz **zdarzenie** w polu wyszukiwania na pasku zadań, a następnie wybierz pozycję **Podgląd zdarzeń**. W okienku po lewej **stronie Podglądu zdarzeń**przejdź do pozycji **Dzienniki systemu Windows > System**. W okienku po prawej stronie skanuj listę, patrząc na kolumnę **Źródło,** aż zobaczysz zdarzenia o wartości źródłowej **MemoryDiagnostics-Results**. Wyróżnij każde takie zdarzenie i zobacz informacje o wyniku w polu pod kartą **Ogólne** poniżej listy.
