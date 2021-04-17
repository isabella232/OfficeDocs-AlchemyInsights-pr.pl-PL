---
title: Ustawienia zasad spotkania
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825453"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Zarządzanie zasadami spotkań w aplikacji Microsoft Teams

**Uwaga: może upłynieć do 24 godzin, aż zmiany zasad zajdą w życie dla użytkowników.** Być może nie będzie można natychmiast wprowadzić zmian w nowo utworzonych zasadach. Odczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.

Zasady spotkań służą do kontrolowania funkcji dostępnych dla uczestników spotkań zaplanowanych przez użytkowników w organizacji. Niektóre funkcje zasad spotkań mogą nie być jeszcze zaimplementowane w centrum administracyjnym aplikacji Teams (są oznaczone w dokumentacji jako "wkrótce"). W takim przypadku lub w przypadku wystąpienia błędu, takiego jak "Nie możemy w tej chwili zaktualizować zasad, ale spróbujemy ponownie później" w centrum administracyjnym usługi Microsoft Teams, zalecamy używanie programu PowerShell do tworzenia i modyfikowania zasad spotkań aplikacji Teams. 

Aby uzyskać więcej informacji na temat zasad spotkania, zobacz następujące zasoby:

- Aby dowiedzieć się więcej o tworzeniu zasad, zmienianiu i przypisywaniu użytkowników do zasad, zobacz [Zarządzanie zasadami spotkań w aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Aby wprowadzić zmiany w zasadach przy użyciu poleceń cmdlet programu PowerShell, zobacz [Omówienie programu Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Należy użyć modułu [Skype dla firm PowerShell dla](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) zasad spotkania w aplikacji Teams. 
    - Przejrzyj [dokumentację polecenia cmdlet *-CsTeamsMeetingPolicy,](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) aby uzyskać więcej informacji.

