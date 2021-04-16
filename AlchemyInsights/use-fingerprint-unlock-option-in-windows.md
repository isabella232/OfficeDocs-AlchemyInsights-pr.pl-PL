---
title: Korzystanie z opcji odblokowywania za pomocą linii papilarnych w systemie Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796687"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Korzystanie z opcji odblokowywania za pomocą linii papilarnych w systemie Windows 10

**Włącz funkcję Windows Hello Fingerprint**

Aby odblokować system Windows 10 przy użyciu linii papilarnych, musisz skonfigurować rozpoznawanie linii papilarnych przez dodanie co najmniej jednego palca (pozwalając systemowi Windows nauczyć się jego rozpoznawania). 

1. Przejdź do **ustawień > Konta > opcje** logowania (lub kliknij [tutaj).](ms-settings:signinoptions?activationSource=GetHelp) Zostaną wyświetlone dostępne opcje logowania. Przykład:

    ![Opcje logowania.](media/sign-in-options.png)

2. Kliknij lub naciśnij pozycję **Linii papilarnych funkcji Windows Hello**, a następnie kliknij pozycję **Skonfiguruj**. W oknie konfiguracji funkcji Windows Hello kliknij pozycję **Wprowadzenie**. Czujnik linii papilarnych zostanie aktywowany i zostaniesz poproszony o włodenie palca do czujnika:

   ![Czujnik linii papilarnych.](media/fingerprint-sensor.png)

3. Postępuj zgodnie z instrukcjami, które będą zawierały prośbę o wielokrotne skanowanie palcem. Po zakończeniu będziesz mieć możliwość dodawania innych palców, których możesz używać do logowania się. Następnym razem, gdy zalogujesz się do systemu Windows 10, będzie można użyć odcisku palca w tym celu.

**Funkcja Windows Hello Fingerprint nie jest dostępna jako opcja logowania**

Jeśli funkcja Windows Hello Fingerprint nie jest wyświetlana jako opcja w opcjach **logowania,** oznacza to, że system Windows nie zna czytnika/skanera linii papilarnych dołączonych do komputera lub że zasady systemowe uniemożliwiają ich użycie (jeśli na przykład Twój komputer jest zarządzany przez Twoje miejsce pracy). Aby rozwiązać problemy: 

1. Wybierz przycisk **Start** na pasku zadań i wyszukaj menedżer **urządzeń**.

2. Kliknij lub naciśnij, aby **otworzyć Menedżera urządzeń.**

3. W Menedżerze urządzeń rozwiń pozycję Biometryczne urządzenia, klikając jej link.

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. Twój skaner linii papilarnych powinien być wymieniony jako urządzenie biometryczne, takie jak skaner WBDItics:

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. Jeśli twój skaner linii papilarnych nie jest widoczny, a skaner jest zintegrowany z komputerem, przejdź do witryny internetowej producenta komputera. W sekcji pomocy technicznej dotyczącej modelu komputera wyszukaj sterownik systemu Windows 10, który możesz zainstalować.

6. Jeśli skaner jest oddzielony od komputera (podłączony przez USB), przejdź do witryny internetowej producenta skanera, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia z systemem Windows 10 dla posiadaowego modelu skanera.
