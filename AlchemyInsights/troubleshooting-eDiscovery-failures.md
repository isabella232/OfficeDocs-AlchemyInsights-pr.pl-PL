---
title: 1490 — Rozwiązywanie problemów-zbieranie elektronicznych materiałów dowodowych — błędy
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277830"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="7cb7a-102">Rozwiązywanie problemów z błędami wyszukiwania zawartości</span><span class="sxs-lookup"><span data-stu-id="7cb7a-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="7cb7a-103">Czy występują problemy z wyszukiwaniem zawartości lub uzyskiwaniem błędów podczas eksportowania wyników wyszukiwania?</span><span class="sxs-lookup"><span data-stu-id="7cb7a-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="7cb7a-104">Na przykład podczas uruchamiania wyszukiwania są wyświetlane następujące pytania?</span><span class="sxs-lookup"><span data-stu-id="7cb7a-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="7cb7a-105">Błędy CS008 lub CS012</span><span class="sxs-lookup"><span data-stu-id="7cb7a-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="7cb7a-106">Błędy serwera/przekroczenia limitu czasu</span><span class="sxs-lookup"><span data-stu-id="7cb7a-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="7cb7a-107">Wystąpił błąd aplikacji</span><span class="sxs-lookup"><span data-stu-id="7cb7a-107">Application error occurred</span></span>

<span data-ttu-id="7cb7a-108">Jeśli chcesz wyszukiwać lub eksportować wyniki z dużej liczby skrzynek pocztowych (ponad 100 000 skrzynek pocztowych), otrzymujesz błędy eksportu?</span><span class="sxs-lookup"><span data-stu-id="7cb7a-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="7cb7a-109">W przypadku tych typów błędów ponów wyszukiwanie w poszukiwaniu nieuszkodzonych lokalizacji zawartości.</span><span class="sxs-lookup"><span data-stu-id="7cb7a-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="7cb7a-110">Aby uzyskać więcej informacji, zobacz  [ten artykuł](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="7cb7a-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="7cb7a-111">Jeśli eksportujesz więcej niż 100K skrzynek pocztowych, musisz użyć następującego programu PowerShell, aby pobrać wyniki eksportu:  [Eksportowanie wyników z ponad 100K skrzynek pocztowych](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="7cb7a-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
