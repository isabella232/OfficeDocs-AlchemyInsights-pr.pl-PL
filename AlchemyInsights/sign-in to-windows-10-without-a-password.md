---
title: Logowanie w celu Windows 10 bez użycia hasła
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107529"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logowanie w celu Windows 10 bez użycia hasła

Aby uniknąć konieczności wpisywania hasła podczas Windows, zalecamy użycie jednej z opcji bezpiecznego logowania usługi Windows Hello, takich jak numer PIN, rozpoznawanie twarzy lub odcisk palca, jeśli są dostępne. Jeśli naprawdę chcesz wyłączyć bezpieczne logowanie, zobacz poniższe instrukcje "Automatyczne logowanie Windows 10 logowania".

**Zabezpieczanie Windows Hello alternatywnego hasła do konta**

Przejdź do **Ustawienia > Konta > opcje** logowania (lub kliknij [tutaj).](ms-settings:signinoptions?activationSource=GetHelp) Zostaną wyświetlone dostępne opcje logowania. Przykład:

![Opcje logowania.](media/sign-in-options.png)

Kliknij lub naciśnij jedną z opcji, aby ją skonfigurować. Przy następnym uruchomieniu lub Windows będzie można używać nowej opcji zamiast hasła. 

**Automatyczne logowanie się do Windows 10**

**Uwaga:** Automatyczne logowanie jest wygodne, ale wprowadza zagrożenie bezpieczeństwa, zwłaszcza jeśli Twój komputer jest dostępny dla wielu osób. 

1. Kliknij lub naciśnij przycisk **Start** na pasku zadań.

2. Wpisz **netplwiz** i naciśnij klawisz Enter, aby otworzyć okno Konta użytkowników.

3. W **ustawieniach** Konta użytkowników kliknij konto, na które chcesz automatycznie się zalogować Windows konta.

4. Wyczyść pole wyboru "Użytkownicy muszą wprowadzić nazwę użytkownika i hasło, aby korzystać z tego komputera".

    ![Użytkownicy muszą wprowadzić opcję nazwy użytkownika i hasła.](media/users-must-enter-username.png)

5. Kliknij przycisk **OK**. Zostaniesz poproszony(-a) o wprowadzenie i potwierdzenie hasła wybranego konta. Kliknij **przycisk OK,** aby zakończyć. Po następnym Windows 10 się ono automatycznie zaloguje do wybranego konta.
