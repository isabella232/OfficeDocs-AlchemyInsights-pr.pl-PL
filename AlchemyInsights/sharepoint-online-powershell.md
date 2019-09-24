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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="9c4a6-102">PowerShell Online programu SharePoint</span><span class="sxs-lookup"><span data-stu-id="9c4a6-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="9c4a6-103">Praca z PowerShell lub skrypty w programie SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9c4a6-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="9c4a6-104">Aby uzyskać więcej informacji, odwiedź poniższe linki.</span><span class="sxs-lookup"><span data-stu-id="9c4a6-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="9c4a6-105">Pierwsze kroki z programu SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="9c4a6-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="9c4a6-106">Połącz się z PowerShell SPO z uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="9c4a6-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="9c4a6-107">[Wzorce i praktyki programu SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawiera bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych działań zarządzania w kierunku spo.</span><span class="sxs-lookup"><span data-stu-id="9c4a6-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="9c4a6-108">Jeśli występują problemy z połączeniem z powłoką zarządzania SPO, upewnij się, że zostały zaktualizowane do najnowszej wersji i spróbuj [ponownie zaimportować moduł](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) za pomocą *"Import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="9c4a6-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="9c4a6-109">Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, trzeba będzie mieć [SharePoint Online klienta składniki SDK](https://www.microsoft.com/download/details.aspx?id=42038) zainstalowane na komputerze lokalnym.</span><span class="sxs-lookup"><span data-stu-id="9c4a6-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="9c4a6-110">Jeśli masz problemy z uruchomieniem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administrator i zmienianie [zasad wykonywania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="9c4a6-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>