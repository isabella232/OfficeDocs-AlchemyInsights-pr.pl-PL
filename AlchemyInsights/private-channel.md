---
title: Kanał prywatny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005448"
---
# <a name="private-channels-in-microsoft-teams"></a>Kanały prywatne w usłudze Microsoft Teams

Kanały prywatne to nowa funkcja w usłudze Microsoft Teams. Należy pamiętać, że kanałów prywatnych nie można konwertować ze standardowych kanałów ani odwrotnie.

Aby uzyskać szczegółowe informacje o kanałach prywatnych, takich jak informacje o [tworzeniu kanałów prywatnych i członkostwie](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) oraz [witrynach programu SharePoint kanału prywatnego,](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)zobacz [Kanały prywatne w usłudze Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Uwaga:** Ponieważ konfiguracja przechowywania wiadomości kanału prywatnego nie jest jeszcze obsługiwana, dzierżawcy z włączonymi zasadami przechowywania nie będą domyślnie wstrzymywani kanałów prywatnych. Kanały prywatne można włączyć w centrum administracyjnym zespołów. Należy również pamiętać, że podczas przechowywania wiadomości kanału prywatnego nie jest obsługiwany, przechowywanie plików udostępnionych w kanałach prywatnych jest obsługiwane.

**Potrzebujesz nowego właściciela zespołu?**

Jeśli twój prywatny właściciel kanału odejdzie, możesz dodać nowego właściciela zespołu za pośrednictwem programu Teams Powershell.


- Przejdź [tutaj,](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) aby zainstalować program Teams Powershell.

Oto polecenie cmdlet, którego potrzebujesz:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Aby uzyskać więcej informacji na temat programu Teams Powershell, zobacz [Omówienie programu Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
