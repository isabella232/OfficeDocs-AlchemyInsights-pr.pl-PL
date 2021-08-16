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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098576"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikroopóźnienia lub ograniczanie w programie PowerShell dla usługi Exchange Online

Podczas uruchamiania skryptów i poleceń cmdlet w usłudze Exchange Online mogą zostać wyświetlone ostrzeżenia „Zastosowano mikroopóźnienie” lub wystąpić opóźnienia. Oto kilka sugestii, jak rozwiązać ten problem:

- Uruchom naszą diagnostykę, aby zrelaksować się na zasadach ograniczania programu PowerShell Twojej dzierżawy. To rozwiązanie rozwiąże problem w większości przypadków.
- Jeśli problem nadal nie został rozwiązany, skorzystaj z modułu programu PowerShell w wersji Exchange Online w wersji [2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)który zawiera polecenia CMDlet oparte na interfejsie API REST i które są znacznie bardziej performantowe. Może to być dobre rozwiązanie w przypadku wielu często używanych poleceń CMDlet Get-.
- Jeśli chcesz używać poleceń CMDlet, które nie zostały uwzględnione w module v2, zobacz Uruchamianie poleceń [cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)programu PowerShell dla dużej liczby użytkowników w programie Office 365, który zawiera informacje dotyczące sposobu obejmowania limitów ograniczania programu PowerShell w programie Exchange Online.
