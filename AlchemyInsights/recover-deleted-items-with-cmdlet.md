---
title: Odzyskiwanie usuniętych elementów za pomocą polecenia cmdlet
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835821"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="fabe5-102">Odzyskiwanie usuniętych elementów za pomocą polecenia cmdlet</span><span class="sxs-lookup"><span data-stu-id="fabe5-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="fabe5-103">Aby wyświetlić usunięte elementy w skrzynkach pocztowych, użyj polecenia cmdlet [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="fabe5-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="fabe5-104">Po odnalezieniu usuniętych elementów użyj polecenia cmdlet [Restore-RecoverableItems,](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) aby je przywrócić.</span><span class="sxs-lookup"><span data-stu-id="fabe5-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="fabe5-105">Szczegółowe informacje znajdziesz w [tece Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="fabe5-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="fabe5-106">Aby można było uruchomić to polecenie cmdlet, musisz mieć przypisaną rolę importowania i eksportowania skrzynek pocztowych.</span><span class="sxs-lookup"><span data-stu-id="fabe5-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="fabe5-107">Aby uzyskać więcej informacji, zobacz [Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="fabe5-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
