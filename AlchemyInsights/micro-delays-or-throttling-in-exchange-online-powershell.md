---
title: Mikroopóźnienia lub ograniczanie w programie PowerShell dla usługi Exchange Online
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
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830043"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="4fd0a-102">Mikroopóźnienia lub ograniczanie w programie PowerShell dla usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="4fd0a-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="4fd0a-103">Podczas uruchamiania skryptów i poleceń cmdlet w usłudze Exchange Online mogą zostać wyświetlone ostrzeżenia „Zastosowano mikroopóźnienie” lub wystąpić opóźnienia.</span><span class="sxs-lookup"><span data-stu-id="4fd0a-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="4fd0a-104">Oto dwie sugestie dotyczące tej kwestii:</span><span class="sxs-lookup"><span data-stu-id="4fd0a-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="4fd0a-105">Być może zechcesz spróbować skorzystać z modułu [Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), który obsługuje polecenia CMDlet oparte na interfejsie API REST i znacznie bardziej wydajniej.</span><span class="sxs-lookup"><span data-stu-id="4fd0a-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="4fd0a-106">Może to być dobre rozwiązanie w przypadku wielu często używanych poleceń CMDlet Get-.</span><span class="sxs-lookup"><span data-stu-id="4fd0a-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="4fd0a-107">Jeśli musisz używać poleceń CMDlet, które nie są objęte modułem w wersji 2, zobacz [Uruchamianie poleceń cmdlet programu PowerShell dla dużej liczby użytkowników w usłudze Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), który zawiera informacje o tym, jak obejść oczekiwane limity ograniczania programu PowerShell dla usługi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4fd0a-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
