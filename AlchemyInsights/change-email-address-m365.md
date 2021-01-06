---
title: Zmienianie adresu e-mail grupy Microsoft 365 lub aplikacji Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756567"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Zmienianie adresu e-mail grupy Microsoft 365 lub Microsoft Teams

Możesz zmienić adres e-mail grupy Microsoft 365 lub Microsoft Teams, korzystając z [Centrum administracyjnego platformy Microsoft 365](https://admin.microsoft.com/). Po prostu zaznacz grupę, a następnie wybierz pozycję @edytuj adres e-mail.

Możesz również użyć następującego polecenia EXO PowerShell, aby zmienić podstawowy adres SMTP grupy Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Przykład: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
