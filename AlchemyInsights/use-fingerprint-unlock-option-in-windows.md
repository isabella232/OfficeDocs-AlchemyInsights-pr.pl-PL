---
title: Używanie opcji odblokowywania odcisku palca w systemie Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795254"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Używanie opcji odblokowywania odcisku palca w systemie Windows 10

**Włączanie odcisku palca Windows Hello**

Aby odblokować system Windows 10 przy użyciu odcisku palca, musisz skonfigurować odcisk cyfrowy funkcji Windows Hello, dodając (pozwalając systemowi Windows na rozpoznanie) co najmniej jednego palca. 

1. Przejdź do obszaru **ustawienia > konta > opcji logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)). Zostaną wyświetlone dostępne opcje logowania. Przykład:

    ![Opcje logowania.](media/sign-in-options.png)

2. Kliknij lub naciśnij pozycję **odciskiem palca Windows Hello**, a następnie kliknij pozycję **Konfiguruj**. W oknie Konfiguracja usługi Windows Hello kliknij pozycję **Rozpocznij**. Czujnik linii papilarnych zostanie aktywowany, a użytkownik zostanie poproszony o umieszczenie palca na czujniku:

   ![Czujnik odcisku palca.](media/fingerprint-sensor.png)

3. Postępuj zgodnie z instrukcjami, co spowoduje wyświetlenie monitu o powtarzanie skanowania palca. Po zakończeniu tej opcji będziesz mieć możliwość dodawania innych palców, których możesz użyć do logowania się. Gdy następnym razem zalogujesz się do systemu Windows 10, będziesz mieć możliwość skorzystania z odcisku palca.

**Odcisk palca Windows Hello niedostępny jako opcja logowania**

Jeśli odcisk palca funkcji Windows Hello nie jest widoczny jako opcja w **opcjach logowania**, oznacza to, że system Windows nie rozpoznaje żadnego czytnika linii papilarnych ani skanera podłączonego do komputera lub zasady systemowe uniemożliwiają korzystanie z nich (Jeśli na przykład komputer jest zarządzany przez miejsce pracy). Aby rozwiązać problem: 

1. Wybierz przycisk **Start** na pasku zadań i Wyszukaj pozycję **Menedżer urządzeń**.

2. Kliknij lub naciśnij, aby otworzyć **Menedżera urządzeń**.

3. W Menedżerze urządzeń rozwiń węzeł Urządzenia biometryczne, klikając jego Pagon.

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. Skaner linii papilarnych powinien być wymieniony na urządzeniu biometrycznym, na przykład w skanerze Synaptics WBDI:

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. Jeśli skaner linii papilarnych nie jest widoczny, a skaner jest zintegrowany z komputerem, przejdź do witryny producenta komputera w sieci Web. W sekcji Pomoc techniczna dotycząca modelu komputerów Wyszukaj sterownik systemu Windows 10, aby skaner mógł zostać zainstalowany.

6. Jeśli skaner jest niezależny od komputera (dołączonego za pośrednictwem magistrali USB), przejdź do witryny producenta skanera w sieci Web, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia w systemie Windows 10 dla modelu skanera.
