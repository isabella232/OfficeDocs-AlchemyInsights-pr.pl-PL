---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737883"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej

Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:
  
1. Utwórz kontakt poczty dla użytkownika zewnętrznego:
    
    1. W centrum administracyjnym przejdź na stronę[kontakty](https://admin.microsoft.com/adminportal/home#/Contact) **użytkowników** > . 
    
    2. Wybierz pozycję **Dodaj kontakt**.
    
    3. Wpisz informacje o kontakcie i wybierz **Dodaj**.
    
2. Dodaj kontakt poczty do swojej DG:
    
    1. W centrum administracyjnym przejdź > [na stronę](https://admin.microsoft.com/adminportal/home#/groups) **grupy grup.** 
    
    2. Znajdź DG, do której chcesz dodać użytkownika zewnętrznego, i wybierz ją, aby otworzyć okno dialogowe edycji.
    
    3. Na karcie **Członkowie** wybierz pozycję **Wyświetl wszystkie i Zarządzaj elementami członkowskimi**. 
    
    4. Wybierz **Dodaj członków**.
    
    5. Wybierz kontakt poczty utworzony w poprzednim kroku, a następnie wybierz **Zapisz**.
    
Jeśli po wykonaniu tych czynności użytkownicy zewnętrzni nie mogą wysyłać e-maili do Dyrekcji Generalnej lub nie otrzymywać od niego wiadomości e-mail, może to być, że DG jest oznaczony, aby zezwolić tylko na wiadomości e-mail od użytkowników wewnętrznych. Możesz sprawdzić tę konfigurację i naprawić go zgodnie z instrukcjami [tutaj](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Uwaga:** Te instrukcje nie mają zastosowania, jeśli typem grupy jest "Office 365 grupy" zamiast "grupy dystrybucyjnej." W takim przypadku można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook. Szczegółowe informacje na temat Office 365 grupy Gości, jak również instrukcje dotyczące dodawania Gości zewnętrznych można znaleźć w [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  