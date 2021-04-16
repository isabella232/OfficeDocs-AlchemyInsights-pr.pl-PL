---
title: Nie można otworzyć dwukrotnego kliknięcia pliku pakietu Office
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
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814815"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Nie można otworzyć dwukrotnego kliknięcia pliku pakietu Office

Po dwukrotnym kliknięciu pliku pakietu Office może zostać wyświetlony otwarty program, ale sam plik nie zostanie otwarty. Może też zostać wyświetlany komunikat o błędzie: "Wystąpił problem podczas wysyłania polecenia do programu". Przyczyn jest wiele, ale dwa najczęściej spotykane rozwiązania są takie:

- W programie Excel upewnij się, że opcja DDE nie jest zaznaczona. Tę opcję można znaleźć, tworząc nowy skoroszyt, a następnie wybierając pozycję Plik **> opcje > zaawansowane.** W sekcji **Ogólne** wyczyść pole wyboru Ignoruj inne aplikacje, które korzystają z dynamicznej wymiany danych **(DDE, Dynamic Data Exchange).**

- Uruchom naprawę online, aby przywrócić ustawienia domyślne. Kliknij przycisk Start systemu Windows i wyszukaj pozycję "Panel sterowania". Otwórz Panel **sterowania**, a następnie przejdź do **a programs > Programs and Features**. Następnie kliknij prawym przyciskiem myszy **pozycję Microsoft Office [Wersja]** i wybierz pozycję **Zmień > Naprawa online.**

Jeśli żadne z tych rozwiązań nie działa, bardziej kompletną listę rozwiązań można znaleźć w artykule pomocy technicznej. Dwukrotne kliknięcie pliku pakietu Office nie powiedzie się, [aby go otworzyć.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)
