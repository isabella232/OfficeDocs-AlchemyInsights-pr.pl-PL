---
title: SharePoint online — program PowerShell
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770849"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="ac0ed-102">SharePoint online — program PowerShell</span><span class="sxs-lookup"><span data-stu-id="ac0ed-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="ac0ed-103">Pracujesz za pomocą programu PowerShell lub skryptów w usłudze SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ac0ed-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="ac0ed-104">Aby uzyskać więcej informacji, Skorzystaj z linków poniżej.</span><span class="sxs-lookup"><span data-stu-id="ac0ed-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="ac0ed-105">Wprowadzenie do powłoki zarządzania usługi SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ac0ed-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="ac0ed-106">Nawiązywanie połączenia z programem usługi spo programu PowerShell za pomocą uwierzytelniania wieloskładnikowego (MFA)</span><span class="sxs-lookup"><span data-stu-id="ac0ed-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="ac0ed-107">Funkcje [wzorów i praktyk programu SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) zawierają bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji związanych z zarządzaniem w kierunku usługi spo.</span><span class="sxs-lookup"><span data-stu-id="ac0ed-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="ac0ed-108">Jeśli masz problemy z połączeniem się z powłoką zarządzania usługi spo, upewnij się, że Zaktualizowano najnowszą wersję, i spróbuj [ponownie zaimportować moduł,](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) używając *"Import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="ac0ed-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="ac0ed-109">W przypadku próby uruchomienia skryptów modelu obiektów po stronie klienta na komputerze lokalnym musi być zainstalowany [zestaw SDK składniki klienta usługi SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="ac0ed-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="ac0ed-110">Jeśli występują problemy z uruchamianiem skryptów z programu PowerShell, warto rozważyć uruchomienie programu PowerShell jako administrator i zmianę [zasad wykonywania](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="ac0ed-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>