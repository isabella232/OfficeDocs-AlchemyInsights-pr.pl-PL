---
title: Aktualizowanie serwerów nazw domeny, aby wskazywały firmę Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734921"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="992ba-102">Aktualizowanie serwerów nazw domeny, aby wskazywały firmę Microsoft</span><span class="sxs-lookup"><span data-stu-id="992ba-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="992ba-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="992ba-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="992ba-104">Aby skonfigurować domenę w firmie Microsoft, serwery nazw na rejestratorze musi zostać zaktualizowany.</span><span class="sxs-lookup"><span data-stu-id="992ba-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="992ba-105">Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="992ba-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="992ba-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="992ba-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="992ba-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="992ba-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="992ba-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="992ba-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="992ba-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="992ba-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="992ba-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="992ba-110">Save changes.</span></span>

<span data-ttu-id="992ba-111">Szczegółowe instrukcje można znaleźć również w tym artykule: [Zmienianie serwery nazw w celu skonfigurowania usługi Microsoft 365 za pomocą rejestratora domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="992ba-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  