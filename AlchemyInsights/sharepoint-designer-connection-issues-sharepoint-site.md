---
title: Poziomy uprawnień programu SharePoint w trybie Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760702"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="b0c93-102">Problemy z połączeniem programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b0c93-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="b0c93-103">Jeśli program SharePoint Designer występują problemy z połączeniem do witryn programu SharePoint, prosimy spróbować następujących wspólnych rozwiązań.</span><span class="sxs-lookup"><span data-stu-id="b0c93-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="b0c93-104">Krok 1: Sprawdź aktualizacja programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b0c93-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="b0c93-105">Program SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="b0c93-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="b0c93-106">Dodatek Service Pack 1 (SP1) dla programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="b0c93-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="b0c93-107">Aktualizacja dla programu SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="b0c93-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="b0c93-108">Krok 2: Wyczyść lokalnej pamięci podręcznej plików</span><span class="sxs-lookup"><span data-stu-id="b0c93-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="b0c93-109">Zamknij program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="b0c93-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="b0c93-110">Na komputerze lokalnym przejdź do następujących folderów, aby usunąć pliki z pamięci podręcznej.</span><span class="sxs-lookup"><span data-stu-id="b0c93-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="b0c93-111">Kliknij przycisk Start, uruchom i Usuń wszystkie pliki znajdują się w obszarze każdego z poniżej lokalizacjach.</span><span class="sxs-lookup"><span data-stu-id="b0c93-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="b0c93-112">Serwer %appdata%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="b0c93-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="b0c93-113">Otwórz program SharePoint Designer 2013 i wprowadzić konto ponownie, aby sprawdzić, czy działa.</span><span class="sxs-lookup"><span data-stu-id="b0c93-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="b0c93-114">Krok 3: [Włącz uwierzytelnianie nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="b0c93-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="b0c93-115">Krok 4: Administratorzy należy umożliwić niestandardowego skryptu zezwalające na połączenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="b0c93-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="b0c93-116">Aby uzyskać szczegółowe instrukcje, przykłady i uwagi dotyczące zobacz [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="b0c93-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


