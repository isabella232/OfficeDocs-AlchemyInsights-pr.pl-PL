---
title: Rozwiązywanie problemów z dźwiękiem w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: f51fd233db5ae068e719f1cf3bc94a0dac82444f
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265026"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>Rozwiązywanie problemów z dźwiękiem w systemie Windows 10

**Uruchamianie narzędzia do rozwiązywania problemów z dźwiękiem**

1.  Otwórz [ustawienia rozwiązywania problemów](ms-settings:troubleshoot).

2.  Wybierz **pozycję Odtwarzanie dźwięku** > **Uruchom narzędzie do rozwiązywania problemów**.

**Ustawianie urządzenia domyślnego**

Jeśli łączysz się z urządzeniem audio za pomocą pamięci USB lub HDMI, może być konieczne ustawienie tego urządzenia jako domyślnego:

1. Otwórz**dźwięk** **startowy,** > a następnie **wybierz** dźwięk lub zmień **dźwięki systemu** z listy wyników.

2.  Na karcie **Odtwarzanie** wybierz urządzenie, wybierz pozycję **Ustaw domyślne**, a następnie wybierz **przycisk OK**.

**Sprawdź kable, głośność, głośniki i słuchawki**

1. Sprawdź, czy w przypadku luźnych kabli nie ma połączenia głośnika i słuchawek, a następnie upewnij się, że są podłączone do właściwego gniazda.

2. Sprawdź poziom mocy i głośności i spróbuj podkręcać wszystkie elementy sterujące głośnością.

3. Niektóre głośniki i aplikacje mają własne regulatory głośności; być może trzeba będzie sprawdzić je wszystkie, aby upewnić się, że są na odpowiednim poziomie.

4. Spróbuj połączyć się za pomocą innego portu USB.

**Uwaga:** Pamiętaj, że głośniki mogą nie działać, gdy słuchawki są podłączone.

**Sprawdź Menedżera urządzeń**

Aby upewnić się, że sterowniki są aktualne:

1. Wybierz **pozycję Start**, wpisz Menedżera **urządzeń**, a następnie wybierz pozycję Menedżer **urządzeń** z listy wyników.

2. W obszarze **Kontrolery dźwięku, wideo i gier**wybierz kartę dźwiękową, otwórz ją, wybierz kartę **Sterownik** i wybierz pozycję **Aktualizuj sterownik**.

**Uwaga:** Jeśli system Windows nie znajdzie nowego sterownika, poszukaj go w witrynie sieci Web producenta urządzenia i postępuj zgodnie z jego instrukcjami.

**Ponowne instalowanie sterownika**

Jeśli nie możesz zaktualizować za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie producenta w sieci Web, spróbuj wykonać następujące czynności:

1. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) sterownik audio, a następnie wybierz polecenie **Odinstaluj**. Uruchom ponownie urządzenie, a system Windows podejmie próbę ponownej instalacji sterownika.

2. Jeśli ponowna instalacja sterownika nie działa, spróbuj użyć ogólnego sterownika audio, który jest dostarczany z systemem Windows. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) sterownik audio > **Aktualizuj oprogramowanie** > sterownika**Przeglądaj mój komputer w celu uzyskania oprogramowania** > sterownika**Pozwól mi wybrać z listy sterowników urządzeń na moim komputerze,** wybierz **opcję High Definition Audio Device**, wybierz **dalej**i postępuj zgodnie z instrukcjami, aby go zainstalować.
