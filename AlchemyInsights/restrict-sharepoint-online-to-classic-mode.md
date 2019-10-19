---
title: Ogranicz usługi SharePoint Online do trybu klasycznego
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752078"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9fe15-102">Ogranicz usługi SharePoint Online do trybu klasycznego</span><span class="sxs-lookup"><span data-stu-id="9fe15-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9fe15-103">Niektóre organizacje nadal wymagają doświadczenia w trybie klasycznym.</span><span class="sxs-lookup"><span data-stu-id="9fe15-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9fe15-104">Chociaż nie ma żadnych planów, aby usunąć Tryb klasyczny na poziomie szczegółowości, nie jest już możliwe ograniczenie całej organizacji (dzierżawcy) do trybu klasycznego dla list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="9fe15-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9fe15-105">Administrator będzie miał następujące opcje zarządzania poszczególnymi listami i bibliotekami w trybie klasycznym przy użyciu szczegółowych przełączników rezygnacji, które oferujemy na następujących poziomach:</span><span class="sxs-lookup"><span data-stu-id="9fe15-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9fe15-106">Kolekcja witryn</span><span class="sxs-lookup"><span data-stu-id="9fe15-106">site collection</span></span>
- <span data-ttu-id="9fe15-107">Witryny</span><span class="sxs-lookup"><span data-stu-id="9fe15-107">site</span></span>
- <span data-ttu-id="9fe15-108">Listy</span><span class="sxs-lookup"><span data-stu-id="9fe15-108">list</span></span>
- <span data-ttu-id="9fe15-109">Biblioteki</span><span class="sxs-lookup"><span data-stu-id="9fe15-109">library</span></span>

<span data-ttu-id="9fe15-110">Ponadto listy, które używają niektórych funkcji i dostosowań, które nie są obsługiwane przez nowoczesne nadal będą automatycznie przełączane do trybu klasycznego.</span><span class="sxs-lookup"><span data-stu-id="9fe15-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9fe15-111">Począwszy od dnia 1 kwietnia 2019, proces, aby wyłączyć poziom dzierżawy zrezygnować z nowoczesnych list i bibliotek rozpocznie się i kontynuować do 31 maja 2019.</span><span class="sxs-lookup"><span data-stu-id="9fe15-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="9fe15-112">Listy i bibliotek, które są w trybie klasycznym w wyniku rezygnacji dzierżawy zostanie automatycznie przesunięty do nowoczesnych.</span><span class="sxs-lookup"><span data-stu-id="9fe15-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="9fe15-113">Jeśli potrzebujesz trybu klasycznego, Zobacz więcej informacji [tutaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i instrukcji programu PowerShell PnP [tutaj](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , który opisuje opcje i narzędzia, których można użyć dzisiaj, aby korzystać z trybu klasycznego doświadczenie.</span><span class="sxs-lookup"><span data-stu-id="9fe15-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
