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
# <a name="your-archive-mailbox-is-almost-full"></a>Archiwum Skrzynka pocztowa jest prawie pełna

Jeśli użytkownik otrzyma ostrzeżenie; **Archiwum Skrzynka pocztowa jest prawie pełna** lub musisz zwiększyć rozmiar swojej skrzynki pocztowej w archiwum, poniżej przedstawiono kilka porad:

1. Jeśli użytkownikowi jest przypisany dodatek Exchange Online (plan 1), uaktualnienie do **usługi Exchange Online (plan 2** ) w celu zwiększenia rozmiaru od 50 GB do 100 GB.
1. Jeśli użytkownikowi przypisano już jedną z następujących opcji: **Exchange Online (plan 2** ) lub Exchange Online (plan 1) z dodatkiem Archiwizacja usługi Exchange Online, wykonaj poniższe czynności, aby włączyć automatyczne rozwijanie archiwizacji:.
 
    1. [Nawiązywanie połączenia z programem Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Uruchom następujące unifiedgroup dla użytkownika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Uruchom następujące unifiedgroup, aby potwierdzić, że jest on włączony dla użytkownika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Aby uzyskać więcej informacji, zobacz:

- [ Włączanie archiwizacji bez ograniczeń — pomoc dla administratorów — zgodność z programem Microsoft 365 | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limity usługi Exchange Online — opisy usług | Dokumenty Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Uaktualnij do innego planu biznesowego | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

