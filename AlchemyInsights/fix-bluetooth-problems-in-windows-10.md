---
title: Rozwiązywanie problemów z Bluetooth w systemie Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730169"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a>Rozwiązywanie problemów z Bluetooth w systemie Windows 10

Jeśli brakuje ikony Bluetooth lub nie można włączyć lub wyłączyć protokołu Bluetooth, może być konieczne uruchomienie narzędzia do rozwiązywania problemów z funkcją Bluetooth. [Otwórz ustawienia rozwiązywania problemów](ms-settings:troubleshoot), kliknij pozycję **Bluetooth** w obszarze **Znajdź i Rozwiąż inne problemy**, kliknij pozycję **Uruchom narzędzie do rozwiązywania problemów**.

Jeśli nie widzisz ikony Bluetooth, ale protokół Bluetooth jest wyświetlany w Menedżerze urządzeń:

1. W Menedżerze urządzeń kliknij pozycję **Bluetooth**. Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) nazwę karty Bluetooth i kliknij pozycję **Odinstaluj urządzenie**.

2. Zamknij urządzenie z systemem Windows, poczekaj kilka sekund, a następnie włącz je ponownie. System Windows podejmie próbę ponownego zainstalowania sterownika.

Jeśli ostatnio zainstalowano aktualizacje systemu Windows 10 lub uaktualniono do systemu Windows 10, warto sprawdzić dostępność aktualizacji sterowników:

1. W Menedżerze urządzeń kliknij pozycję **Bluetooth**, a następnie kliknij nazwę karty Bluetooth (która może zawierać wyraz "Radio").

2. Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) kartę Bluetooth, a następnie kliknij pozycję **Aktualizuj**  >  **Wyszukiwanie sterowników automatycznie, aby uzyskać zaktualizowane oprogramowanie sterownika**. Postępuj zgodnie z instrukcjami, a następnie kliknij przycisk **Zamknij**.

      - Jeśli system Windows nie może znaleźć nowego sterownika Bluetooth, odwiedź witrynę internetową producenta komputera i Pobierz z niego najnowszą wersję sterownika Bluetooth.

    - Po pobraniu pliku kliknij pozycję **Aktualizuj sterownik**  >  **Przeglądaj mój komputer w poszukiwaniu oprogramowania sterownika**  >  **Wyszukaj** lokalizację, w której są przechowywane pliki sterowników, > **OK**  >  **Next**, a następnie postępuj zgodnie z instrukcjami instalacji.

3. Po zainstalowaniu zaktualizowanego sterownika Uruchom ponownie komputer, a następnie sprawdź, czy rozwiązanie problemu z połączeniem jest rozwiązywane.

Aby uzyskać więcej informacji na temat rozwiązywania problemów z funkcją Bluetooth, zobacz pełny artykuł [Rozwiązywanie problemów z Bluetooth w systemie Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).
