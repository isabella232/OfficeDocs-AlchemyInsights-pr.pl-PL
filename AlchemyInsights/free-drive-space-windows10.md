---
title: Zwalnianie miejsca na dysku w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928091"
---
# <a name="free-up-drive-space-in-windows-10"></a>Zwalnianie miejsca na dysku w systemie Windows 10

Oto dwie metody zwalniania miejsca na dysku w systemie Windows:

- Zwalnianie miejsca na dysku w systemie Windows 10
- Zwolnij miejsce na aktualizacje systemu Windows 10 za pomocą zewnętrznego urządzenia pamięci masowej.

Jeśli po użyciu narzędzia Oczyszczanie dysku nadal masz mało miejsca na dysku, możliwe, że folder Temp szybko zapełnia się plikami aplikacji (.appx) używanymi przez Microsoft Store. Aby rozwiązać ten problem, zresetuj sklep Microsoft Store, wyczyść jego pamięć podręczną, a następnie uruchom narzędzie do rozwiązywania problemów usługi Windows Update. Przed wykonaniem tych czynności upewnij się, że sklep Microsoft Store jest zamknięty.

**Krok 1. Resetowanie sklepu Microsoft Store**

**Uwaga** Spowoduje to trwałe usunięcie danych aplikacji z urządzenia, w tym preferencji i danych logowania.

1. Wybierz pozycję **Start** > **Ustawienia** > **Aplikacje** > **Aplikacje i funkcje**.

1. Na liście aplikacji znajdź i wybierz sklep Microsoft Store.

1. Wybierz **Opcje zaawansowane**.

1. Przewiń w dół i wybierz **Resetowanie**, a następnie **Potwierdź resetowanie**.

**Krok 2. Wyczyść pamięć podręczną sklepu Microsoft Store**

1. Naciśnij klawisze logo Windows+R, aby otworzyć okno dialogowe Uruchamianie.

1. Wpisz wsreset.exe i wybierz **OK**.

1. Otwarte zostanie puste okno wiersza poleceń. Po upływie około 10 sekund okno zostanie zamknięte, a sklep zostanie automatycznie otwarty.

**Krok 3. Resetowanie usługi Windows Update**

1. Wybierz **Start** > **Ustawienia** > **Aktualizacja i zabezpieczenia** > **Rozwiązywanie problemów**.

1. Przewiń w dół i wybierz **Windows Update** z listy, a następnie wybierz pozycję **Uruchom narzędzie do rozwiązywania problemów**.

1. Uruchom ponownie komputer i sprawdź, czy problem nadal występuje.

