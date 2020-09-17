---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812557"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="2cc73-102">Program Outlook nie może połączyć się z folderami publicznymi</span><span class="sxs-lookup"><span data-stu-id="2cc73-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="2cc73-103">Jeśli dostęp do folderu publicznego nie działa w przypadku niektórym użytkownikom, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="2cc73-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="2cc73-104">Nawiązywanie połączenia z programem EXO programu PowerShell i Konfigurowanie parametru DefaultPublicFolderMailbox na koncie użytkownika z problemem w celu dopasowania go do parametru na działającym koncie użytkownika.</span><span class="sxs-lookup"><span data-stu-id="2cc73-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="2cc73-105">Przykłady</span><span class="sxs-lookup"><span data-stu-id="2cc73-105">Example:</span></span>

<span data-ttu-id="2cc73-106">Get-Skrzynka pocztowa WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="2cc73-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="2cc73-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="2cc73-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="2cc73-108">Odczekaj co najmniej godzinę, aby zmiana została uwzględniona.</span><span class="sxs-lookup"><span data-stu-id="2cc73-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="2cc73-109">Jeśli problem nadal występuje, wykonaj poniższą [procedurę](https://aka.ms/pfcte) , aby rozwiązać problemy z dostępem do folderów publicznych przy użyciu programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="2cc73-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="2cc73-110">**Aby określić, którzy użytkownicy mogą uzyskiwać dostęp do folderów publicznych przy użyciu programu Outlook**:</span><span class="sxs-lookup"><span data-stu-id="2cc73-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="2cc73-111">Użyj ustawień-Casmailboxhttps <mailboxname> -PublicFolderClientAccess $true lub $false</span><span class="sxs-lookup"><span data-stu-id="2cc73-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="2cc73-112">$true: Zezwalaj użytkownikom na dostęp do folderów publicznych w programie Outlook</span><span class="sxs-lookup"><span data-stu-id="2cc73-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="2cc73-113">$false: uniemożliwić użytkownikom dostęp do folderów publicznych w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="2cc73-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="2cc73-114">Jest to wartość domyślna.</span><span class="sxs-lookup"><span data-stu-id="2cc73-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="2cc73-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="2cc73-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="2cc73-116">**Uwaga** Ta procedura może kontrolować połączenia tylko z aplikacją pulpitową programu Outlook dla klientów systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="2cc73-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="2cc73-117">Użytkownik może nadal uzyskiwać dostęp do folderów publicznych przy użyciu programu OWA lub Outlook dla komputerów Mac.</span><span class="sxs-lookup"><span data-stu-id="2cc73-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="2cc73-118">Aby uzyskać więcej informacji, zobacz [ogłaszanie obsługi połączeń sterowanych z folderami publicznymi w programie Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="2cc73-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>