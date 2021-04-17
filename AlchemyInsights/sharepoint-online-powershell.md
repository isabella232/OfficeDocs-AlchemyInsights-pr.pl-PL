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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="dde74-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="dde74-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="dde74-103">Pracujesz z programem PowerShell lub skryptami w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="dde74-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="dde74-104">Aby uzyskać więcej informacji, odwiedź poniższe linki.</span><span class="sxs-lookup"><span data-stu-id="dde74-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="dde74-105">Wprowadzenie do powłoki zarządzania usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="dde74-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="dde74-106">Nawiązywanie połączenia z programem PowerShell usługi SPO za pomocą uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="dde74-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="dde74-107">Wzorce i wskazówki programu [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w kierunku usługi SPO.</span><span class="sxs-lookup"><span data-stu-id="dde74-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="dde74-108">Jeśli masz problemy z połączeniem się z powłoką zarządzania usługą SPO, [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) upewnij się, że zaktualizowano program do najnowszej wersji, i spróbuj ponownie zaimportować moduł za pomocą *polecenia "Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="dde74-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="dde74-109">Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, na komputerze lokalnym musi być zainstalowany zestaw SDK składników klienta usługi [SharePoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)</span><span class="sxs-lookup"><span data-stu-id="dde74-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="dde74-110">Jeśli masz problemy z uruchamianiem skryptów z programu PowerShell, rozważ uruchomienie programu PowerShell jako administrator i zmianę [zasad wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="dde74-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>