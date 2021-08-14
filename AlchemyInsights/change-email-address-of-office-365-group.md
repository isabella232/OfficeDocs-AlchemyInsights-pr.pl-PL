---
title: Zmienianie adresu e-mail Microsoft 365 grupy
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
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930739"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Zmienianie adresu e-mail Microsoft 365 grupy

Możesz zmienić adres e-mail grupy Microsoft 365, korzystając z centrum administracyjnego. Po prostu zaznacz grupę, a następnie wybierz pozycję @edytuj adres e-mail.

Za pomocą polecenia EXO PowerShell możesz również zmienić podstawowy adres SMTP grupy Microsoft 365 serwera:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Przykład: 

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
