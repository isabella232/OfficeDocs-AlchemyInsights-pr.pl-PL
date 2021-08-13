---
title: Zmienianie adresu e-mail grupy Microsoft 365 lub aplikacji Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995632"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Zmienianie adresu e-mail grupy Microsoft 365 lub Microsoft Teams

Możesz zmienić adres e-mail grupy Microsoft 365 lub Microsoft Teams, korzystając z [Centrum administracyjnego platformy Microsoft 365](https://admin.microsoft.com/). Po prostu zaznacz grupę, a następnie wybierz pozycję @edytuj adres e-mail.

Możesz również użyć następującego polecenia EXO PowerShell, aby zmienić podstawowy adres SMTP grupy Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Przykład: 

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
