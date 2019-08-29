---
title: Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660802"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodawanie użytkowników zewnętrznych do grupy dystrybucyjnej

Dodawanie kontaktu zewnętrznego do grupy dystrybucyjnej (DG) jest procesem dwuetapowym:
  
1. Tworzenie kontaktu poczty dla użytkownika zewnętrznego:
    
    1. W Centrum administracyjnym przejdź do **użytkowników** > strony[Kontakty](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Wybierz opcję **Dodaj kontakt**.
    
    3. Wpisz informacje dotyczące kontaktu i wybierz polecenie **Dodaj**.
    
2. Dodaj kontakt poczty do Twojego DG:
    
    1. W Centrum administracyjnego, przejdź do **grupy** > strony[grupy](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Znajdź DG, którego chcesz dodać użytkownika zewnętrznego do i zaznacz ją, aby otworzyć okno dialogowe Edytuj.
    
    3. Na karcie **Członkowie** wybierz **Wyświetl wszystkie i Zarządzaj członkami**. 
    
    4. Wybierz **Dodaj członków**.
    
    5. Wybierz kontakt poczty został utworzony w poprzednim kroku, a następnie wybierz przycisk **Zapisz**.
    
Jeśli po wykonaniu tych czynności użytkownika zewnętrznego, nie można wysłać wiadomości e-mail do dyrekcji generalnej lub nie otrzymywać wiadomości e-mail z niego, możliwe, że DG jest oznaczona zezwalają tylko wiadomości e-mail od użytkowników wewnętrznych. Można sprawdzić tę konfigurację i naprawić go zgodnie ze wskazówkami wyświetlanymi [w tym miejscu](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).
  
 **Uwaga:** Te instrukcje nie mają zastosowania, jeśli typ grupy jest "Grupa Office 365" zamiast "Grupa dystrybucyjna." Jeśli tak się stanie, można dodać użytkownika zewnętrznego bezpośrednio do grupy z programu Outlook. W [tym artykule](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)znajdują się szczegółowe informacje dotyczące usługi Office 365 grupy gości, jak również instrukcje dotyczące dodawania zewnętrznego gośćmi.
  