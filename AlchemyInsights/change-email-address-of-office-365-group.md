---
title: Zmienianie adresu e-mail grupy usługi Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283267"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Zmienianie adresu e-mail grupy usługi Microsoft 365

Adres e-mail grupy usługi Microsoft 365 można zmienić za pomocą centrum administracyjnego. Wystarczy wybrać grupę i wybrać @edit adres e-mail.

Można również użyć następującego polecenia EXO PowerShell, aby zmienić podstawowy adres SMTP grupy microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Przykład:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
