---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710453"
---
# <a name="verify-your-domain"></a><span data-ttu-id="3a46e-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="3a46e-102">Verify your domain</span></span>

 <span data-ttu-id="3a46e-103">**Rekord prawdopodobnie nie został zaktualizowany w Internecie.**</span><span class="sxs-lookup"><span data-stu-id="3a46e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="3a46e-104">Zazwyczaj możemy zobaczyć nowy rekord już po kilku minutach, ale w niektórych przypadkach może to potrwać nawet kilka godzin.</span><span class="sxs-lookup"><span data-stu-id="3a46e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="3a46e-105">Jeśli już tak długo czekałeś, sprawdź, czy skopiowano i wkleiłeś dokładną wartość do rekordu weryfikacji TXT na hoście DNS.</span><span class="sxs-lookup"><span data-stu-id="3a46e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="3a46e-106">Jednym z typowych problemów jest pominięcie części „MS=" rekordu.</span><span class="sxs-lookup"><span data-stu-id="3a46e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="3a46e-107">Ta część jest również potrzebna!</span><span class="sxs-lookup"><span data-stu-id="3a46e-107">We need that too!</span></span>

- <span data-ttu-id="3a46e-108">W przypadku niektórych hostów DNS musisz wykonać dodatkowy krok w celu zapisania pliku strefy (w którym jest przechowywany dany rekord DNS), aby został zaktualizowany w Internecie.</span><span class="sxs-lookup"><span data-stu-id="3a46e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="3a46e-109">Upewnij się, że zmiany zostały zapisane, aby firma Microsoft mogła zobaczyć i zweryfikować rekord.</span><span class="sxs-lookup"><span data-stu-id="3a46e-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
