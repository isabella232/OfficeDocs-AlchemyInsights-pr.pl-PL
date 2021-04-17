---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830592"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Pracujesz z programem PowerShell lub skryptami w usłudze SharePoint Online? Aby uzyskać więcej informacji, odwiedź poniższe linki.
- [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Nawiązywanie połączenia z programem PowerShell usługi SPO za pomocą uwierzytelniania wieloskładnikowego (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Wzorce i wskazówki programu [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w kierunku usługi SPO.

> [!NOTE]
> - Jeśli masz problemy z połączeniem się z powłoką zarządzania usługą SPO, [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) upewnij się, że zaktualizowano program do najnowszej wersji, i spróbuj ponownie zaimportować moduł za pomocą *polecenia "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, na komputerze lokalnym musi być zainstalowany zestaw SDK składników klienta usługi [SharePoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)
> - Jeśli masz problemy z uruchamianiem skryptów z programu PowerShell, rozważ uruchomienie programu PowerShell jako administrator i zmianę [zasad wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)