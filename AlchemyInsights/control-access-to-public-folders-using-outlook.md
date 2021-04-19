---
title: Kontrolowanie dostępu do folderów publicznych za pomocą programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816750"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="18436-102">Kontrolowanie dostępu do folderów publicznych za pomocą programu Outlook</span><span class="sxs-lookup"><span data-stu-id="18436-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="18436-103">Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych za pomocą programu Outlook:</span><span class="sxs-lookup"><span data-stu-id="18436-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="18436-104">Zastosowanie `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="18436-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="18436-105">$true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="18436-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="18436-106">$false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="18436-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="18436-107">Jest to wartość domyślna.</span><span class="sxs-lookup"><span data-stu-id="18436-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="18436-108">Uwaga: Ta procedura może dotyczyć tylko połączeń z programem stacjonarnym Outlook dla klientów systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="18436-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="18436-109">Użytkownicy nadal mogą uzyskać dostęp do folderów publicznych za pomocą aplikacji OWA lub programu Outlook dla komputerów Mac.</span><span class="sxs-lookup"><span data-stu-id="18436-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="18436-110">Aby uzyskać więcej informacji, zobacz [Kontrolowane połączenia z folderami publicznymi w](https://aka.ms/controlpf) programie Outlook, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="18436-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
