---
title: Aktualizowanie serwerów nazw domeny, aby wskazywały firmę Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510294"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="88f93-102">Aktualizowanie serwerów nazw domeny, aby wskazywały firmę Microsoft</span><span class="sxs-lookup"><span data-stu-id="88f93-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="88f93-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="88f93-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="88f93-104">Aby skonfigurować domenę w firmie Microsoft, serwery nazw u rejestratora muszą zostać zaktualizowane.</span><span class="sxs-lookup"><span data-stu-id="88f93-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="88f93-105">Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="88f93-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="88f93-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="88f93-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="88f93-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="88f93-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="88f93-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="88f93-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="88f93-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="88f93-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="88f93-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="88f93-110">Save changes.</span></span>

<span data-ttu-id="88f93-111">Szczegółowe instrukcje można również znaleźć w tym artykule: [Zmienianie serwerów nazw w celu skonfigurowania usługi Microsoft 365 z dowolnym rejestratorem domen](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="88f93-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  