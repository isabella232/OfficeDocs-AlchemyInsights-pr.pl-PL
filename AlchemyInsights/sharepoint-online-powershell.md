---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709080"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Pracujesz z programem PowerShell lub skryptami w usłudze SharePoint Online? Aby uzyskać więcej informacji, odwiedź poniższe linki.
- [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Łączenie się z programem PowerShell usługi SPO za pomocą uwierzytelniania wieloskładnikowego (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Wzorce i wskazówki programu [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w stosunku do usługi SPO.

> [!NOTE]
> - Jeśli masz problemy z nawiązaniem połączenia z powłoką zarządzania usługi SPO, [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) upewnij się, że zaktualizowano usługę SPO do najnowszej wersji, i spróbuj ponownie zaimportować moduł przy użyciu *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, na komputerze lokalnym musi być zainstalowany zestaw SDK składników klienta usługi [SharePoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)
> - Jeśli masz problemy z uruchamianiem skryptów z programu PowerShell, możesz rozważyć uruchomienie programu PowerShell jako administrator i zmianę zasad [wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)