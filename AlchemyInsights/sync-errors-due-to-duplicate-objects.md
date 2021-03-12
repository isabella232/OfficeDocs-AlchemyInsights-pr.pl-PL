---
title: 902 (Błędy synchronizacji spowodowane zduplikowanymi obiektami)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708072"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="8737a-102">Błędy synchronizacji spowodowane zduplikowanymi obiektami</span><span class="sxs-lookup"><span data-stu-id="8737a-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="8737a-103">Po zakończeniu synchronizacji katalogów na usłudze Microsoft 365 może zostać wyświetlony jeden z następujących komunikatów o błędzie:</span><span class="sxs-lookup"><span data-stu-id="8737a-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="8737a-104">Nie można zaktualizować tego obiektu w usługach Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w katalogu lokalnym.</span><span class="sxs-lookup"><span data-stu-id="8737a-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="8737a-105">Obiekt zsynchronizowany z tym samym adresem serwera proxy już istnieje w katalogu usług Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="8737a-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="8737a-106">Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem mają wartości, które mogą być już skojarzone z innym obiektem w lokalnych usługach katalogowych: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="8737a-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="8737a-107">Aby zidentyfikować i rozwiązać ten problem, pobierz i uruchom narzędzie do rozwiązywania problemów [narzędzia DirSync narzędzia IdFix.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="8737a-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="8737a-108">Aby uzyskać więcej informacji, zobacz [ARTYKUŁ KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="8737a-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
