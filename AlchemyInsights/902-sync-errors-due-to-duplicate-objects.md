---
title: 902 (błędy synchronizacji z powodu zduplikowane obiekty)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483373"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="7d787-102">Błędy synchronizacji ze względu na powielanie obiektów</span><span class="sxs-lookup"><span data-stu-id="7d787-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="7d787-103">Może pojawić się jeden z następujących komunikatów o błędach po zakończeniu synchronizacji katalogów:</span><span class="sxs-lookup"><span data-stu-id="7d787-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="7d787-104">Nie można zaktualizować tego obiektu w witrynie Microsoft Online Services, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w katalogu lokalnym.</span><span class="sxs-lookup"><span data-stu-id="7d787-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="7d787-105">Synchronizowanego obiektu z tym samym adresem proxy już istnieje w katalogu programu Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="7d787-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="7d787-106">Nie można zaktualizować tego obiektu, ponieważ następujące atrybuty skojarzone z tym obiektem wartości, które mogą być już skojarzony z innym obiektem w sieci usługi katalogu lokalnego: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="7d787-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="7d787-107">Aby zidentyfikować i rozwiązać ten problem, Pobierz i uruchom [Narzędzie korygowania błędów IdFix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="7d787-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="7d787-108">Aby uzyskać więcej informacji zobacz [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="7d787-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

