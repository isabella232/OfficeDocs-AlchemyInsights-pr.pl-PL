---
title: 'Aby skonfigurować automatyczne odpowiadanie na wszystkie wiadomości e-mail Microsoft 365 grupy:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 3ed937d38627c1089c9203550498ce7b21ce01c0c5a2deea7326f8057f5338d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036142"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Aby skonfigurować automatyczne odpowiadanie na wszystkie wiadomości e-mail Microsoft 365 grupy:

**Połączenie programu EXO PowerShell przy użyciu konta administratora dzierżawy i użyj następującego polecenia:**

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> Zmień **nazwę grupymailbox** na nazwę grupy, dla której chcesz skonfigurować automatyczne odpowiadanie.

