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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="01637-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="01637-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="01637-103">Pracujesz z programem PowerShell lub skryptami w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="01637-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="01637-104">Aby uzyskać więcej informacji, odwiedź poniższe linki.</span><span class="sxs-lookup"><span data-stu-id="01637-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="01637-105">Wprowadzenie do powłoki zarządzania usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="01637-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="01637-106">Łączenie się z programem PowerShell usługi SPO za pomocą uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="01637-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="01637-107">Wzorce i wskazówki programu [SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w stosunku do usługi SPO.</span><span class="sxs-lookup"><span data-stu-id="01637-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="01637-108">Jeśli masz problemy z nawiązaniem połączenia z powłoką zarządzania usługi SPO, [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) upewnij się, że zaktualizowano usługę SPO do najnowszej wersji, i spróbuj ponownie zaimportować moduł przy użyciu *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="01637-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="01637-109">Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, na komputerze lokalnym musi być zainstalowany zestaw SDK składników klienta usługi [SharePoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)</span><span class="sxs-lookup"><span data-stu-id="01637-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="01637-110">Jeśli masz problemy z uruchamianiem skryptów z programu PowerShell, możesz rozważyć uruchomienie programu PowerShell jako administrator i zmianę zasad [wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="01637-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>