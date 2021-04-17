---
title: Rozwiązywanie problemów z istniejącym monitorem
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824589"
---
# <a name="troubleshoot-an-existing-monitor"></a>Rozwiązywanie problemów z istniejącym monitorem

Wypróbuj poniższe rozwiązania, aby rozwiązać problemy z monitorem. 

**Odświeżanie ekranu monitora:**

Naciśnij jednocześnie następujące klawisze: klawisz systemu Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji ze sterownikem graficznym. Monitory będą migać chwilę i odwrócić po upływie kilku sekund.

**Rozwiązywanie problemów ze sprzętem monitorów:**

1. Odłącz kabel od podłączania komputera do monitora i podłącz go z powrotem.
2. Odłącz od komputera wszystkie nieistnikowe urządzenia (takie jak adaptery lub stacje dokujące).

**Jeśli niedawno na komputerze została zainstalowana aktualizacja, możesz wycofać sterownik ekranu:**

1. Wybierz **pozycję Start**, wpisz menedżer **urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach.
2. Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Właściwości.**
3. Przejdź do karty **Sterownik i** wybierz pozycję **Przywróć sterownik.** <br>
Uwaga: Jeśli ta opcja jest niedostępne lub jest wyszarzona, wybierz pozycję **Nie** z poniższych opcji, aby przejść do następnego kroku.
4. Zanim te zmiany zajdą w życie, może być konieczne ponowne uruchomienie komputera.

**Odinstaluj i ponownie zainstaluj sterownik ekranu:**

1. Wybierz **pozycję Start**, wpisz menedżer **urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach.
2. Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Odinstaluj urządzenie**. 
3. Zaznacz pole wyboru Usuń oprogramowanie sterownika **dla tego urządzenia** i wybierz pozycję Odinstaluj . <br>
Uwaga: na tym etapie może pojawić się monit o ponowne uruchomienie komputera. Przed ponownym uruchomieniem zapisz pozostałe instrukcje.
4. Otwórz ponownie Menedżera urządzeń.
5. Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Aktualizuj sterownik**.
6. Wybierz **pozycję Wyszukaj automatycznie, aby zaktualizować oprogramowanie sterownika** i postępuj zgodnie z instrukcjami instalacji.