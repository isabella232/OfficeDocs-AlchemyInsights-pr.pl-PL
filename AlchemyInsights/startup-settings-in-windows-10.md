---
title: Ustawienia uruchamiania w systemie Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828162"
---
# <a name="startup-settings-in-windows-10"></a>Ustawienia uruchamiania w systemie Windows 10

**Zmienianie aplikacji uruchomionych automatycznie podczas uruchamiania**

1. Przejdź do [strony Ustawienia > Uruchamianie > uruchamianie.](ms-settings:startupapps?activationSource=GetHelp)

2. Upewnij się, że każda aplikacja, która ma być uruchamiana podczas uruchamiania, jest **włączona.**

**Dodawanie aplikacji, która będzie uruchamiana automatycznie przy uruchamianiu**

1. Kliknij lub naciśnij **przycisk Start** i znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.

2. Kliknij aplikację prawym przyciskiem myszy, kliknij pozycję **Więcej**, a następnie kliknij **pozycję Otwórz lokalizację pliku**. Spowoduje to otwarcie lokalizacji, w której został zapisany skrót do aplikacji. Jeśli nie ma opcji Otwórz lokalizację pliku, oznacza to, że aplikacja nie może być uruchamiana podczas uruchamiania.

3. Po otwarciu lokalizacji pliku naciśnij klawisze **logo Windows + R,** wpisz **shell:startup,** a następnie kliknij przycisk **OK.** Zostanie otwarty folder Autostart.

4. Skopiuj skrót do aplikacji i wklej go z lokalizacji pliku do folderu Autostart.

**Zaawansowane opcje uruchamiania (w tym tryb awaryjny, ustawienia UEFI i rozruch z innego urządzenia)**

1. Zapisz pracę i zamknij wszystkie otwarte dokumenty, ponieważ spowoduje to ponowne uruchomienie komputera.

2. Przejdź do [strony Ustawienia > i & w celu > zabezpieczeń.](ms-settings:recovery?activationSource=GetHelp)

3. W **obszarze Uruchamianie zaawansowane** kliknij pozycję Uruchom ponownie **teraz.** 

4. Po ponownym uruchomieniu komputera i wybraniu ekranu Wybierz opcję:

    - Aby uruchomić komputer z urządzenia, takiego jak dysk USB, kliknij **pozycję Użyj urządzenia**.

    - Aby wprowadzić ustawienia UEFI (czasami nazywane konfiguracją KARTO), kliknij pozycję Rozwiązywanie problemów z > zaawansowane opcje > ustawienia oprogramowania **układowego UEFI.** 

    - Aby wejść w tryb awaryjny lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję Rozwiązywanie problemów z > zaawansowane > Ustawienia **uruchamiania**, a następnie kliknij pozycję Uruchom **ponownie.** Może pojawić się monit o wprowadzenie klucza [odzyskiwania funkcji BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.