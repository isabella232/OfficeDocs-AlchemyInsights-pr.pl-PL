---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341413"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="efcba-102">Program Outlook nie może połączyć się z folderami publicznymi</span><span class="sxs-lookup"><span data-stu-id="efcba-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="efcba-103">Jeśli dostęp do folderu publicznego nie działa w przypadku niektórym użytkownikom, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="efcba-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="efcba-104">Nawiązywanie połączenia z programem EXO programu PowerShell i Konfigurowanie parametru DefaultPublicFolderMailbox na koncie użytkownika z problemem w celu dopasowania go do parametru na działającym koncie użytkownika.</span><span class="sxs-lookup"><span data-stu-id="efcba-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="efcba-105">Przykłady</span><span class="sxs-lookup"><span data-stu-id="efcba-105">Example:</span></span>

<span data-ttu-id="efcba-106">Get-Skrzynka pocztowa WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="efcba-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="efcba-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="efcba-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="efcba-108">Odczekaj co najmniej godzinę, aby zmiana została uwzględniona.</span><span class="sxs-lookup"><span data-stu-id="efcba-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="efcba-109">Jeśli problem nadal występuje, wykonaj poniższą [procedurę](https://aka.ms/pfcte) , aby rozwiązać problemy z dostępem do folderów publicznych przy użyciu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="efcba-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="efcba-110">**Aby określić, którzy użytkownicy mogą uzyskiwać dostęp do folderów publicznych przy użyciu programu Outlook**:</span><span class="sxs-lookup"><span data-stu-id="efcba-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="efcba-111">Użyj ustawień-Casmailboxhttps <mailboxname> -PublicFolderClientAccess $true lub $false</span><span class="sxs-lookup"><span data-stu-id="efcba-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="efcba-112">$true: Zezwalaj użytkownikom na dostęp do folderów publicznych w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="efcba-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="efcba-113">$false: uniemożliwić użytkownikom dostęp do folderów publicznych w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="efcba-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="efcba-114">Jest to wartość domyślna.</span><span class="sxs-lookup"><span data-stu-id="efcba-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="efcba-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="efcba-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="efcba-116">**Uwaga** Ta procedura może kontrolować połączenia tylko z aplikacją pulpitową programu Outlook dla klientów systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="efcba-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="efcba-117">Użytkownik może nadal uzyskiwać dostęp do folderów publicznych przy użyciu programu OWA lub Outlook dla komputerów Mac.</span><span class="sxs-lookup"><span data-stu-id="efcba-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="efcba-118">Aby uzyskać więcej informacji, zobacz [ogłaszanie obsługi połączeń sterowanych z folderami publicznymi w programie Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="efcba-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>