---
title: Pomoc w ustawieniu wyświetlania wyświetlania nocnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404668"
---
# <a name="help-with-the-night-light-display-setting"></a>Pomoc w ustawieniu wyświetlania wyświetlania nocnego

Aby dowiedzieć się więcej o ustawieniach wyświetlania nocnego, zobacz Ustawianie czasu wyświetlania nocnego w [systemie Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Jeśli opcje wyświetlania nocnego są wyszarowane w ustawieniach, sprawdź sterownik ekranu: 

1. Kliknij pole wyszukiwania na pasku zadań i wpisz **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach wyszukiwania.
1. Rozwiń **kartę graficzną**. 

Niestety, funkcja wyświetlania nocnego nie jest dostępna, jeśli w urządzeniu jest używany sterownik DisplayLink lub sterownik Ekranu podstawowego.

Funkcja wyświetlania nocnego korzysta z najnowszej technologii graficznej, więc może być konieczne zaktualizowanie sterownika ekranu:  

- Sprawdź aktualizacje, przechodząc do menu **Start**  >  **Settings**  >  **Update & Security** Windows  >    >  **UpdateS sprawdzaj aktualizacje.**  

LUB

- Aby ręcznie pobrać i zainstalować najnowsze sterowniki ekranu, odwiedź witrynę internetową pomocy technicznej producenta sprzętu.

## <a name="reset-night-light-in-the-registry"></a>Resetowanie nocnego światła w rejestrze

Jeśli aktualizacja sterownika ekranu nie działa, może być konieczne zresetowanie wyświetlania nocnego w rejestrze.  

**Przestroga:** Ten krok rozwiązywania problemów jest zalecany tylko dla użytkowników zaawansowanych. Niepoprawne zmodyfikowanie rejestru może być związane z poważnych problemami. Aby uzyskać dodatkową ochronę, przed zmodyfikowaniem rejestru należy utworzyć jego kopię zapasową, aby można było przywrócić go w przypadku wystąpienia problemów.

1. W polu wyszukiwania wpisz **regedit**, a następnie wybierz pozycję **Edytor rejestru** w wynikach wyszukiwania.

1. Przejdź do następującego klucza rejestru: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Eksportuj, a następnie usuń następujący podklucz:$$windows.data.bluelightreduction.bluelightreductionstate

1. Wyeksportuj, a następnie usuń następujący podklucz:$$windows.data.bluelightreduction.settings

1. Uruchom ponownie system Windows i sprawdź, czy są dostępne opcje światła nocnego.


