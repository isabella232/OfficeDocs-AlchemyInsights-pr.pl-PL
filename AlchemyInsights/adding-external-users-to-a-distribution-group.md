---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934843"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej

Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej jest procesem dwuetapowym:
  
1. Tworzenie kontaktu pocztowego dla użytkownika zewnętrznego:
    
    1. W centrum administracyjnym przejdź do strony **Kontakty**  >  [](https://admin.microsoft.com/adminportal/home#/Contact) użytkowników. 
    
    2. Wybierz **pozycję Dodaj kontakt**.
    
    3. Wpisz informacje o kontakcie i wybierz pozycję **Dodaj**.
    
2. Dodawanie kontaktu pocztowego do listy kontaktów:
    
    1. W centrum administracyjnym przejdź do strony  >  [Grupy](https://admin.microsoft.com/adminportal/home#/groups) grupy. 
    
    2. Znajdź dg danych, do której chcesz dodać użytkownika zewnętrznego, i wybierz ją, aby otworzyć okno dialogowe edycji.
    
    3. Na karcie **Członkowie** wybierz pozycję **Wyświetl wszystkich i zarządzaj członkami**. 
    
    4. Wybierz **pozycję Dodaj członków**.
    
    5. Wybierz kontakt pocztowy utworzony w poprzednim kroku, a następnie wybierz pozycję **Zapisz**.
    
Jeśli po zakończeniu tych czynności użytkownicy zewnętrzni nie mogą wysyłać wiadomości e-mail do sieci dg lub nie otrzymują wiadomości e-mail z tej listy, być może owa owa dg jest oznaczona tak, aby zezwalała tylko na wiadomości e-mail od użytkowników wewnętrznych. Możesz sprawdzić konfigurację i rozwiązać ją, zgodnie z [instrukcjami](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)tutaj.
  
 **Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy to "grupa Microsoft 365" zamiast "Grupa dystrybucyjna". W takim przypadku możesz dodać użytkownika zewnętrznego bezpośrednio do grupy z Outlook. Szczegółowe informacje o Microsoft 365 grupy, a także instrukcje dodawania gości zewnętrznych można znaleźć w [tym artykule.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  