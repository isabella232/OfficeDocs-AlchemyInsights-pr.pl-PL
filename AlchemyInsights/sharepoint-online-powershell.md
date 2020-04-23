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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="529fb-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="529fb-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="529fb-103">Praca z programem PowerShell lub skryptami w usłudze Sharepoint Online?</span><span class="sxs-lookup"><span data-stu-id="529fb-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="529fb-104">Odwiedź poniższe linki, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="529fb-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="529fb-105">Wprowadzenie do powłoki zarządzania usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="529fb-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="529fb-106">Łączenie się z programem SPO PowerShell za pomocą uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="529fb-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="529fb-107">[Wzorce i praktyki programu SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawiera bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania w kierunku spo.</span><span class="sxs-lookup"><span data-stu-id="529fb-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="529fb-108">Jeśli występują problemy z nawiązaniem połączenia z powłoką zarządzania SPO, upewnij się, że zaktualizowano do najnowszej wersji i spróbuj [ponownie zaimportować moduł](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) przy użyciu *funkcji "Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="529fb-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="529fb-109">Jeśli próbujesz uruchomić skrypty modelu obiektów po stronie klienta, musisz mieć zainstalowany [sDK składników klienta usługi Sharepoint Online na](https://www.microsoft.com/download/details.aspx?id=42038) komputerze lokalnym.</span><span class="sxs-lookup"><span data-stu-id="529fb-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="529fb-110">Jeśli występują problemy z uruchamianiem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administratora i zmianę [zasad wykonywania.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="529fb-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>