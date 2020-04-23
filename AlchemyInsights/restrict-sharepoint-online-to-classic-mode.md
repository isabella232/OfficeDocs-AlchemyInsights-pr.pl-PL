---
title: Ograniczanie usługi SharePoint Online do trybu klasycznego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742479"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="2e1fa-102">Ograniczanie usługi SharePoint Online do trybu klasycznego</span><span class="sxs-lookup"><span data-stu-id="2e1fa-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="2e1fa-103">Niektóre organizacje nadal wymagają trybu klasycznego.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="2e1fa-104">Chociaż nie ma planów usunięcia trybu klasycznego na poziomie szczegółowym, nie jest już możliwe ograniczenie całej organizacji (dzierżawy) do trybu klasycznego dla list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="2e1fa-105">Administrator będzie miał następujące opcje zarządzania poszczególnymi listami i bibliotekami w trybie klasycznym przy użyciu szczegółowych przełączników opt-out, które udostępniamy na następujących poziomach:</span><span class="sxs-lookup"><span data-stu-id="2e1fa-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="2e1fa-106">zbiór witryn</span><span class="sxs-lookup"><span data-stu-id="2e1fa-106">site collection</span></span>
- <span data-ttu-id="2e1fa-107">Witryny</span><span class="sxs-lookup"><span data-stu-id="2e1fa-107">site</span></span>
- <span data-ttu-id="2e1fa-108">Listy</span><span class="sxs-lookup"><span data-stu-id="2e1fa-108">list</span></span>
- <span data-ttu-id="2e1fa-109">Biblioteki</span><span class="sxs-lookup"><span data-stu-id="2e1fa-109">library</span></span>

<span data-ttu-id="2e1fa-110">Ponadto listy, które używają niektórych funkcji i dostosowań, które nie są obsługiwane przez nowoczesne, będą nadal automatycznie przełączane do trybu klasycznego.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="2e1fa-111">Od 1 kwietnia 2019 r. rozpocznie się proces wyłączania poziomu dzierżawy z nowoczesnej listy i bibliotek do 31 maja 2019 r.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="2e1fa-112">Listy i biblioteki, które są w trybie klasycznym w wyniku rezygnacji dzierżawy zostaną automatycznie przesunięte na nowoczesne.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="2e1fa-113">Jeśli potrzebujesz trybu klasycznego, zobacz więcej informacji [tutaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i instrukcja PnP Powershell [tutaj,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) która opisuje opcje i narzędzia, których możesz użyć dzisiaj, aby korzystać z trybu klasycznego.</span><span class="sxs-lookup"><span data-stu-id="2e1fa-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
