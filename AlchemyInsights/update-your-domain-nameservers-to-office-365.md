---
title: Aktualizowanie serwerów nazw domeny do usługi Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742193"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="16ba7-102">Aktualizowanie serwerów nazw domeny do usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="16ba7-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="16ba7-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="16ba7-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="16ba7-p101">Aby skonfigurować domenę w usłudze Office 365, należy zaktualizować serwery nazw u rejestratora. Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="16ba7-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="16ba7-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="16ba7-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="16ba7-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="16ba7-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="16ba7-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="16ba7-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="16ba7-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="16ba7-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="16ba7-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="16ba7-110">Save changes.</span></span>

<span data-ttu-id="16ba7-111">Szczegółowe instrukcje można także znaleźć w tym artykule: [Zmienianie serwerów nazw w celu skonfigurowania usługi Office 365 u dowolnego rejestratora domen](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="16ba7-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  