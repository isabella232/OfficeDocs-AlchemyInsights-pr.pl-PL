---
title: Ustawienia zasad spotkania
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376760"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Zarządzanie zasadami spotkania w programie Microsoft Teams

Zasady spotkania są używane do kontrolowania funkcji, które są dostępne dla uczestników spotkania dla spotkań, które są zaplanowane przez użytkowników w organizacji. Niektóre funkcje zasad spotkania mogą nie zostać wdrożone w centrum administracyjnym zespołów jeszcze (są one oznaczone jako "wkrótce" w dokumentacji). W tym przypadku lub jeśli otrzymujesz błąd, takich jak "Firma Microsoft nie można zaktualizować zasady teraz, ale spróbuj ponownie później" w centrum administracyjnego programu Teams firmy Microsoftzaleca się używanie programu PowerShell do tworzenia lub modyfikowania zespołów zasad spotkania. 

Aby uzyskać więcej informacji na temat zasad spotkania zobacz następujące zasoby:

- Aby dowiedzieć się więcej na temat tworzenia zasad, wprowadzania zmian i przypisywania użytkowników do zasad, zobacz [Zarządzanie zasadami spotkania w zespołach](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Aby wprowadzić zmiany zasad za pomocą poleceń cmdlet programu PowerShell, zobacz [Omówienie programu PowerShell zespołów](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Należy użyć programu [Skype dla modułu Business PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) dla zespołów spotkań zasad. 
    - Przejrzyj [dokumentację poleceń cmdlet *-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , aby uzyskać więcej informacji.

**Uwaga:** Może potrwać do 24 godzin, aby zmiany zasad zostały uwzględnione dla użytkowników. Może nie być możliwe natychmiastowe wprowadzenie zmian w nowo utworzonych zasadach; Poczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzoną zasadę. Jeśli nadal występują problemy, Wypróbuj program PowerShell.  