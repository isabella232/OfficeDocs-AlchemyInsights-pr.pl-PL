---
title: Ustawienia uruchamiania w Windows 10
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
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909836"
---
# <a name="startup-settings-in-windows-10"></a>Ustawienia uruchamiania w Windows 10

**Zmienianie aplikacji uruchomionych automatycznie podczas uruchamiania**

1. Przejdź do [Ustawienia > Uruchamianie >.](ms-settings:startupapps?activationSource=GetHelp)

2. Upewnij się, że każda aplikacja, która ma być uruchamiana podczas uruchamiania, jest **włączona.**

**Dodawanie aplikacji, która będzie uruchamiana automatycznie przy uruchamianiu**

1. Kliknij lub naciśnij **przycisk Start** i znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.

2. Kliknij aplikację prawym przyciskiem myszy, kliknij pozycję **Więcej**, a następnie kliknij **pozycję Otwórz lokalizację pliku**. Spowoduje to otwarcie lokalizacji, w której został zapisany skrót do aplikacji. Jeśli nie ma opcji Otwórz lokalizację pliku, oznacza to, że aplikacja nie może być uruchamiana podczas uruchamiania.

3. Po otwarciu lokalizacji pliku naciśnij klawisze **logo Windows + R,** wpisz **shell:startup,** a następnie kliknij przycisk **OK.** Zostanie otwarty folder Autostart.

4. Skopiuj skrót do aplikacji i wklej go z lokalizacji pliku do folderu Autostart.

**Zaawansowane opcje uruchamiania (w tym tryb Sejf, ustawienia UEFI i rozruch z innego urządzenia)**

1. Zapisz pracę i zamknij wszystkie otwarte dokumenty, ponieważ spowoduje to ponowne uruchomienie komputera.

2. Przejdź do [Ustawienia > & odzyskiwania > zabezpieczeń.](ms-settings:recovery?activationSource=GetHelp)

3. W **obszarze Uruchamianie zaawansowane** kliknij pozycję Uruchom ponownie **teraz.** 

4. Po ponownym uruchomieniu komputera i wybraniu ekranu Wybierz opcję:

    - Aby uruchomić komputer z urządzenia, takiego jak dysk USB, kliknij **pozycję Użyj urządzenia**.

    - Aby wprowadzić ustawienia UEFI (czasami nazywane konfiguracją INTERFEJSU), kliknij pozycję Rozwiązywanie problemów z > opcjami zaawansowanymi > oprogramowania układowego **UEFI Ustawienia.** 

    - Aby wejść Sejf uruchamiania lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję Rozwiązywanie problemów > zaawansowane opcje **> Uruchamianie Ustawienia**, a następnie kliknij pozycję Uruchom **ponownie.** Może pojawić się monit o wprowadzenie klucza [odzyskiwania funkcji BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.