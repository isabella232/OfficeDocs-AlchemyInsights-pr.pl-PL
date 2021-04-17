---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819522"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c4acf-102">Program Outlook nie może połączyć się z folderami publicznymi</span><span class="sxs-lookup"><span data-stu-id="c4acf-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c4acf-103">Jeśli niektórzy użytkownicy nie mogą uzyskać dostępu do folderu publicznego, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="c4acf-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="c4acf-104">Połącz się z programem POWERShell programu EXO i skonfiguruj parametr DefaultPublicFolderMailbox na koncie użytkownika problemu, aby dopasować go do parametru na roboczym koncie użytkownika.</span><span class="sxs-lookup"><span data-stu-id="c4acf-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="c4acf-105">Przykład: </span><span class="sxs-lookup"><span data-stu-id="c4acf-105">Example:</span></span>

<span data-ttu-id="c4acf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c4acf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c4acf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="c4acf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c4acf-108">Poczekaj co najmniej godzinę, aby zmiana obowiązywała.</span><span class="sxs-lookup"><span data-stu-id="c4acf-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="c4acf-109">Jeśli problem pozostanie, [](https://aka.ms/pfcte) wykonaj tę procedurę, aby rozwiązać problemy z dostępem do folderu publicznego przy użyciu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4acf-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="c4acf-110">**Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych za pomocą programu Outlook:**</span><span class="sxs-lookup"><span data-stu-id="c4acf-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="c4acf-111">Użyj Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true lub $false</span><span class="sxs-lookup"><span data-stu-id="c4acf-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="c4acf-112">$true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="c4acf-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="c4acf-113">$false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4acf-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="c4acf-114">Jest to wartość domyślna.</span><span class="sxs-lookup"><span data-stu-id="c4acf-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="c4acf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="c4acf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="c4acf-116">**Uwaga** Ta procedura pozwala kontrolować połączenia tylko za pomocą klasycznego programu Outlook dla klientów systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="c4acf-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="c4acf-117">Użytkownik może nadal mieć dostęp do folderów publicznych przy użyciu aplikacji OWA lub Outlook dla komputerów Mac.</span><span class="sxs-lookup"><span data-stu-id="c4acf-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="c4acf-118">Aby uzyskać więcej informacji, zobacz Ogłaszanie obsługi kontrolowanego połączenia z folderami [publicznymi w programie Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="c4acf-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>