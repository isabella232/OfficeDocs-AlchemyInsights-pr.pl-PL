---
title: Użytkownik odbiera błąd AADSTS7000112 Usługa Yammer jest wyłączona
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198376"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Użytkownik odbiera błąd AADSTS7000112 Usługa Yammer jest wyłączona

Jeśli zostanie wyświetlony błąd "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000000000" (Yammer) jest wyłączony", występuje problem z jednostką usługi w usłudze Azure AD. Administrator mógł wyłączyć jednostkę usługi, aby zablokować dostęp do usługi Yammer.

Wyłączenie jednostki usługi nie jest zalecane i może spowodować dodatkowe problemy. Aby uzyskać więcej informacji na temat obsługiwanego podejścia do blokowania dostępu użytkownika do usługi Yammer, zobacz [Wyłączanie dostępu usługi Yammer dla użytkowników usługi Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Aby rozwiązać ten problem w witrynie Azure Portal i przywrócić dostęp użytkowników do usługi Yammer:

1.  Otwórz stronę Usługi Azure Active Directory i wybierz pozycję **Aplikacje przedsiębiorstwa** w obszarze **Zarządzaj** w lewym okienku nawigacji.
3.  Wpisz **usługę Yammer usługi Office 365** w polu wyszukiwania i wybierz nazwę aplikacji, aby otworzyć ustawienia.
4.  Wybierz **pozycję Właściwości** w obszarze **Zarządzaj** w lewym okienku nawigacji.
5.  Czy ustaw wartość **Włączone dla użytkowników do logowania?** na **Tak**, a następnie wybierz pozycję **Zapisz**.
6.  Zaloguj się ponownie do usługi Yammer. Może być konieczne wyczyszczenie plików cookie.

Alternatywnie uruchom polecenia programu PowerShell, aby ustawić wartość. Aby uzyskać więcej informacji, zobacz [błąd "Przepraszamy, ale problemy z zalogowaniem się" po kliknięciu kafelka Usługi Yammer w usłudze Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 