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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663523"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej

Dodanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:
  
1. Tworzenie kontaktu poczty dla użytkownika zewnętrznego:
    
    1. W centrum administracyjnym przejdź do strony Kontakty **użytkowników**  >  [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Wybierz pozycję **Dodaj kontakt**.
    
    3. Wpisz informacje dotyczące kontaktu i wybierz pozycję **Dodaj**.
    
2. Dodaj kontakt z pocztą do swojej DG:
    
    1. W centrum administracyjnym przejdź do strony grupy **grup**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Znajdź DG, do którego chcesz dodać użytkownika zewnętrznego, a następnie wybierz go, aby otworzyć okno dialogowe Edytowanie.
    
    3. Na karcie **Członkowie** wybierz pozycję **Pokaż wszystkich członków i zarządzaj nimi**. 
    
    4. Wybierz pozycję **Dodaj członków**.
    
    5. Wybierz kontakt poczty utworzony w poprzednim kroku, a następnie wybierz pozycję **Zapisz**.
    
Jeśli po wykonaniu tych czynności użytkownicy zewnętrzni nie będą mogli wysyłać wiadomości e-mail do tej DG ani odbierać wiadomości e-mail z tej usługi, może to oznaczać, że ta DG jest oznaczona jako przeznaczona tylko do obsługi wiadomości e-mail od użytkowników wewnętrznych. Możesz sprawdzić tę konfigurację i rozwiązać ją, postępując zgodnie z [instrukcjami.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ Twojej grupy to "Microsoft 365 Group" zamiast "Grupa dystrybucyjna". W takim przypadku użytkownik zewnętrzny może dodać użytkownika zewnętrznego bezpośrednio do grupy z poziomu programu Outlook. Szczegółowe informacje na temat Gości grupowych Microsoft 365 oraz instrukcje dotyczące dodawania zewnętrznych Gości można znaleźć w [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  