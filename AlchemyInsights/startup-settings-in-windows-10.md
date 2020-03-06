---
title: Ustawienia uruchamiania w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409235"
---
# <a name="startup-settings-in-windows-10"></a>Ustawienia uruchamiania w systemie Windows 10

**Zmienianie aplikacji uruchamianych automatycznie podczas uruchamiania**

1. Przejdź do [ustawienia > aplikacji > uruchamiania](ms-settings:startupapps?activationSource=GetHelp).

2. Upewnij się, że każda aplikacja, którą chcesz uruchomić podczas uruchamiania, jest **włączona**.

**Dodawanie aplikacji do automatycznego uruchamiania podczas uruchamiania**

1. Kliknij lub naciśnij **pozycję Start** i znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.

2. Kliknij prawym przyciskiem myszy aplikację, kliknij polecenie **Więcej**, a następnie kliknij polecenie **Otwórz lokalizację pliku**. Spowoduje to otwarcie lokalizacji, w której jest zapisywany skrót do aplikacji. Jeśli nie ma opcji Otwórz lokalizację pliku, oznacza to, że aplikacja nie może działać podczas uruchamiania.

3. Po otwarciu lokalizacji pliku naciśnij **klawisz logo systemu Windows + R**, wpisz **powłokę:startup,** a następnie kliknij przycisk **OK**. Spowoduje to otwarcie folderu Startup.

4. Skopiuj i wklej skrót do aplikacji z lokalizacji pliku do folderu Startup.

**Zaawansowane opcje uruchamiania (w tym tryb awaryjny, ustawienia UEFI i uruchamianie z innego urządzenia)**

1. Zapisz swoją pracę i zamknij wszystkie otwarte dokumenty, ponieważ te kroki uruchomią ponownie komputer.

2. Przejdź do [ustawienia > aktualizacja & odzyskiwania > zabezpieczeń](ms-settings:recovery?activationSource=GetHelp).

3. W obszarze **Uruchamianie zaawansowane**kliknij pozycję **Uruchom ponownie teraz**. 

4. Po ponownym uruchomieniu komputera na ekranie opcji Wybierz:

    - Aby uruchomić komputer taki jak dysk USB, kliknij **pozycję Użyj urządzenia**.

    - Aby wprowadzić ustawienia INTERFEJSU UEFI (czasami nazywane konfiguracją systemu BIOS), kliknij pozycję **Rozwiązywanie problemów > zaawansowane opcje > ustawienia oprogramowania układowego UEFI**. 

    - Aby przejść do trybu awaryjnego lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję **Rozwiązywanie problemów > zaawansowane opcje > ustawienia uruchamiania**, a następnie kliknij przycisk **Uruchom ponownie**. Może zostać wyświetlony monit o wprowadzenie [klucza odzyskiwania funkcji BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.