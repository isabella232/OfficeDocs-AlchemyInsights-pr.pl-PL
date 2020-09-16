---
title: Rozwiązywanie problemów z dźwiękiem w systemie Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750321"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Rozwiązywanie problemów z dźwiękiem w systemie Windows 10

**Uruchamianie narzędzia do rozwiązywania problemów z dźwiękiem**

1.  Otwórz [Ustawienia rozwiązywania problemów](ms-settings:troubleshoot).

2.  Wybieranie opcji **odtwarzania audio**  >  **Uruchom narzędzie do rozwiązywania problemów**.

**Ustawianie urządzenia domyślnego**

Jeśli łączysz się z urządzeniem audio przy użyciu magistrali USB lub HDMI, być może trzeba ustawić to urządzenie jako domyślne:

1. Otwórz **Start**  >  **dźwięk**Start, a następnie wybierz pozycję **dźwięk** lub **Zmień dźwięki systemowe** z listy wyników.

2.  Na karcie **odtwarzanie** wybierz urządzenie, wybierz pozycję **Ustaw domyślne**, a następnie wybierz **przycisk OK**.

**Sprawdzanie kabli, głośności, głośników i słuchawek**

1. Sprawdź połączenia głośników i słuchawek, aby uzyskać kable i upewnić się, że są podłączone do właściwego złącza.

2. Sprawdź poziomy zasilania i głośności, a następnie spróbuj wyłączyć regulatory głośności.

3. Niektóre głośniki i aplikacje mają własne regulatory głośności; może być konieczne sprawdzenie wszystkich, aby upewnić się, że są na odpowiednim poziomie.

4. Spróbuj połączyć się przy użyciu innego portu USB.

**Uwaga**: Pamiętaj, że głośniki mogą nie działać po podłączeniu słuchawek.

**Sprawdzanie Menedżera urządzeń**

Aby upewnić się, że sterowniki są aktualne:

1. Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z listy wyników.

2. W obszarze **Kontrolery dźwięku, wideo i gier**wybierz kartę dźwiękową, otwórz ją, wybierz kartę **Sterownik** i wybierz pozycję **Aktualizuj sterownik**.

**Uwaga**: Jeśli system Windows nie znajdzie nowego sterownika, poszukaj go w witrynie internetowej producenta urządzenia i postępuj zgodnie z instrukcjami.

**Ponowne instalowanie sterownika**

Jeśli nie możesz zaktualizować się za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie internetowej producenta, spróbuj wykonać następujące czynności:

1. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, a następnie wybierz pozycję **Odinstaluj**. Uruchom ponownie urządzenie, a system Windows podejmie próbę ponownego zainstalowania sterownika.

2. Jeśli ponowna instalacja sterownika nie zadziała, spróbuj użyć uniwersalnego sterownika audio, który jest dostarczany z systemem Windows. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, > **Aktualizuj oprogramowanie sterownika**  >  **Przeglądaj mój komputer w poszukiwaniu oprogramowania sterownika**  >  **umożliwia mi wybieranie z listy sterowników urządzeń na komputerze**, wybieranie **urządzenia audio High Definition**, wybieranie **pozycji dalej**i postępuj zgodnie z instrukcjami, aby go zainstalować.
