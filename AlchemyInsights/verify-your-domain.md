---
title: Verify your domain
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
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771001"
---
# <a name="verify-your-domain"></a><span data-ttu-id="816ce-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="816ce-102">Verify your domain</span></span>

 <span data-ttu-id="816ce-103">**Rekord prawdopodobnie nie został zaktualizowany w Internecie.**</span><span class="sxs-lookup"><span data-stu-id="816ce-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="816ce-104">Zazwyczaj możemy zobaczyć nowy rekord już po kilku minutach, ale w niektórych przypadkach może to potrwać nawet kilka godzin.</span><span class="sxs-lookup"><span data-stu-id="816ce-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="816ce-105">Jeśli mi było dużo czasu, sprawdź dokładnie, czy wartość została skopiowana i wklejona do rekordu weryfikacji TXT u Twojego hosta DNS.</span><span class="sxs-lookup"><span data-stu-id="816ce-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="816ce-106">Jednym z typowych problemów jest pominięcie części „MS=" rekordu.</span><span class="sxs-lookup"><span data-stu-id="816ce-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="816ce-107">Ta część jest również potrzebna!</span><span class="sxs-lookup"><span data-stu-id="816ce-107">We need that too!</span></span>

- <span data-ttu-id="816ce-108">W przypadku niektórych hostów DNS musisz wykonać dodatkowy krok w celu zapisania pliku strefy (w którym jest przechowywany dany rekord DNS), aby został zaktualizowany w Internecie.</span><span class="sxs-lookup"><span data-stu-id="816ce-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="816ce-109">Upewnij się, że zmiany zostały zapisane, aby firma Microsoft widziała i zweryfikowała rekord.</span><span class="sxs-lookup"><span data-stu-id="816ce-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
