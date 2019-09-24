---
title: PowerShell Online programu SharePoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123008"
---
# <a name="sharepoint-online-powershell"></a>PowerShell Online programu SharePoint

Praca z PowerShell lub skrypty w programie SharePoint Online? Aby uzyskać więcej informacji, odwiedź poniższe linki.
- [Pierwsze kroki z programu SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Połącz się z PowerShell SPO z uwierzytelniania wieloskładnikowego (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Wzorce i praktyki programu SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawiera bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych działań zarządzania w kierunku spo.

> [!NOTE]
> - Jeśli występują problemy z połączeniem z powłoką zarządzania SPO, upewnij się, że zostały zaktualizowane do najnowszej wersji i spróbuj [ponownie zaimportować moduł](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) za pomocą *"Import-Module Microsoft. online. SharePoint. PowerShell".*
> - Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, trzeba będzie mieć [SharePoint Online klienta składniki SDK](https://www.microsoft.com/download/details.aspx?id=42038) zainstalowane na komputerze lokalnym.
> - Jeśli masz problemy z uruchomieniem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administrator i zmienianie [zasad wykonywania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).