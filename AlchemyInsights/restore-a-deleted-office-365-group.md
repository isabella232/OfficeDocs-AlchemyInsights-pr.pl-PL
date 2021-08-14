---
title: Przywracanie usuniętej Microsoft 365 grupy
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959036"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Przywracanie usuniętej Microsoft 365 grupy

Usunięte elementy można Microsoft 365 lub grupy Microsoft Teams w ciągu 30 dni od usunięcia.

1. Przejdź do [centrum administracyjne platformy Microsoft 365,](https://aka.ms/RestoreDeletedGroup) aby zalogować się do listy usuniętych grup i zespołów.

    **Uwaga:** Zaloguj się przy użyciu konta przypisanego do administratora dzierżawy lub roli administratora grup.

1. Wybierz usunięte grupy Microsoft 365/Teams, które chcesz przywrócić, a następnie kliknij pozycję **przywróć grupę**.

    Jeśli nie można przywrócić grupy z powodu konfliktu adresu SMTP, użyj następującego polecenia, aby znaleźć obiekt, który powoduje konflikt, i usunąć adres SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Uwaga:** W niektórych przypadkach przywrócenie grupy i wszystkich jej danych może potrwać nawet 24 godziny.

    Aby uzyskać więcej informacji lub dowiedzieć się, jak przywrócić grupy przy użyciu programu PowerShell, zobacz Przywracanie usuniętej grupy Microsoft 365 [grupy.](https://go.microsoft.com/fwlink/?linkid=867802)