---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387887"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d892e-102">Rozwiązywanie problemów z synchronizacją haseł</span><span class="sxs-lookup"><span data-stu-id="d892e-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d892e-103">Aby rozwiązać problemy z synchronizacją haseł, zacznij od użycia tego zadania rozwiązywania problemów AAD Connect, aby ustalić, dlaczego hasła nie są synchronizowane.</span><span class="sxs-lookup"><span data-stu-id="d892e-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="d892e-104">Aby rozpocząć, przejdź do [zarządzania synchronizacją bezpośrednią](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="d892e-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="d892e-105">Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect i wybierz opcję **Uruchom jako administrator.**</span><span class="sxs-lookup"><span data-stu-id="d892e-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="d892e-106">Uruchom Set-ExecutionPolicy RemoteSigned lub Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="d892e-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="d892e-107">Uruchom kreatora usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d892e-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="d892e-108">Przejdź do strony Zadania dodatkowe > **rozwiąż**  >  **dalej**.</span><span class="sxs-lookup"><span data-stu-id="d892e-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="d892e-109">Wybierz **przycisk Uruchom,** aby otworzyć menu rozwiązywania problemów z programem PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d892e-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="d892e-110">Wybierz **pozycję Rozwiązywanie problemów z synchronizacją haseł**.</span><span class="sxs-lookup"><span data-stu-id="d892e-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="d892e-111">Problem polega zazwyczaj na tym, że hasło nie jest synchronizowane dla określonego konta użytkownika.</span><span class="sxs-lookup"><span data-stu-id="d892e-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="d892e-112">**Uwagi** Synchronizacja haseł kończy się niepowodzeniem, jeśli ostatnia pomyślna synchronizacja hasła miała jakiś czas temu.</span><span class="sxs-lookup"><span data-stu-id="d892e-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="d892e-113">Aby uzyskać więcej pomocy w rozwiązywaniu problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją skrótów haseł z synchronizacją usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d892e-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>