---
title: Usuwanie osieroconego użytkownika z serwera lokalnego
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198592"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Usuwanie osieroconego użytkownika z serwera lokalnego

Aby usunąć osieroconego użytkownika, wykonaj następujące czynności:

1. Wymusić synchronizację katalogów, postępując zgodnie z instrukcjami w [obszarze Co to jest tożsamość hybrydowa z usługą Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Aby zweryfikować synchronizację katalogów, zobacz [Co to jest tożsamość hybrydowa z usługą Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Jeśli synchronizacja działa poprawnie, ale usunięcie obiektu usługi Active Directory nie jest propagowane do usługi Azure AD, ręcznie usuń oddzielony obiekt przy użyciu jednego z następujących poleceń cmdlet usługi Azure Active Directory dla programu Windows PowerShell:

    Usuń-MsolContaktact  
    Usuń-MsolGroup  
    Usuń-MsolUser

    Na przykład, aby usunąć osierocony identyfikator użytkownika john.smith@contoso.com, pierwotnie utworzony przy użyciu synchronizacji katalogów, uruchom polecenie cmdlet:

    Usuń-MsolUser –UserPrincipalName John.Smith@Contoso.com