---
title: Korzystanie z animacjami Giphy w rozmowach zespołów
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982502"
---
# <a name="using-giphys-in-teams-conversations"></a>Korzystanie z animacjami Giphy w rozmowach zespołów

Animacjami Giphy dostęp w usłudze Teams jest domyślnie włączony. Jako administrator możesz kontrolować, czy animacjami Giphy są dostępne dla użytkowników, [ustawiając zasady obsługi wiadomości](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i upewniając się, że **Korzystanie z animacjami Giphy w konwersacjach** jest **włączone**.

Jeśli w konwersacjach zespołów pliki GIF nie działają zgodnie z oczekiwaniami, sprawdź, czy:

[Zasady obsługi wiadomości](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) muszą zezwalać na animacjami Giphy. Aby sprawdzić za pomocą poleceń cmdlet programu PowerShell:

- Sprawdź, czy możesz [zarządzać zespołami za pomocą programu PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Uruchom polecenie programu PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i sprawdź, czy **AllowGiphy** jest ustawiona na **wartość true**.
- Jeśli **AllowGiphy** jest ustawiona na **false** , uruchom następujące polecenie programu PowerShell [Set-CsTeamsMessagingPolicy-Identity Global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

W celu umożliwienia dostępu do adresu URL usługi Giphy należy włączyć [opcjonalne środowisko połączone](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Jeśli dla dzierżawy skonfigurowano wiele zasad dotyczących wiadomości programu Teams, możesz określić tożsamość zasad przypisanych do dotkniętego problemem użytkownikowi za pomocą polecenia programu PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Wybierz pozycję TeamsMessagingPolicy.
