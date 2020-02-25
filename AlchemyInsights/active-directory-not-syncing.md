---
title: Niesynchronizowanie usługi Active Directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265266"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="165d9-102">Niesynchronizowanie usługi Active Directory</span><span class="sxs-lookup"><span data-stu-id="165d9-102">Active Directory not syncing</span></span>

<span data-ttu-id="165d9-103">Jeśli otrzymujesz błędy synchronizacji, takie jak "brak niedawnej synchronizacji" lub zauważysz stan synchronizacji katalogów w portalu administracyjnym pakietu Office mówi: "Ostatnia synchronizacja sprzed ponad 3 dni", może się okazać, że AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do wykonywania synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="165d9-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="165d9-104">Ponowna instalacja usługi AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać problem:</span><span class="sxs-lookup"><span data-stu-id="165d9-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="165d9-105">[Pobierz najnowszą wersję AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="165d9-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="165d9-106">[Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="165d9-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="165d9-107">Aby uzyskać więcej informacji o kontach usług AADConnect, zobacz [Azure AD Connect: Konta i uprawnienia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="165d9-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
