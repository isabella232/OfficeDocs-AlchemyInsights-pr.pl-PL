---
title: Ustawienia uruchamiania w systemie Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751145"
---
# <a name="startup-settings-in-windows-10"></a>Ustawienia uruchamiania w systemie Windows 10

**Zmienianie aplikacji uruchamianych automatycznie podczas uruchamiania**

1. Przejdź do obszaru [ustawienia > aplikacje > uruchamiania](ms-settings:startupapps?activationSource=GetHelp).

2. Upewnij się, że wszystkie aplikacje, które chcesz uruchomić podczas uruchamiania, są **włączone.**

**Dodawanie aplikacji w celu automatycznego uruchamiania podczas uruchamiania**

1. Kliknij lub naciśnij pozycję **Rozpocznij** i Znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.

2. Kliknij prawym przyciskiem myszy aplikację, kliknij pozycję **więcej**, a następnie kliknij pozycję **Otwórz lokalizację pliku**. Spowoduje to otwarcie lokalizacji, w której zostanie zapisany skrót do aplikacji. Jeśli nie ma opcji otwierania lokalizacji pliku, oznacza to, że aplikacja nie będzie działać podczas uruchamiania.

3. Po otwarciu lokalizacji pliku naciśnij klawisze **logo Windows + R**, wpisz **powłokę: uruchamianie**, a następnie kliknij przycisk **OK**. Zostanie otwarty folder Autostart.

4. Skopiuj i Wklej skrót do aplikacji z lokalizacji pliku do folderu Autostart.

**Zaawansowane opcje uruchamiania (w tym tryb awaryjny, ustawienia UEFI i rozruch z innego urządzenia)**

1. Zapisz swoją pracę i Zamknij wszystkie otwarte dokumenty, ponieważ te czynności spowodują ponowne uruchomienie komputera.

2. Przejdź do obszaru [ustawienia > aktualizowanie & zabezpieczenia > odzyskiwanie](ms-settings:recovery?activationSource=GetHelp).

3. W obszarze **Uruchamianie zaawansowane**kliknij pozycję **Uruchom ponownie teraz**. 

4. Po ponownym uruchomieniu komputera na ekranie wybierz opcję:

    - Aby wykonać rozruch z urządzenia podobnego do dysku USB, kliknij pozycję **Użyj urządzenia**.

    - Aby wprowadzić ustawienia interfejsu UEFI (czasami nazywane konfiguracją systemu BIOS), kliknij pozycję **Rozwiązywanie problemów > opcje zaawansowane > ustawienia oprogramowania UEFI**. 

    - Aby wprowadzić tryb awaryjny lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję **Rozwiązywanie problemów > opcje zaawansowane > ustawienia uruchamiania**, a następnie kliknij pozycję **Uruchom ponownie**. Może zostać wyświetlony monit o wprowadzenie [klucza odzyskiwania funkcji BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.