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
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506057"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="97022-102">Aktualizowanie serwerów nazw domeny do usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="97022-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="97022-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="97022-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="97022-p101">Aby skonfigurować domenę w usłudze Office 365, należy zaktualizować serwery nazw u rejestratora. Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="97022-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="97022-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="97022-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="97022-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="97022-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="97022-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="97022-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="97022-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="97022-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="97022-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="97022-110">Save changes.</span></span>

<span data-ttu-id="97022-111">Szczegółowe instrukcje można także znaleźć w tym artykule: [Zmienianie serwerów nazw w celu skonfigurowania usługi Office 365 u dowolnego rejestratora domen](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="97022-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  