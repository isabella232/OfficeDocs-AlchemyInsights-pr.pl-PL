---
title: Usługa Active Directory nie jest synchronizowana
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697639"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="9f13e-102">Usługa Active Directory nie jest synchronizowana</span><span class="sxs-lookup"><span data-stu-id="9f13e-102">Active Directory not syncing</span></span>

<span data-ttu-id="9f13e-103">Jeśli otrzymujesz błędy synchronizacji, na przykład "Brak ostatniej synchronizacji", lub Zwróć uwagę, że stan synchronizacji katalogów w portalu Office Admin zawiera komunikat "Ostatnia synchronizacja: ponad 3 dni temu", być może AADConnect ma niepoprawne ustawienia lub nie masz wystarczających uprawnień do przeprowadzenia synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="9f13e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="9f13e-104">Ponowna instalacja AADConnect za pomocą ustawień ekspresowych może szybko rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="9f13e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="9f13e-105">[Pobierz najnowszą wersję programu AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="9f13e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="9f13e-106">[Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="9f13e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="9f13e-107">Aby uzyskać więcej informacji na temat kont usługi AADConnect, zobacz [usługa Azure AD Connect: konta i uprawnienia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="9f13e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
