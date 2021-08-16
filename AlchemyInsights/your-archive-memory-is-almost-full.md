---
title: Archiwalne skrzynki pocztowe są prawie pełne
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046762"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Archiwalne skrzynki pocztowe są prawie pełne

Jeśli użytkownik otrzyma ostrzeżenie; **Archiwalne skrzynki pocztowe są prawie pełne** lub musisz zwiększyć rozmiar ich archiwaalnych skrzynek pocztowych, oto kilka porad:

1. Jeśli użytkownikowi przypisano licencję Exchange Online Plan 1, uaktualnij go do licencji Exchange Online **Plan 2,** aby zwiększyć rozmiar z 50 GB do 100 GB.
1. Jeśli do użytkownika przypisano już jedną z następujących funkcji: **Exchange Online Plan 2** lub Exchange Online Plan 1 z dodatku programu Exchange Online — archiwum, skorzystaj z poniższych instrukcji, aby włączyć automatyczne rozszerzanie archiwizacji:.
 
    1. [Połączenie do Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Uruchom następujące polecenie polecenia dla użytkownika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Uruchom następujące polecenie commandlet, aby potwierdzić, że ta funkcja jest włączona dla użytkownika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Więcej informacji można znaleźć w następującym artykule:

- [Włączanie nieograniczonej archiwizacji — Pomoc dla administratorów — Microsoft 365 dotyczące zgodności | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online — opisy | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Uaktualnianie do innego planu | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

