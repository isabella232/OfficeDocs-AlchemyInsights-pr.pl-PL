---
title: Narzędzie eksportu zbierania elektronicznych materiałów dowodowych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711105"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="742a4-102">Nie można zainstalować lub uruchomić narzędzia eksportu zbierania elektronicznych materiałów dowodowych?</span><span class="sxs-lookup"><span data-stu-id="742a4-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="742a4-103">Jeśli nie możesz zainstalować lub uruchomić narzędzia eksportu zbierania elektronicznych materiałów dowodowych w celu pobrania wyników wyszukiwania, sprawdź następujące elementy:</span><span class="sxs-lookup"><span data-stu-id="742a4-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="742a4-104">Komputer, z którego korzystasz, spełnia następujące wymagania wstępne:</span><span class="sxs-lookup"><span data-stu-id="742a4-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="742a4-105">32-lub 64-bitowe wersje systemu Windows 7 i nowsze wersje</span><span class="sxs-lookup"><span data-stu-id="742a4-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="742a4-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="742a4-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="742a4-107">Obsługiwana przeglądarka:</span><span class="sxs-lookup"><span data-stu-id="742a4-107">A supported browser:</span></span>

  - <span data-ttu-id="742a4-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="742a4-108">Microsoft Edge</span></span>

    <span data-ttu-id="742a4-109">Lub</span><span class="sxs-lookup"><span data-stu-id="742a4-109">Or</span></span>

  - <span data-ttu-id="742a4-110">Internet Explorer 10 i nowsze wersje</span><span class="sxs-lookup"><span data-stu-id="742a4-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="742a4-111">Inne przeglądarki, takie jak Google Chrome i Mozilla Firefox, nie są obsługiwane.</span><span class="sxs-lookup"><span data-stu-id="742a4-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="742a4-112">Twoja organizacja może nawiązać połączenie z punktem końcowym na platformie Azure, czyli \*\* \* BLOB.Core.Windows.NET\*\* (symbol wieloznaczny reprezentuje unikatowy identyfikator zadania eksportu).</span><span class="sxs-lookup"><span data-stu-id="742a4-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="742a4-113">Rola eksportowania jest przypisywana w centrum zgodności zabezpieczeń programu Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="742a4-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="742a4-114">Domyślnie ta rola jest przypisana tylko do grupy ról Menedżera zbierania elektronicznych materiałów dowodowych.</span><span class="sxs-lookup"><span data-stu-id="742a4-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="742a4-115">Zobacz [przypisywanie uprawnień do zbierania elektronicznych materiałów dowodowych](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="742a4-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="742a4-116">Aby uzyskać więcej informacji, zobacz [Eksportowanie wyników wyszukiwania zawartości](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="742a4-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>
  