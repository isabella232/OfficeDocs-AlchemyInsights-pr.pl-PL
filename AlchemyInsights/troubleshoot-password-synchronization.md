---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664936"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="917a1-102">Rozwiązywanie problemów z synchronizacją haseł</span><span class="sxs-lookup"><span data-stu-id="917a1-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="917a1-103">Aby rozwiązać problemy z synchronizacją haseł, zacznij korzystać z tego zadania rozwiązywania problemów z usługą AAD Connect w celu określenia, dlaczego hasła nie są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="917a1-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="917a1-104">Aby rozpocząć, przejdź do obszaru [Zarządzanie synchronizacją bezpośrednią](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="917a1-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="917a1-105">Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect, a następnie wybierz opcję **Uruchom jako administrator** .</span><span class="sxs-lookup"><span data-stu-id="917a1-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="917a1-106">Uruchom polecenie Set-ExecutionPolicy RemoteSigned lub Set-ExecutionPolicy bez ograniczeń.</span><span class="sxs-lookup"><span data-stu-id="917a1-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="917a1-107">Uruchom Kreatora usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="917a1-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="917a1-108">Przejdź do strony zadania dodatkowe > **rozwiązywania problemów**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="917a1-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="917a1-109">Wybierz pozycję **Uruchom** , aby otworzyć menu Rozwiązywanie problemów z programem PowerShell.</span><span class="sxs-lookup"><span data-stu-id="917a1-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="917a1-110">Wybierz pozycję **Rozwiązywanie problemów z synchronizacją haseł**.</span><span class="sxs-lookup"><span data-stu-id="917a1-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="917a1-111">Przyczyną problemu jest zwykle niezsynchronizowane hasło dla określonego konta użytkownika.</span><span class="sxs-lookup"><span data-stu-id="917a1-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="917a1-112">**Uwagi** Synchronizacja haseł kończy się niepowodzeniem, jeśli Ostatnia pomyślna synchronizacja hasła była niedawna.</span><span class="sxs-lookup"><span data-stu-id="917a1-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="917a1-113">Aby uzyskać więcej pomocy dotyczącej rozwiązywania problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją skrótu hasła za pomocą funkcji synchronizacji Azure](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="917a1-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>