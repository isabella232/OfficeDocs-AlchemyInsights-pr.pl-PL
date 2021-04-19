---
title: Włączanie osadzania starszych okien dialogowych w celu otwierania raportów
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814274"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="1b917-102">Włączanie osadzania starszych okien dialogowych w celu otwierania raportów</span><span class="sxs-lookup"><span data-stu-id="1b917-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="1b917-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="1b917-103">**Symptom**</span></span>

<span data-ttu-id="1b917-104">Użytkownicy nie mogą otwierać raportów.</span><span class="sxs-lookup"><span data-stu-id="1b917-104">Users are unable to open reports.</span></span> <span data-ttu-id="1b917-105">"Coś poszło nie tak.</span><span class="sxs-lookup"><span data-stu-id="1b917-105">"Something has gone wrong.</span></span> <span data-ttu-id="1b917-106">Aby uzyskać więcej szczegółowych informacji, zapoznaj się ze szczegółami technicznymi".</span><span class="sxs-lookup"><span data-stu-id="1b917-106">Check technical details for more details."</span></span>

<span data-ttu-id="1b917-107">**Przyczyna**</span><span class="sxs-lookup"><span data-stu-id="1b917-107">**Cause**</span></span>

<span data-ttu-id="1b917-108">Raporty nie są ładowane w u użytkownika UCI z błędem "Deskryptor formularza ma wartość null lub nie został zdefiniowany".</span><span class="sxs-lookup"><span data-stu-id="1b917-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="1b917-109">Raporty w układzie UCI nadal wymagają starszych okien dialogowych, więc system klienta musi mieć włączoną *funkcjęlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="1b917-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="1b917-110">**Rozwiązanie**</span><span class="sxs-lookup"><span data-stu-id="1b917-110">**Solution**</span></span>

1. <span data-ttu-id="1b917-111">Przejdź do **karty >ustawienia > ustawienia systemu > Ogólne.**</span><span class="sxs-lookup"><span data-stu-id="1b917-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="1b917-112">Ustaw wartość "Włącz osadzanie niektórych starszych okien dialogowych w kliencie przeglądarki Unified Interface" na **wartość Tak.**</span><span class="sxs-lookup"><span data-stu-id="1b917-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
