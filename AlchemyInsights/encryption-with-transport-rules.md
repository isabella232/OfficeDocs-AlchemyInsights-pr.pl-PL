---
title: Szyfrowanie z wykorzystaniem reguł transportu
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813878"
---
# <a name="encryption-with-transport-rules"></a>Szyfrowanie z wykorzystaniem reguł transportu

W [centrum administracyjnym programu Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) możesz zastosować funkcję szyfrowania wiadomości pakietu Office w regułach przepływu poczty e-mail, aby wyzwalać szyfrowanie wiadomości. Wybierz opcję **Zastosuj Szyfrowanie wiadomości usługi Office 365 i ochronę praw** w warunku Reguła transportu.

- Aby uzyskać więcej informacji, zobacz [Definiowanie reguł przepływu poczty e-mail na potrzeby szyfrowania](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- W programie Powershell użyj polecenia cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) i ustaw parametr *ApplyOME* jako $true.
