---
title: Logowanie się do systemu Windows 10 bez użycia hasła
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719963"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Logowanie się do systemu Windows 10 bez użycia hasła

Aby uniknąć konieczności wpisywania hasła podczas uruchamiania systemu Windows, zalecamy używanie jednej z bezpiecznych opcji logowania funkcji Windows Hello, takich jak kod PIN, rozpoznawanie twarzy lub odcisk cyfrowy, jeśli są one dostępne. Jeśli naprawdę chcesz wyłączyć bezpieczne logowanie, zobacz poniższe instrukcje "automatyczne logowanie do systemu Windows 10" poniżej.

**Zabezpieczanie hasła konta w usłudze Windows Hello**

Przejdź do obszaru **ustawienia > konta > opcji logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)). Zostaną wyświetlone dostępne opcje logowania. Przykład:

![Opcje logowania.](media/sign-in-options.png)

Kliknij lub naciśnij dowolną z opcji, aby ją skonfigurować. Gdy następnym razem uruchomisz lub odblokowuje system Windows, będziesz mieć możliwość skorzystania z opcji Nowy zamiast hasła. 

**Automatyczne logowanie w systemie Windows 10**

**Uwaga**: automatyczne logowanie jest wygodne, ale stanowi zagrożenie bezpieczeństwa, szczególnie wtedy, gdy komputer jest dostępny dla wielu osób. 

1. Kliknij lub naciśnij przycisk **Start** na pasku zadań.

2. Wpisz **netplwiz** i naciśnij klawisz ENTER, aby otworzyć okno konta użytkowników.

3. W obszarze **konta użytkowników**kliknij konto, z którym chcesz automatycznie logować się podczas uruchamiania systemu Windows.

4. Wyczyść pole wyboru "użytkownicy muszą wprowadzić nazwę użytkownika i hasło, aby używać tego komputera".

    ![Użytkownicy muszą wprowadzić odpowiednią nazwę użytkownika i hasło.](media/users-must-enter-username.png)

5. Kliknij przycisk **OK**. Zostanie wyświetlony monit o wprowadzenie i potwierdzenie hasła dla wybranego konta. Kliknij przycisk **OK** , aby zakończyć. Następnym razem po uruchomieniu systemu Windows 10 zostanie automatycznie zalogowanie się do wybranego konta.
