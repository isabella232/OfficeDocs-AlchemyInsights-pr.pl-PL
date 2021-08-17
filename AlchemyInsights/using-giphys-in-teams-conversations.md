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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104318"
---
# <a name="using-giphys-in-teams-conversations"></a>Korzystanie z aplikacji Giphy w Teams konwersacjach

Dostęp do aplikacji Giphy w Teams jest domyślnie włączony. Jako administrator możesz kontrolować, czy aplikacja **Giphys** jest dostępna dla użytkowników, ustawiając zasady obsługi wiadomości i upewniając się, że w konwersacjach jest [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) wł. 

Jeśli pliki GIF nie działają zgodnie z oczekiwaniami w Teams konwersacjach, sprawdź:

Zasady [wiadomości muszą](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) zezwalać na giphy. Aby to sprawdzić przy użyciu poleceń cmdlet programu PowerShell:

- Sprawdź, czy możesz [zarządzać Teams za pomocą programu PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Uruchom polecenie programu PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i upewnij się, że dla właściwości **AllowGiphy** ustawiono wartość **TRUE.**
- Jeśli **dla właściwości AllowGiphy** ustawiono wartość **FALSE,** uruchom następujące polecenie programu PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Opcjonalne połączone środowisko musi](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) zostać włączone, aby umożliwić dostęp do adresu URL Giphy.

> [!NOTE]
> Jeśli dla dzierżawy skonfigurowano wiele zasad usługi Teams Messaging, możesz określić tożsamość zasad przypisanych do użytkownika, na który wpływa problem, za pomocą polecenia [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) dla programu PowerShell | <user@domain.com> Wybierz pozycję TeamsMessagingPolicy.
