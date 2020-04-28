---
title: Szyfrowanie z wykorzystaniem reguł transportu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915170"
---
# <a name="encryption-with-transport-rules"></a>Szyfrowanie z wykorzystaniem reguł transportu

W [centrum administracyjnym programu Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) możesz zastosować funkcję szyfrowania wiadomości pakietu Office w regułach przepływu poczty e-mail, aby wyzwalać szyfrowanie wiadomości. Wybierz opcję **Zastosuj Szyfrowanie wiadomości usługi Office 365 i ochronę praw** w warunku Reguła transportu.

- Aby uzyskać więcej informacji, zobacz [Definiowanie reguł przepływu poczty e-mail na potrzeby szyfrowania](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- W programie Powershell użyj polecenia cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) i ustaw parametr *ApplyOME* jako $true.
