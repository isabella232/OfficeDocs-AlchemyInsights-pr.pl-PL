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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/28/2019
ms.locfileid: "30956007"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="dd050-102">Ogranicz Online programu SharePoint w trybie klasycznym</span><span class="sxs-lookup"><span data-stu-id="dd050-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="dd050-103">Niektóre organizacje nadal wymagają doświadczenia trybie klasycznym.</span><span class="sxs-lookup"><span data-stu-id="dd050-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="dd050-104">Gdy nie ma żadnych planów, aby usunąć trybie klasycznym na najbardziej szczegółowym poziomie, od kwietnia 1,2019, to nie będzie już możliwe ograniczenie całej organizacji (dzierżawcy) w trybie klasycznym dla list i bibliotek.</span><span class="sxs-lookup"><span data-stu-id="dd050-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="dd050-105">Admin będzie miał następujące opcje, aby zarządzać poszczególnych list i bibliotek w trybie klasycznym za pomocą przełączników zrezygnować granulowanych, które oferujemy na następujących poziomach:</span><span class="sxs-lookup"><span data-stu-id="dd050-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="dd050-106">zbiór witryn</span><span class="sxs-lookup"><span data-stu-id="dd050-106">site collection</span></span>
- <span data-ttu-id="dd050-107">witryny</span><span class="sxs-lookup"><span data-stu-id="dd050-107">site</span></span>
- <span data-ttu-id="dd050-108">listy</span><span class="sxs-lookup"><span data-stu-id="dd050-108">list</span></span>
- <span data-ttu-id="dd050-109">Biblioteka</span><span class="sxs-lookup"><span data-stu-id="dd050-109">library</span></span>

<span data-ttu-id="dd050-110">Ponadto list, które korzystają z niektórych funkcji i dostosowania, które nie są obsługiwane przez nowoczesne będzie nadal automatycznie przełącza się na tryb klasyczny.</span><span class="sxs-lookup"><span data-stu-id="dd050-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="dd050-111">Po 1 kwietnia list i bibliotek, które znajdują się w trybie klasycznym w wyniku rezygnacji dzierżawcy automatycznie będą zarządzane na poziomie witryny i poziom listy.</span><span class="sxs-lookup"><span data-stu-id="dd050-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="dd050-112">Jeśli wymagasz trybie klasycznym można znaleźć więcej informacji w tym miejscu i PnP Powershell instrukcja tutaj opisano narzędzia i opcje można użyć dzisiaj do przygotowania do usunięcia dzierżawy poziomu opt-out w dniu 1 kwietnia.</span><span class="sxs-lookup"><span data-stu-id="dd050-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
