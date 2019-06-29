---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365427"
---
# <a name="verify-your-domain"></a><span data-ttu-id="27413-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="27413-102">Verify your domain</span></span>

 <span data-ttu-id="27413-103">**Rekord prawdopodobnie nie aktualizowany przez Internet.**</span><span class="sxs-lookup"><span data-stu-id="27413-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="27413-104">Zazwyczaj możemy zobaczyć nowy rekord już po kilku minutach, ale w niektórych przypadkach może to potrwać nawet kilka godzin.</span><span class="sxs-lookup"><span data-stu-id="27413-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="27413-105">Po odczekaniu który już długo, sprawdź już skopiowany i wklejony dokładną wartość do rekordu TXT weryfikacji na hoście DNS.</span><span class="sxs-lookup"><span data-stu-id="27413-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="27413-106">Jednym z typowych problemów jest pominięcie części „MS=" rekordu.</span><span class="sxs-lookup"><span data-stu-id="27413-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="27413-107">Ta część jest również potrzebna!</span><span class="sxs-lookup"><span data-stu-id="27413-107">We need that too!</span></span>

- <span data-ttu-id="27413-108">W przypadku niektórych hostów DNS musisz wykonać dodatkowy krok w celu zapisania pliku strefy (w którym jest przechowywany dany rekord DNS), aby został zaktualizowany w Internecie.</span><span class="sxs-lookup"><span data-stu-id="27413-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="27413-109">Upewnij się, że zmiany zostały zapisane, tak aby usługa Office 365 mogła zobaczyć i zweryfikować rekord.</span><span class="sxs-lookup"><span data-stu-id="27413-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
