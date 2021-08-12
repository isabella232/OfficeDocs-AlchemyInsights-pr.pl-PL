---
title: Dwukrotne kliknięcie pliku Office nie może go otworzyć
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
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965111"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Dwukrotne kliknięcie pliku Office nie może go otworzyć

Dwukrotne kliknięcie pliku Office może spowodować otwarcie programu, ale sam plik nie zostanie otwarty. Może też zostać wyświetlany komunikat o błędzie: "Wystąpił problem podczas wysyłania polecenia do programu". Przyczyn jest wiele, ale dwa najczęściej spotykane rozwiązania są takie:

- Z poziomu Excel upewnij się, że opcja DDE nie jest zaznaczona. Tę opcję można znaleźć, tworząc nowy skoroszyt, a następnie wybierając pozycję Plik **> opcje > zaawansowane.** W sekcji **Ogólne** wyczyść pole wyboru Ignoruj inne aplikacje, które używają Exchange **danych dynamicznych (DDE).**

- Uruchom naprawę online, aby przywrócić ustawienia domyślne. Kliknij przycisk Windows Start i wyszukaj pozycję "Panel sterowania". Otwórz Panel **sterowania**, a następnie przejdź do **a programs > Programs and Features**. Następnie kliknij prawym przyciskiem myszy **pozycję Microsoft Office [Wersja]** i wybierz pozycję **Zmień > Naprawa online.**

Jeśli żadne z tych rozwiązań nie działa, bardziej kompletną listę rozwiązań można znaleźć w artykule pomocy technicznej. Dwukrotne kliknięcie pliku Office nie powiedzie się jego [otwarcie.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
