---
title: Korzystanie z aplikacji Giphy w Teams konwersacjach
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323530"
---
# <a name="using-giphys-in-teams-conversations"></a>Korzystanie z aplikacji Giphy w Teams konwersacjach

Dostęp do giphy w Teams jest domyślnie włączony. Jako administrator możesz kontrolować, czy aplikacja **Giphys** jest dostępna dla użytkowników, ustawiając zasady obsługi wiadomości i upewniając się, że w konwersacjach jest [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) wł. 

Jeśli pliki GIF nie działają zgodnie z oczekiwaniami w Teams konwersacjach, sprawdź:

Zasady [wiadomości muszą zezwalać](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) na giphy. Aby to sprawdzić przy użyciu poleceń cmdlet programu PowerShell:

- Sprawdź, czy możesz [zarządzać Teams za pomocą programu PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Uruchom polecenie programu PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i upewnij się, że dla właściwości **AllowGiphy** ustawiono wartość **TRUE.**
- Jeśli **dla właściwości AllowGiphy** ustawiono wartość **FALSE,** uruchom następujące polecenie programu PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Opcjonalne połączone środowisko musi](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) zostać włączone, aby umożliwić dostęp do adresu URL Giphy.

**Uwaga:** Jeśli dla twojej dzierżawy skonfigurowano wiele zasad obsługi wiadomości usługi Teams, możesz określić tożsamość zasad przypisanych do użytkownika, na który wpływa problem, za pomocą polecenia [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Wybierz pozycję TeamsMessagingPolicy.
