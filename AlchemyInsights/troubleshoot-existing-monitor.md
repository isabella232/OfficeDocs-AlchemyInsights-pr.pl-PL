---
title: Rozwiązywanie problemów z istniejącym monitorem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690721"
---
# <a name="troubleshoot-an-existing-monitor"></a>Rozwiązywanie problemów z istniejącym monitorem

Wypróbuj te rozwiązania, aby rozwiązać problem z monitorem. 

**Odśwież ekran monitora:**

Naciśnij następujące klawisze w tym samym czasie: klawisz Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji za pomocą sterownika graficznego. Twoje monitory będą migać, a po kilku sekundach rozpocznie się odtwarzanie.

**Rozwiązywanie problemów ze sprzętem monitora:**

1. Odłącz kabel łączący komputer z monitorem i podłącz go ponownie.
2. Odłączanie wszelkich nieistotnych urządzeń z komputera (takich jak karty lub stacje dokujące).

**Jeśli niedawno zainstalowano aktualizację na komputerze PC, możesz wycofać sterownik ekranu:**

1. Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z wyników.
2. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, ands wybierz pozycję **Właściwości**.
3. Przejdź do karty **Sterownik** i wybierz pozycję **Przywróć sterownik**. <br>
Uwaga: Jeśli ta funkcja jest niedostępna lub jest wyszarzona, wybierz pozycję **nie** z poniższych opcji, aby przejść do następnego kroku.
4. Aby zmiany zostały wprowadzone, może być konieczne ponowne uruchomienie komputera.

**Odinstaluj i ponownie zainstaluj sterownik ekranu:**

1. Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z wyników.
2. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, ands wybierz pozycję **Odinstaluj urządzenie**. 
3. Zaznacz pole wyboru obok pozycji **Usuń oprogramowanie sterownika dla tego urządzenia** i wybierz pozycję **Odinstaluj**.<br>
Uwaga: może zostać wyświetlony monit o ponowne uruchomienie komputera na tym etapie. Przed ponownym uruchomieniem upewnij się, że Zanotuj pozostałe instrukcje.
4. Ponownie otwórz Menedżera urządzeń.
5. Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, a następnie wybierz polecenie **Aktualizuj sterownik**.
6. Wybierz pozycję **Wyszukaj automatycznie w celu zaktualizowania oprogramowania sterownika** i postępuj zgodnie z instrukcjami instalacji.