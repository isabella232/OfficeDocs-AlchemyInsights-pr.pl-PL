---
title: Wolne miejsce na dysku w systemie Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037955"
---
# <a name="free-up-drive-space-in-windows-10"></a>Wolne miejsce na dysku w systemie Windows 10

Oto dwie opcje, które można zrobić, aby uwolnić miejsce na dysku w systemie Windows:

- Uwolnij miejsce na dysku w systemie Windows 10.
- Uwolnij miejsce na aktualizacje systemu Windows 10 za pomocą zewnętrznego urządzenia magazynującego.

Jeśli po użyciu funkcji Oczyszczanie dysku nadal masz mało miejsca na dysku, możliwe, że folder Temp szybko wypełnia pliki aplikacji (appx) używane w Sklepie Microsoft. Aby rozwiązać ten problem, zresetuj Sklep, wyczyść pamięć podręczną Sklepu, a następnie uruchom narzędzie do rozwiązywania problemów z usługą Windows Update. Przed kontynuowaniem tej procedury upewnij się, że Sklep Microsoft jest zamknięty.

**Krok 1. Resetowanie Sklepu Microsoft**

**Uwaga** Spowoduje to trwałe usunięcie danych aplikacji na urządzeniu, w tym Twoich preferencji i szczegółów logowania.

1. Wybierz **pozycję Start**  >  **Ustawienia**  >  **Aplikacje**&  >  **funkcje**.

1. Na liście aplikacji znajdź i wybierz pozycję Microsoft Store.

1. Wybierz **pozycję Opcje zaawansowane.**

1. Przewiń w dół i **wybierz pozycję Resetuj**, a następnie **Potwierdź resetowanie**.

**Krok 2. Wyczyszczenie pamięci podręcznej Microsoft Store**

1. Naciśnij klawisze logo Windows + R, aby otworzyć okno dialogowe Uruchamianie.

1. Wpisz wsreset.exe i wybierz przycisk **OK.**

1. Zostanie otwarte puste okno wiersza polecenia. Po upływie około 10 sekund okno zostaje zamknięte, a Sklep jest otwierany automatycznie.

**Krok 3. Resetowanie usługi Windows Update**

1. Wybierz **pozycję Uruchom**  >    >  **aktualizację ustawień i & rozwiązywanie problemów z**  >  **zabezpieczeniami.**

1. Przewiń w dół i wybierz z listy usługę **Windows Update,** a następnie **wybierz pozycję Uruchom narzędzie do rozwiązywania problemów**.

1. Uruchom ponownie komputer i sprawdź, czy problem nadal występuje.

