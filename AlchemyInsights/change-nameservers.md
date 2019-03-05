---
title: Zmienianie serwerów nazw
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 61c4c5e43a247679bf18fd3861dd98fbe9a7b3eb
ms.sourcegitcommit: f1c96fd3890d4e211f7d6bf73b9105fdaab2e11c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2019
ms.locfileid: "30405333"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="2012b-102">Aktualizowanie serwerów nazw domeny do usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="2012b-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="2012b-103">Uwaga: Zmiany nazw czasami może trwać maksymalnie 48 godzin do propagowania.</span><span class="sxs-lookup"><span data-stu-id="2012b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="2012b-p101">Aby skonfigurować domenę w usłudze Office 365, należy zaktualizować serwery nazw u rejestratora. Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="2012b-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="2012b-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="2012b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="2012b-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="2012b-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="2012b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2012b-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="2012b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="2012b-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="2012b-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="2012b-110">Save changes.</span></span>
    
<span data-ttu-id="2012b-111">Szczegółowe instrukcje można także znaleźć w tym artykule: [Zmienianie serwerów nazw w celu skonfigurowania usługi Office 365 u dowolnego rejestratora domen](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="2012b-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

