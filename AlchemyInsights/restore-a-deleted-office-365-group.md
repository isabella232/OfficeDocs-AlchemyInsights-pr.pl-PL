---
title: Przywracanie usuniętej grupy platformy Microsoft 365
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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505697"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Przywracanie usuniętej grupy platformy Microsoft 365

Usuniętą grupę platformy Microsoft 365 lub usługę Microsoft Teams możesz przywrócić w ciągu 30 dni od usunięcia.

1. Aby zalogować się do centrum administracyjnego platformy Microsoft 365 i wyświetlić listę usuniętych grup i zespołów, przejdź do centrum administracyjnego platformy [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Uwaga:** Zaloguj się przy użyciu konta przypisanego do administratora dzierżawy lub roli administratora grup.

1. Wybierz usuniętą grupę platformy Microsoft 365/usługę Teams do przywrócenia i kliknij grupę **przywracania.**

    Jeśli nie można przywrócić grupy z powodu konfliktu adresu SMTP, użyj następującego polecenia, aby znaleźć obiekt, który powoduje konflikt, i usunąć adres SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Uwaga:** W niektórych przypadkach przywrócenie grupy i wszystkich jej danych może potrwać nawet 24 godziny.

    Aby uzyskać więcej informacji lub dowiedzieć się, jak przywrócić grupy przy użyciu programu PowerShell, zobacz [Przywracanie usuniętej grupy platformy Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)