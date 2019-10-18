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
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736659"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="33967-102">Aktualizowanie serwerów nazw domeny do usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="33967-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="33967-103">Uwaga: Wprowadzenie zmian w serwerach nazw może potrwać nawet do 48 godzin.</span><span class="sxs-lookup"><span data-stu-id="33967-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="33967-p101">Aby skonfigurować domenę w usłudze Office 365, należy zaktualizować serwery nazw u rejestratora. Utwórz rekordy serwera nazw u rejestratora domen lub przeprowadź ich edycję.</span><span class="sxs-lookup"><span data-stu-id="33967-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="33967-106">Przejdź do witryny internetowej rejestratora domen i znajdź obszar, w którym można edytować serwery nazw.</span><span class="sxs-lookup"><span data-stu-id="33967-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="33967-107">Utwórz lub edytuj dwa rekordy serwera nazw, aby pasowały do tych wartości:</span><span class="sxs-lookup"><span data-stu-id="33967-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="33967-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="33967-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="33967-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="33967-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="33967-110">Zapisywanie zmian.</span><span class="sxs-lookup"><span data-stu-id="33967-110">Save changes.</span></span>

<span data-ttu-id="33967-111">Szczegółowe instrukcje można także znaleźć w tym artykule: [Zmienianie serwerów nazw w celu skonfigurowania usługi Office 365 u dowolnego rejestratora domen](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="33967-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  