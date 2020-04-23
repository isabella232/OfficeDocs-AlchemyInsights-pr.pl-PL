---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764271"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Praca z programem PowerShell lub skryptami w usłudze Sharepoint Online? Odwiedź poniższe linki, aby uzyskać więcej informacji.
- [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Łączenie się z programem SPO PowerShell za pomocą uwierzytelniania wieloskładnikowego (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Wzorce i praktyki programu SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawiera bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w kierunku spo.

> [!NOTE]
> - Jeśli występują problemy z nawiązaniem połączenia z powłoką zarządzania SPO, upewnij się, że zaktualizowano do najnowszej wersji i spróbuj [ponownie zaimportować moduł](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) przy użyciu *funkcji "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, musisz mieć zainstalowany [sDK składników klienta usługi Sharepoint Online na](https://www.microsoft.com/download/details.aspx?id=42038) komputerze lokalnym.
> - Jeśli występują problemy z uruchamianiem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administratora i zmianę [zasad wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)