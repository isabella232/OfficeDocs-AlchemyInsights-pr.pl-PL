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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645141"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="9add7-102">Przywracanie usuniętej grupy platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9add7-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="9add7-103">Usuniętą grupę platformy Microsoft 365 lub usługę Microsoft Teams możesz przywrócić w ciągu 30 dni od usunięcia.</span><span class="sxs-lookup"><span data-stu-id="9add7-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="9add7-104">Przejdź do centrum [administracyjnego platformy Microsoft 365,](https://aka.ms/RestoreDeletedGroup) aby zalogować się na listę usuniętych grup i zespołów.</span><span class="sxs-lookup"><span data-stu-id="9add7-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="9add7-105">**Uwaga:** Zaloguj się przy użyciu konta przypisanego do administratora dzierżawy lub roli administratora grup.</span><span class="sxs-lookup"><span data-stu-id="9add7-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="9add7-106">Wybierz usuniętą grupę platformy Microsoft 365/usługę Teams do przywrócenia i kliknij grupę **przywracania.**</span><span class="sxs-lookup"><span data-stu-id="9add7-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="9add7-107">Jeśli nie można przywrócić grupy z powodu konfliktu adresu SMTP, użyj następującego polecenia, aby znaleźć obiekt, który powoduje konflikt, i usunąć adres SMTP:</span><span class="sxs-lookup"><span data-stu-id="9add7-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="9add7-108">**Uwaga:** W niektórych przypadkach przywrócenie grupy i wszystkich jej danych może potrwać nawet 24 godziny.</span><span class="sxs-lookup"><span data-stu-id="9add7-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="9add7-109">Aby uzyskać więcej informacji lub dowiedzieć się, jak przywrócić grupy przy użyciu programu PowerShell, zobacz [Przywracanie usuniętej grupy platformy Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="9add7-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>