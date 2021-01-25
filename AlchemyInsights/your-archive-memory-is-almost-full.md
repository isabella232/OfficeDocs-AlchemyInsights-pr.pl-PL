---
title: Archiwum Skrzynka pocztowa jest prawie pełna
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974659"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="38a46-102">Archiwum Skrzynka pocztowa jest prawie pełna</span><span class="sxs-lookup"><span data-stu-id="38a46-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="38a46-103">Jeśli użytkownik otrzyma ostrzeżenie; **Archiwum Skrzynka pocztowa jest prawie pełna** lub musisz zwiększyć rozmiar swojej skrzynki pocztowej w archiwum, poniżej przedstawiono kilka porad:</span><span class="sxs-lookup"><span data-stu-id="38a46-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="38a46-104">Jeśli użytkownikowi jest przypisany dodatek Exchange Online (plan 1), uaktualnienie do **usługi Exchange Online (plan 2** ) w celu zwiększenia rozmiaru od 50 GB do 100 GB.</span><span class="sxs-lookup"><span data-stu-id="38a46-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="38a46-105">Jeśli użytkownikowi przypisano już jedną z następujących opcji: **Exchange Online (plan 2** ) lub Exchange Online (plan 1) z dodatkiem Archiwizacja usługi Exchange Online, wykonaj poniższe czynności, aby włączyć automatyczne rozwijanie archiwizacji:.</span><span class="sxs-lookup"><span data-stu-id="38a46-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="38a46-106">[Nawiązywanie połączenia z programem Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="38a46-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="38a46-107">Uruchom następujące unifiedgroup dla użytkownika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="38a46-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="38a46-108">Uruchom następujące unifiedgroup, aby potwierdzić, że jest on włączony dla użytkownika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="38a46-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="38a46-109">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="38a46-109">For more information see:</span></span>

- [<span data-ttu-id="38a46-110"> Włączanie archiwizacji bez ograniczeń — pomoc dla administratorów — zgodność z programem Microsoft 365 | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="38a46-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="38a46-111">Limity usługi Exchange Online — opisy usług | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="38a46-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="38a46-112">Uaktualnij do innego planu biznesowego | Dokumenty Microsoft</span><span class="sxs-lookup"><span data-stu-id="38a46-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

