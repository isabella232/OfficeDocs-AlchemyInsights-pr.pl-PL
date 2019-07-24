---
title: Problemy z połączeniem programu SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840561"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="52438-102">Problemy z połączeniem programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="52438-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="52438-103">Jeśli program SharePoint Designer występują problemy z połączeniem do witryn programu SharePoint, spróbuj następujących wspólnych rozwiązań.</span><span class="sxs-lookup"><span data-stu-id="52438-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="52438-104">Krok 1: Sprawdź, czy program SharePoint Designer 2013 jest aktualizowana z [dodatku Service Pack 1 dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2 sierpnia 2016 aktualizacja dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="52438-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="52438-105">Krok 2: Wyczyść pliki lokalnej pamięci podręcznej:</span><span class="sxs-lookup"><span data-stu-id="52438-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="52438-106">Zamknij program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="52438-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="52438-107">Na komputerze lokalnym należy usunąć wszystkie pliki znajdujące się w każdym z następujących folderów.</span><span class="sxs-lookup"><span data-stu-id="52438-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="52438-108">Extensions\Cache serwera %appdata%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="52438-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="52438-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="52438-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="52438-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="52438-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="52438-111">Otwórz program SharePoint Designer 2013 i wprowadzić konto ponownie, aby sprawdzić, czy działa.</span><span class="sxs-lookup"><span data-stu-id="52438-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="52438-112">Krok 3: [Włącz uwierzytelnianie nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="52438-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="52438-113">Krok 4: Administratorzy należy **Umożliwić niestandardowego skryptu** w ustawieniach Centrum administracyjnego programu SharePoint zezwalające na połączenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="52438-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="52438-114">Zobacz [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="52438-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


