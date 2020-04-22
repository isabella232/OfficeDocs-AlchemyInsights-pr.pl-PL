---
title: 902 (Błędy synchronizacji spowodowane zduplikowanymi obiektami)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767144"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="91fc2-102">Błędy synchronizacji spowodowane duplikatami obiektów</span><span class="sxs-lookup"><span data-stu-id="91fc2-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="91fc2-103">Po zakończeniu synchronizacji katalogów w usłudze Microsoft 365 może zostać wyświetlony jeden z następujących komunikatów o błędach:</span><span class="sxs-lookup"><span data-stu-id="91fc2-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="91fc2-104">Nie można zaktualizować tego obiektu w usługach Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.</span><span class="sxs-lookup"><span data-stu-id="91fc2-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="91fc2-105">Zsynchronizowany obiekt o tym samym adresie serwera proxy już istnieje w katalogu usług Online Services firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="91fc2-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="91fc2-106">Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="91fc2-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="91fc2-107">Aby zidentyfikować i rozwiązać problem, pobierz i uruchom [narzędzie do korygowania błędów IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="91fc2-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="91fc2-108">Aby uzyskać więcej informacji, zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="91fc2-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
