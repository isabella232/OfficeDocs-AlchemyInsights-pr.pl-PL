---
title: Odzyskiwanie usuniętych elementów za pomocą polecenia cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493166"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="f7514-102">Odzyskiwanie usuniętych elementów za pomocą polecenia cmdlet</span><span class="sxs-lookup"><span data-stu-id="f7514-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="f7514-103">Polecenie cmdlet [Get-RecoverAbleItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) służy do wyświetlania usuniętych elementów w skrzynkach pocztowych.</span><span class="sxs-lookup"><span data-stu-id="f7514-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="f7514-104">Po znalezieniu usuniętych elementów, należy użyć polecenia cmdlet [Restore-RecoverItems,](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) aby je przywrócić.</span><span class="sxs-lookup"><span data-stu-id="f7514-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="f7514-105">Zobacz szczegółowe informacje w [get-recoverableitems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f7514-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="f7514-106">Aby można było uruchomić to polecenie cmdlet, należy przypisać rolę Eksportuj skrzynkę pocztową.</span><span class="sxs-lookup"><span data-stu-id="f7514-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="f7514-107">Aby uzyskać więcej [informacji, zobacz Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="f7514-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
