---
title: Problemy z połączeniem programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051723"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="67858-102">Problemy z połączeniem programu SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="67858-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="67858-103">Jeśli program SharePoint Designer występuje problemy z połączeniem do witryn programu SharePoint, wypróbuj następujące typowe rozwiązania.</span><span class="sxs-lookup"><span data-stu-id="67858-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="67858-104">Krok 1: Sprawdź, czy 2013 programu SharePoint Designer jest aktualizowany za pomocą [dodatku Service Pack 1 dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2 sierpnia 2016 aktualizacja dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="67858-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="67858-105">Krok 2: Wyczyść pliki lokalnej pamięci podręcznej:</span><span class="sxs-lookup"><span data-stu-id="67858-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="67858-106">Zamknij program SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="67858-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="67858-107">Na komputerze lokalnym Usuń wszystkie pliki Znalezione w każdym z następujących folderów.</span><span class="sxs-lookup"><span data-stu-id="67858-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="67858-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="67858-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="67858-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="67858-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="67858-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="67858-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="67858-111">Otwórz program SharePoint Designer 2013 i wprowadź ponownie konto, aby sprawdzić, czy działa.</span><span class="sxs-lookup"><span data-stu-id="67858-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="67858-112">Krok 3: [Włącz nowoczesnych uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="67858-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="67858-113">Krok 4: Administratorzy będą musieli **zezwolić na niestandardowy skrypt** w ustawieniach centrum administracyjnego programu SharePoint, aby zezwolić na połączenie programu SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="67858-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="67858-114">Aby uzyskać więcej informacji, zobacz [Zezwalanie lub zapobieganie skryptowaniu niestandardowym](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="67858-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


