---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734316"
---
# <a name="verify-your-domain"></a><span data-ttu-id="5a2e2-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="5a2e2-102">Verify your domain</span></span>

 <span data-ttu-id="5a2e2-103">**Prawdopodobnie rekord nie został zaktualizowany przez Internet.**</span><span class="sxs-lookup"><span data-stu-id="5a2e2-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="5a2e2-104">Zazwyczaj możemy zobaczyć nowy rekord już po kilku minutach, ale w niektórych przypadkach może to potrwać nawet kilka godzin.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="5a2e2-105">Jeśli wcześniej zaznaczono już długo, dokładnie sprawdź, czy skopiowano i wkleisz dokładną wartość w rekordzie weryfikującym TXT na hoście DNS.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="5a2e2-106">Jednym z typowych problemów jest pominięcie części „MS=" rekordu.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="5a2e2-107">Ta część jest również potrzebna!</span><span class="sxs-lookup"><span data-stu-id="5a2e2-107">We need that too!</span></span>

- <span data-ttu-id="5a2e2-108">W przypadku niektórych hostów DNS musisz wykonać dodatkowy krok w celu zapisania pliku strefy (w którym jest przechowywany dany rekord DNS), aby został zaktualizowany w Internecie.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="5a2e2-109">Upewnij się, że Zapisano zmiany, aby firma Microsoft mogła sprawdzić i zweryfikować rekord.</span><span class="sxs-lookup"><span data-stu-id="5a2e2-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
