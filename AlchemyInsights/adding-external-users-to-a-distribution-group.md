---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910942"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej

Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:
  
1. Utwórz kontakt poczty dla użytkownika zewnętrznego:
    
    1. W centrum administracyjnym przejdź do strony[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) **użytkowników.** >  
    
    2. Wybierz **pozycję Dodaj kontakt**.
    
    3. Wpisz informacje dotyczące kontaktu i wybierz pozycję **Dodaj**.
    
2. Dodaj kontakt pocztowy do dyrekcji dg:
    
    1. W centrum administracyjnym przejdź **Groups** > do strony[Grupy](https://admin.microsoft.com/adminportal/home#/groups) grup. 
    
    2. Znajdź dyrekcję dg, do której chcesz dodać użytkownika zewnętrznego, i wybierz ją, aby otworzyć okno dialogowe edycji.
    
    3. Na karcie **Członkowie** wybierz pozycję **Wyświetl wszystkich członków i zarządzaj nimi.** 
    
    4. Wybierz **pozycję Dodaj członków**.
    
    5. Wybierz kontakt poczty utworzony w poprzednim kroku, a następnie wybierz pozycję **Zapisz**.
    
Jeśli po wykonać te kroki użytkownicy zewnętrzni nie mogą wysyłać wiadomości e-mail do Dyrekcji DG lub nie otrzymują od niej wiadomości e-mail, może to oznaczać, że Dyrekcja DG jest oznaczona jako zezwalana tylko na wiadomości e-mail od użytkowników wewnętrznych. Możesz sprawdzić tę konfigurację i naprawić ją, postępują zgodnie ze wskazówkami [tutaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy to "Grupa microsoft 365" zamiast "Grupa dystrybucyjna". W takim przypadku można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook. Szczegółowe informacje na temat gości grupy Microsoft 365 oraz instrukcje dotyczące dodawania gości zewnętrznych można znaleźć w [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  