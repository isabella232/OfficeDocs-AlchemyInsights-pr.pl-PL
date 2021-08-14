---
title: W systemie Windows 10 brakuje ikony zasilania lub baterii
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
- "9002953"
- "5655"
ms.openlocfilehash: 82d41844de1eafdf7e0cc38f91416f3b71868e3d5d1b3eb8be0f10abd701ddc8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973331"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>W systemie Windows 10 brakuje ikony zasilania lub baterii

Jeśli Twoje urządzenie z systemem Windows 10 ma baterię (np. laptop lub tablet albo komputer podłączony przez USB do zasilacza awaryjnego), zwykle ikona zasilania/baterii jest wyświetlana na pasku zadań obok zegara, na przykład:

![Ikona baterii](media/battery-icon.png)

Jeśli ta ikona nie jest wyświetlana, może być ukryta:

1. Przejdź do pozycji **[Ustawienia > Personalizacji > Pasek zadań](ms-settings:taskbar?activationSource=GetHelp)**.

2. W obszarze powiadomień kliknij pozycję **Wybierz ikony, które będą wyświetlane na pasku zadań**.

3. Następnie znajdź na liście element **Zasilanie** i przełącz jego ustawienie na wartość **Wł.**.

    ![Pokazywanie ikony zasilania na pasku zadań](media/power-icon-on.png)

**Rozwiązywanie problemów**

Jeśli po wykonaniu powyższych instrukcji przełącznik **Zasilanie** jest wyszarzony lub niewidoczny, w polu wyszukiwania na pasku zadań wpisz **menedżer urządzeń**, a następnie na liście wyników wybierz pozycję **Menedżer urządzeń**. W obszarze **Baterie** kliknij prawym przyciskiem myszy baterię urządzenia, kliknij pozycję **Wyłącz**, a następnie kliknij pozycję **Tak**. Poczekaj kilka sekund, a następnie kliknij prawym przyciskiem myszy baterię i kliknij pozycję **Włącz**. Następnie ponownie uruchom urządzenie.

Jeśli po wykonaniu powyższych instrukcji ikona baterii nie jest wyświetlana na pasku zadań, w polu wyszukiwania na pasku zadań wpisz **menedżer zadań**, a następnie na liście wyników kliknij pozycję **Menedżer zadań**. Na karcie **Procesy** w obszarze **Nazwa** kliknij prawym przyciskiem myszy pozycję **Eksplorator**, a następnie kliknij pozycję **Uruchom ponownie**.
