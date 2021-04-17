---
title: Nie można zsynchronizować usługi Active Directory
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822861"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="f1f53-102">Nie można zsynchronizować usługi Active Directory</span><span class="sxs-lookup"><span data-stu-id="f1f53-102">Active Directory not syncing</span></span>

<span data-ttu-id="f1f53-103">Jeśli otrzymujesz błędy synchronizacji, takie jak "nie masz ostatniej synchronizacji", lub zwróć uwagę na stan synchronizacji katalogów w portalu administracyjnym pakietu Office o treści "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="f1f53-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="f1f53-104">Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="f1f53-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="f1f53-105">[Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="f1f53-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="f1f53-106">[Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="f1f53-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="f1f53-107">Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz [Azure AD Connect: konta i uprawnienia.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="f1f53-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
