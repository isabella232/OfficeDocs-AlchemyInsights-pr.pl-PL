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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikroopóźnienia lub ograniczanie w programie PowerShell dla usługi Exchange Online

Podczas uruchamiania skryptów i poleceń cmdlet w usłudze Exchange Online mogą zostać wyświetlone ostrzeżenia „Zastosowano mikroopóźnienie” lub wystąpić opóźnienia. Oto dwie sugestie dotyczące tej kwestii:

- Być może zechcesz spróbować skorzystać z modułu [Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), który obsługuje polecenia CMDlet oparte na interfejsie API REST i znacznie bardziej wydajniej. Może to być dobre rozwiązanie w przypadku wielu często używanych poleceń CMDlet Get-.
- Jeśli musisz używać poleceń CMDlet, które nie są objęte modułem w wersji 2, zobacz [Uruchamianie poleceń cmdlet programu PowerShell dla dużej liczby użytkowników w usłudze Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), który zawiera informacje o tym, jak obejść oczekiwane limity ograniczania programu PowerShell dla usługi Exchange Online.
