---
title: Logowanie się do systemu Windows 10 bez użycia hasła
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830556"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logowanie się do systemu Windows 10 bez użycia hasła

Aby uniknąć konieczności wpisywania hasła podczas uruchamiania systemu Windows, zalecamy używanie jednej z opcji bezpiecznego logowania funkcji Windows Hello, na przykład numeru PIN, rozpoznawania twarzy lub odcisku palca, jeśli są dostępne. Jeśli naprawdę chcesz wyłączyć bezpieczne logowanie, zobacz poniższe instrukcje "Automatyczne logowanie się do systemu Windows 10".

**Zabezpieczanie alternatyw funkcji Windows Hello dla hasła do konta**

Przejdź do **ustawień > Konta > opcje** logowania (lub kliknij [tutaj).](ms-settings:signinoptions?activationSource=GetHelp) Zostaną wyświetlone dostępne opcje logowania. Przykład:

![Opcje logowania.](media/sign-in-options.png)

Kliknij lub naciśnij jedną z opcji, aby ją skonfigurować. Po następnym uruchomieniu lub odblokowaniu systemu Windows będzie można używać nowej opcji zamiast hasła. 

**Automatyczne logowanie do systemu Windows 10**

**Uwaga:** Automatyczne logowanie jest wygodne, ale wprowadza zagrożenie bezpieczeństwa, zwłaszcza jeśli Twój komputer jest dostępny dla wielu osób. 

1. Kliknij lub naciśnij przycisk **Start** na pasku zadań.

2. Wpisz **netplwiz** i naciśnij klawisz Enter, aby otworzyć okno Konta użytkowników.

3. Na **stronie Konta** użytkowników kliknij konto, do którego chcesz automatycznie zalogować się podczas uruchamiania systemu Windows.

4. Wyczyść pole wyboru "Użytkownicy muszą wprowadzić nazwę użytkownika i hasło, aby korzystać z tego komputera".

    ![Użytkownicy muszą wprowadzić opcję nazwy użytkownika i hasła.](media/users-must-enter-username.png)

5. Kliknij przycisk **OK**. Zostaniesz poproszony(-a) o wprowadzenie i potwierdzenie hasła wybranego konta. Kliknij **przycisk OK,** aby zakończyć. Następnym razem, gdy system Windows 10 uruchomi się, automatycznie zaloguje się na wybrane konto.
