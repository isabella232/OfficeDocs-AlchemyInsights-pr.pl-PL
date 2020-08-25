---
title: Nadawca nie odbiera wiadomości e-mail wysłanej do grupy Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872028"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Nadawca nie odbiera wiadomości e-mail wysłanej do grupy Microsoft 365

Domyślnie nadawca wiadomości e-mail w grupie Microsoft 365 nie otrzymuje kopii wiadomości w swojej skrzynce odbiorczej, nawet jeśli nadawca jest członkiem grupy.

Użyj tego polecenia programu PowerShell EXO, aby umożliwić nadawcy otrzymywanie kopii wszystkich wiadomości e-mail wysyłanych do grupy Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Aby włączyć ustawienie dla wszystkich skrzynek pocztowych jednocześnie:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Uwaga** Zmiany wprowadzone w tym ustawieniu zaczną obowiązywać w ciągu godziny.