---
title: 902 (błędy synchronizacji ze względu na zduplikowane obiekty)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737351"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="839e3-102">Błędy synchronizacji ze względu na zduplikowane obiekty</span><span class="sxs-lookup"><span data-stu-id="839e3-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="839e3-103">Po zakończeniu synchronizacji katalogów w programie Microsoft 365 może zostać wyświetlony następujący komunikat o błędzie:</span><span class="sxs-lookup"><span data-stu-id="839e3-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="839e3-104">Nie można zaktualizować tego obiektu w usługach online firmy Microsoft, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.</span><span class="sxs-lookup"><span data-stu-id="839e3-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="839e3-105">Zsynchronizowany obiekt o tym samym adresie serwera proxy już istnieje w katalogu usługi Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="839e3-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="839e3-106">Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="839e3-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="839e3-107">Aby zidentyfikować i rozwiązać problem, Pobierz i uruchom narzędzie do [korygowania błędów w narzędziu narzędzia IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="839e3-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="839e3-108">Aby uzyskać więcej informacji, zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="839e3-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
