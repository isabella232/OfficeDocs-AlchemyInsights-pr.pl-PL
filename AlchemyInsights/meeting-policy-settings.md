---
title: Ustawienia zasad spotkania
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704616"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Zarządzanie zasadami spotkań w aplikacji Microsoft Teams

**Uwaga: może upłynieć do 24 godzin, aż zmiany zasad zajdą w życie dla użytkowników.** Zmiany nowo utworzonych zasad mogą nie być możliwe od razu; Odczekaj 4 godziny i spróbuj ponownie zmodyfikować nowo utworzone zasady.

Zasady spotkań służą do kontrolowania funkcji dostępnych dla uczestników spotkania w przypadku spotkań zaplanowanych przez użytkowników w organizacji. Niektóre funkcje zasad spotkań mogą nie być jeszcze zaimplementowane w centrum administracyjnym aplikacji Teams (w dokumentacji są one oznaczone jako "wkrótce"). W takim przypadku lub w przypadku wystąpienia błędu, takiego jak "Nie możemy w tej chwili zaktualizować zasad, ale spróbuj ponownie później" w centrum administracyjnym usługi Microsoft Teams, zalecamy używanie programu PowerShell do tworzenia lub modyfikowania zasad spotkań aplikacji Teams. 

Aby uzyskać więcej informacji na temat zasad spotkań, zobacz następujące zasoby:

- Aby dowiedzieć się, jak tworzyć zasady, wprowadzać zmiany i przypisywać użytkowników do zasad, zobacz Zarządzanie zasadami spotkań w [aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Aby wprowadzić zmiany w zasadach przy użyciu poleceń cmdlet programu PowerShell, zobacz [Omówienie programu Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Musisz użyć modułu Skype dla [firm PowerShell dla](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) zasad spotkań aplikacji Teams. 
    - Aby uzyskać więcej informacji, zapoznaj się z dokumentacją [polecenia cmdlet *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

