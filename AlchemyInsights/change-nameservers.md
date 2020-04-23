---
title: Zmienianie serwerów nazw
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706765"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="4ec2a-102">Aktualizowanie serwerów nazw domeny, aby wskazywały firmę Microsoft</span><span class="sxs-lookup"><span data-stu-id="4ec2a-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="4ec2a-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="4ec2a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4ec2a-p101">Aby skonfigurować domenę w usłudze Microsoft 365, należy zaktualizować serwery nazw u rejestratora. Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="4ec2a-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4ec2a-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="4ec2a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4ec2a-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="4ec2a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4ec2a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ec2a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4ec2a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ec2a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4ec2a-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="4ec2a-110">Save changes.</span></span>

<span data-ttu-id="4ec2a-111">Szczegółowe instrukcje można także znaleźć w tym artykule: [Zmienianie serwerów nazw u dowolnego rejestratora domen](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4ec2a-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  