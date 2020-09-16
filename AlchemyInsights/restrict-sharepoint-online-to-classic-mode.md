---
title: Ograniczanie usługi SharePoint Online do trybu klasycznego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751432"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="f68da-102">Ograniczanie usługi SharePoint Online do trybu klasycznego</span><span class="sxs-lookup"><span data-stu-id="f68da-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="f68da-103">Niektóre organizacje nadal wymagają środowiska klasycznego.</span><span class="sxs-lookup"><span data-stu-id="f68da-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="f68da-104">Chociaż żadne plany nie pozwalają na usunięcie trybu klasycznego na poziomie szczegółowości, nie można już ograniczać całej organizacji (dzierżawy) do trybu klasycznego dla list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="f68da-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="f68da-105">Administrator będzie mógł skorzystać z następujących opcji zarządzania poszczególnymi listami i bibliotekami w trybie klasycznym przy użyciu dostępnych w ten sposób przełączników, które są dostępne na następujących poziomach:</span><span class="sxs-lookup"><span data-stu-id="f68da-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="f68da-106">zbiór witryn</span><span class="sxs-lookup"><span data-stu-id="f68da-106">site collection</span></span>
- <span data-ttu-id="f68da-107">klienta</span><span class="sxs-lookup"><span data-stu-id="f68da-107">site</span></span>
- <span data-ttu-id="f68da-108">Lista</span><span class="sxs-lookup"><span data-stu-id="f68da-108">list</span></span>
- <span data-ttu-id="f68da-109">bibliotece</span><span class="sxs-lookup"><span data-stu-id="f68da-109">library</span></span>

<span data-ttu-id="f68da-110">Ponadto listy korzystające z pewnych funkcji i dostosowań, które nie są obsługiwane przez nowoczesne, będą nadal automatycznie przełączane na tryb klasyczny.</span><span class="sxs-lookup"><span data-stu-id="f68da-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="f68da-111">Począwszy od 1 kwietnia 2019 r., proces wyłączania rezygnacji z nowoczesnej listy i bibliotek będzie można rozpocząć i przejść do 31 maja 2019.</span><span class="sxs-lookup"><span data-stu-id="f68da-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="f68da-112">Listy i biblioteki, które są w trybie klasycznym w wyniku rezygnacji z dzierżawy, zostaną automatycznie przesunięte na nowoczesne.</span><span class="sxs-lookup"><span data-stu-id="f68da-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="f68da-113">Jeśli wymagany jest tryb klasyczny, Zobacz więcej informacji [tutaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i instrukcje programu PowerShell w [tym](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) artykule opisujące opcje i narzędzia, których możesz użyć dzisiaj, aby korzystać z klasycznego środowiska.</span><span class="sxs-lookup"><span data-stu-id="f68da-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
