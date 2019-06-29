---
title: Ogranicz Online programu SharePoint w trybie klasycznym
ms.author: kirks
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
ms.openlocfilehash: 52c63d8909796f8d0d114a46c5255e4073e8c47d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369783"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="22e80-102">Ogranicz Online programu SharePoint w trybie klasycznym</span><span class="sxs-lookup"><span data-stu-id="22e80-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="22e80-103">Niektóre organizacje nadal wymagają doświadczenia trybie klasycznym.</span><span class="sxs-lookup"><span data-stu-id="22e80-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="22e80-104">Podczas gdy nie ma żadnych planów, aby usunąć trybie klasycznym na najniższym poziomie, nie jest możliwe ograniczenie całej organizacji (dzierżawcy) w trybie klasycznym dla list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="22e80-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="22e80-105">Admin będzie miał następujące opcje, aby zarządzać poszczególnych list i bibliotek w trybie klasycznym za pomocą przełączników zrezygnować granulowanych, które oferujemy na następujących poziomach:</span><span class="sxs-lookup"><span data-stu-id="22e80-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="22e80-106">zbiór witryn</span><span class="sxs-lookup"><span data-stu-id="22e80-106">site collection</span></span>
- <span data-ttu-id="22e80-107">witryny</span><span class="sxs-lookup"><span data-stu-id="22e80-107">site</span></span>
- <span data-ttu-id="22e80-108">listy</span><span class="sxs-lookup"><span data-stu-id="22e80-108">list</span></span>
- <span data-ttu-id="22e80-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="22e80-109">library</span></span>

<span data-ttu-id="22e80-110">Ponadto list, które korzystają z niektórych funkcji i dostosowania, które nie są obsługiwane przez nowoczesne będzie nadal automatycznie przełącza się na tryb klasyczny.</span><span class="sxs-lookup"><span data-stu-id="22e80-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="22e80-111">Począwszy od 1 kwietnia 2019, proces, aby wyłączyć poziom dzierżawy zrezygnować z nowoczesnymi listy i biblioteki uruchomi i kontynuuj pracę 31 maja 2019.</span><span class="sxs-lookup"><span data-stu-id="22e80-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="22e80-112">List i bibliotek, które znajdują się w trybie klasycznym w wyniku rezygnacji dzierżawy zostaną automatycznie przesunięte do nowoczesnego.</span><span class="sxs-lookup"><span data-stu-id="22e80-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="22e80-113">Jeśli wymagasz trybie klasycznym można znaleźć więcej informacji [tutaj](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i instrukcji PnP Powershell [tutaj](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) opisujące opcje i narzędzia można użyć dzisiaj wykorzystać doświadczenie trybie klasycznym.</span><span class="sxs-lookup"><span data-stu-id="22e80-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
