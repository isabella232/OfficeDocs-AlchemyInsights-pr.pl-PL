---
title: SharePoint online — program PowerShell
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786899"
---
# <a name="sharepoint-online-powershell"></a>SharePoint online — program PowerShell

Pracujesz za pomocą programu PowerShell lub skryptów w usłudze SharePoint Online? Aby uzyskać więcej informacji, Skorzystaj z linków poniżej.
- [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Nawiązywanie połączenia z programem usługi spo programu PowerShell za pomocą uwierzytelniania wieloskładnikowego (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Funkcje [wzorów i praktyk programu SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji związanych z zarządzaniem w kierunku usługi spo.

> [!NOTE]
> - Jeśli masz problemy z połączeniem się z powłoką zarządzania usługi spo, upewnij się, że Zaktualizowano najnowszą wersję, i spróbuj [ponownie zaimportować moduł,](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) używając *"Import-Module Microsoft. online. SharePoint. PowerShell".*
> - W przypadku próby uruchomienia skryptów modelu obiektów po stronie klienta na komputerze lokalnym musi być zainstalowany [zestaw SDK składniki klienta usługi SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .
> - Jeśli występują problemy z uruchamianiem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administrator i zmianę [zasad wykonywania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).