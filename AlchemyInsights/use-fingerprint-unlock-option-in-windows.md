---
title: Korzystanie z opcji odblokowania odcisków palców w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588325"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Korzystanie z opcji odblokowania odcisków palców w systemie Windows 10

**Włączanie odcisku palca funkcji Windows Hello**

Aby odblokować system Windows 10 za pomocą odcisku palca, musisz skonfigurować odcisk palca Windows Hello, dodając (pozwalając systemowi Windows nauczyć się rozpoznawać) co najmniej jednym palcem. 

1. Przejdź do **pozycji Ustawienia > konta > opcje logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)). Zostaną wyświetlone dostępne opcje logowania. Na przykład:

    ![Opcje logowania.](media/sign-in-options.png)

2. Kliknij lub naciśnij pozycję **Odcisk palca Funkcji Rozpoznawania systemu Windows**, a następnie kliknij pozycję **Konfiguruj**. W oknie konfiguracji funkcji Windows Hello kliknij pozycję **Wprowadzenie**. Czujnik odcisków palców zostanie aktywowany, a ty zostaniesz poproszony o umieszczenie palca na czujniku:

   ![Linii papilarnych.](media/fingerprint-sensor.png)

3. Postępuj zgodnie z instrukcjami, które proszą o wielokrotne skanowanie palca. Po zakończeniu tej opcji możesz dodać inne palce, których możesz użyć do logowania. Następnym razem, gdy zalogujesz się do systemu Windows 10, będziesz mieć możliwość użycia odcisku palca.

**Windows Hello Fingerprint nie jest dostępny jako opcja logowania**

Jeśli odcisk palca Windows Hello nie jest wyświetlany jako opcja w **opcjach logowania,** oznacza to, że system Windows nie jest świadomy czytnika linii papilarnych / skanera podłączonego do komputera lub że zasady systemowe uniemożliwiają jego użycie (jeśli na przykład komputer jest zarządzany przez miejsce pracy). Aby rozwiązać problem: 

1. Wybierz przycisk **Start** na pasku zadań i wyszukaj **pozycję Menedżer urządzeń**.

2. Kliknij lub naciśnij, aby otworzyć **menedżera urządzeń**.

3. W Menedżerze urządzeń rozwiń urządzenia biometryczne, klikając jego szewron.

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. Skaner linii papilarnych powinien być wymieniony jako urządzenie biometryczne, takie jak skaner Synaptics WBDI:

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. Jeśli skaner linii papilarnych nie jest wyświetlany, a skaner jest zintegrowany z komputerem, przejdź do witryny producenta komputera w sieci Web. W sekcji pomocy technicznej dla modelu komputera wyszukaj sterownik systemu Windows 10 dla skanera, który można zainstalować.

6. Jeśli skaner jest oddzielony od komputera (podłączonego przez USB), przejdź do witryny producenta skanera w sieci Web, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia systemu Windows 10 dla posiadanej modelu skanera.
