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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702136"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="6c27c-102">Mikroopóźnienia lub ograniczanie w programie PowerShell dla usługi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6c27c-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="6c27c-103">Podczas uruchamiania skryptów i poleceń cmdlet w usłudze Exchange Online mogą zostać wyświetlone ostrzeżenia „Zastosowano mikroopóźnienie” lub wystąpić opóźnienia.</span><span class="sxs-lookup"><span data-stu-id="6c27c-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="6c27c-104">Oto kilka sugestii, jak rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="6c27c-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="6c27c-105">Uruchom naszą diagnostykę, aby zrelaksować się na zasadach ograniczania programu PowerShell Twojej dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="6c27c-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="6c27c-106">To rozwiązanie rozwiąże problem w większości przypadków.</span><span class="sxs-lookup"><span data-stu-id="6c27c-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="6c27c-107">Jeśli problem nadal nie został rozwiązany, skorzystaj z modułu programu PowerShell w wersji Exchange Online w wersji [2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)który zawiera polecenia CMDlet oparte na interfejsie API REST i które są znacznie bardziej performantowe.</span><span class="sxs-lookup"><span data-stu-id="6c27c-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="6c27c-108">Może to być dobre rozwiązanie w przypadku wielu często używanych poleceń CMDlet Get-.</span><span class="sxs-lookup"><span data-stu-id="6c27c-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="6c27c-109">Jeśli chcesz używać poleceń CMDlet, które nie zostały uwzględnione w module v2, zobacz Uruchamianie poleceń [cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)programu PowerShell dla dużej liczby użytkowników w programie Office 365, który zawiera informacje dotyczące sposobu obejmowania limitów ograniczania programu PowerShell w programie Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6c27c-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
