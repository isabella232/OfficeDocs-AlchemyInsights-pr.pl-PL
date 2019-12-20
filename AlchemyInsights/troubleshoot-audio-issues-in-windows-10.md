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
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796283"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Rozwiązywanie problemów z dźwiękiem w systemie Windows 10

**Uruchom narzędzie do rozwiązywania problemów z dźwiękiem**

Narzędzie do rozwiązywania problemów z dźwiękiem może automatycznie naprawiać problemy z dźwiękiem: 

1. Wybierz **Start**, wpisz **Rozwiązywanie problemów**, a następnie wybierz **Rozwiązywanie problemów** z listy wyników. 
2. Wybierz opcję **odtwarzanie dźwięku** > **Uruchom narzędzie do rozwiązywania problemów**.

**Sprawdź przewody, głośność, głośniki i słuchawki**

- Sprawdź połączenia głośników i słuchawek, aby poluzować przewody i upewnij się, że są podłączone do odpowiedniego gniazda.
- Sprawdź poziom mocy i głośności, a następnie spróbuj wyłączyć wszystkie regulatory głośności.
- Niektóre głośniki i aplikacje mają własne regulatory głośności, a może trzeba sprawdzić je wszystkie, aby upewnić się, że są na właściwym poziomie.
- Spróbuj połączyć się przy użyciu innego portu USB.
- **Uwaga:** Pamiętaj, że głośniki mogą nie działać, gdy podłączone są słuchawki.

**Sprawdzanie Menedżera urządzeń**

Aby upewnić się, że sterowniki są aktualne:

- Wybierz pozycję **Start**, wpisz **Menedżer urządzeń**, a następnie z listy wyników wybierz pozycję **Menedżer urządzeń** .

2. W obszarze **Kontrolery dźwięku, wideo i gier**wybierz kartę dźwiękową, otwórz ją, wybierz kartę **Sterownik** i wybierz pozycję **Aktualizuj sterownik**. 

**Uwaga:** Jeśli system Windows nie znajdzie nowego sterownika, poszukaj go w witrynie sieci Web producenta urządzenia i postępuj zgodnie z instrukcjami.

**Ponowna instalacja sterownika**

Jeśli nie można zaktualizować za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie sieci Web producenta, spróbuj wykonać następujące czynności: 

1. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, a następnie wybierz pozycję **Odinstaluj**. Uruchom ponownie urządzenie, a system Windows spróbuje ponownie zainstalować sterownik.

2. Jeśli ponowna instalacja sterownika nie działa, spróbuj użyć ogólnego sterownika audio, który jest dostarczany z systemem Windows. W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio > **Aktualizuj oprogramowanie** > **sterownika Przeglądaj mój komputer w poszukiwaniu oprogramowania** > sterownika**pozwól mi wybrać z listy sterowników urządzeń na moim komputerze**, wybierz **urządzenie audio High Definition**, wybierz **dalej**i postępuj zgodnie z instrukcjami, aby go zainstalować.

**Ustawianie domyślnego urządzenia**

Jeśli łączysz się z urządzeniem audio za pomocą USB lub HDMI, może być konieczne ustawienie tego urządzenia jako domyślnego: 

1. Wybierz **Start**, wpisz **dźwięk**, a następnie wybierz **dźwięk** lub **Zmień dźwięki systemu** z listy wyników.

2. Na karcie **odtwarzanie** wybierz urządzenie, wybierz opcję **Ustaw domyślne**, a następnie wybierz **przycisk OK**.

