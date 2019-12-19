---
title: Rozwiązywanie problemów z istniejącym monitorem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738578"
---
# <a name="troubleshoot-an-existing-monitor"></a>Rozwiązywanie problemów z istniejącym monitorem

Wypróbuj te rozwiązania, aby rozwiązać problem z monitorem. 

**Odśwież ekran monitora:**

Naciśnij jednocześnie następujące przyciski: klucz systemu Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji ze sterownikiem graficznym. Monitory będą migać chwilowo i wrócić po kilku sekundach.

**Rozwiązywanie problemów ze sprzętem monitora:**

1. Odłącz przewód łączący komputer z monitorem i podłącz go ponownie.
2. Odłącz wszystkie urządzenia inne niż istotne z komputera (takie jak karty lub stacje dokujące).

**Jeśli niedawno zainstalowano aktualizację na komputerze, można wycofać sterownik ekranu:**

1. Wybierz **Start**, wpisz **Menedżer urządzeń**i wybierz **Menedżer urządzeń** z wyników.
2. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną, a następnie wybierz polecenie **Właściwości**.
3. Przejdź do zakładki **Sterownik** i wybierz **Przywróć sterownik**. <br>
Uwaga: Jeśli ta opcja nie jest dostępna lub jest wyszarzona, wybierz opcję **nie** z poniższych opcji, aby przejść do kolejnego kroku.
4. Zanim zmiany zostaną uwzględnione, może być konieczne ponowne uruchomienie komputera.

**Odinstaluj i ponownie zainstaluj sterownik ekranu:**

1. Wybierz **Start**, wpisz **Menedżer urządzeń**i wybierz **Menedżer urządzeń** z wyników.
2. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną, a następnie wybierz pozycję **Odinstaluj urządzenie**. 
3. Zaznacz pole wyboru obok opcji **Usuń oprogramowanie sterownika dla tego urządzenia** i wybierz opcję **Odinstaluj**.<br>
Uwaga: na tym etapie może zostać wyświetlony monit o ponowne uruchomienie komputera. Pamiętaj, aby zapisać pozostałe instrukcje przed ponownym uruchomieniem.
4. Ponownie otwórz Menedżera urządzeń.
5. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną i wybierz polecenie **Aktualizuj sterownik**.
6. Wybierz opcję **Wyszukaj automatycznie, aby zaktualizować oprogramowanie sterownika** i postępuj zgodnie z instrukcjami instalacji.