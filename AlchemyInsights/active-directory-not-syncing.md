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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930985"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="a4b09-102">Nie można zsynchronizować usługi Active Directory</span><span class="sxs-lookup"><span data-stu-id="a4b09-102">Active Directory not syncing</span></span>

<span data-ttu-id="a4b09-103">Jeśli otrzymujesz błędy synchronizacji, takie jak "ostatnia synchronizacja", lub zwróć uwagę na stan synchronizacji katalogów w portalu administracyjnym usługi Office "Ostatnia synchronizacja ponad 3 dni temu", może to oznaczać, że program AADConnect ma nieprawidłowe ustawienia lub niewystarczające uprawnienia do przeprowadzenia synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="a4b09-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="a4b09-104">Ponowne zainstalowanie programu AADConnect przy użyciu ustawień ekspresowych może szybko rozwiązać ten problem:</span><span class="sxs-lookup"><span data-stu-id="a4b09-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="a4b09-105">[Pobierz najnowszą wersję programu AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="a4b09-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="a4b09-106">[Postępuj zgodnie z instrukcjami dotyczącymi instalacji ekspresowej.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="a4b09-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="a4b09-107">Program Azure AD Connect można zainstalować w systemie Windows Server 2012 lub nowszym.</span><span class="sxs-lookup"><span data-stu-id="a4b09-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="a4b09-108">Serwer musi być dołączony do domeny i może być kontrolerem domeny lub serwerem członkowskim.</span><span class="sxs-lookup"><span data-stu-id="a4b09-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="a4b09-109">Aby uzyskać pełną listę wymagań Połączenie i wymagań wstępnych usługi Azure AD, zapoznaj się z wymaganiami wstępnymi usługi [Azure AD Połączenie.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="a4b09-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="a4b09-110">Aby uzyskać więcej informacji o kontach usługi AADConnect, zobacz Usługa [Azure AD Połączenie: Konta i uprawnienia.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="a4b09-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
