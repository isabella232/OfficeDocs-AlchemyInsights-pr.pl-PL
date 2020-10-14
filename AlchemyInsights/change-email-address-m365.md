---
title: Zmienianie adresu e-mail grupy usługi Microsoft 365
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/10/2020
ms.locfileid: "48461947"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Zmienianie adresu e-mail grupy usługi Microsoft 365

Możesz zmienić adres e-mail grupy usługi Microsoft 365 przy użyciu Centrum administracyjnego. Po prostu wybierz grupę i wybierz pozycję @edit adres e-mail.

Za pomocą polecenia programu PowerShell w programie EXO można również zmienić podstawowy adres SMTP grupy Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Przykłady

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
