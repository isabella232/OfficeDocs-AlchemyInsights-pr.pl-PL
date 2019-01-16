---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304678"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="60b61-102">Rozwiązywanie problemów z synchronizacją haseł</span><span class="sxs-lookup"><span data-stu-id="60b61-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="60b61-103">Aby rozwiązać problemy, których hasła nie są zsynchronizowane z Azure AD Connect w wersji 1.1.614.0 lub nowszej:</span><span class="sxs-lookup"><span data-stu-id="60b61-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="60b61-104">Otwórz sesję środowiska Windows PowerShell na serwerze Azure Połącz AD za pomocą opcji **Uruchom jako Administrator** .</span><span class="sxs-lookup"><span data-stu-id="60b61-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="60b61-105">Uruchom **zestaw ExecutionPolicy RemoteSigned** lub **zestaw ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="60b61-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="60b61-106">Uruchom kreatora Połącz AD Azure.</span><span class="sxs-lookup"><span data-stu-id="60b61-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="60b61-107">Przejdź do \*\* dodatkowe zadania \*\* wybierz \*\* Rozwiązywanie \*\* i kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="60b61-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="60b61-108">Na stronie Rozwiązywanie problemów kliknij przycisk **Uruchom, aby uruchomić Rozwiązywanie problemów** menu w programie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="60b61-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="60b61-109">W menu głównym wybierz **Rozwiązywanie problemów z synchronizacją haseł**.</span><span class="sxs-lookup"><span data-stu-id="60b61-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="60b61-110">W podmenu wybierz **Synchronizacja haseł nie działać wcale**.</span><span class="sxs-lookup"><span data-stu-id="60b61-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="60b61-111">**Zrozumieć wyniki zadań rozwiązywania problemów**</span><span class="sxs-lookup"><span data-stu-id="60b61-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="60b61-112">Zadania dotyczące rozwiązywania problemów, wykonuje następujące kontrole:</span><span class="sxs-lookup"><span data-stu-id="60b61-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="60b61-113">Sprawdza, czy funkcja synchronizacji hasła jest włączona dla dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="60b61-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="60b61-114">Sprawdza, czy serwer Azure Połącz AD nie jest w trybie tymczasowej.</span><span class="sxs-lookup"><span data-stu-id="60b61-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="60b61-115">Dla każdego istniejącego lokalnego łącznika usługi Active Directory (która odnosi się do istniejącego lasu usługi Active Directory):</span><span class="sxs-lookup"><span data-stu-id="60b61-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="60b61-116">Walidacja będzie przeprowadzana, że włączona jest funkcja synchronizacji hasła.</span><span class="sxs-lookup"><span data-stu-id="60b61-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="60b61-117">Wyszukuje hasło synchronizacji pulsu zdarzenia w dzienniku zdarzeń aplikacji systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="60b61-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="60b61-118">Dla każdej domeny usługi Active Directory w lokalnym łącznika usługi Active Directory:</span><span class="sxs-lookup"><span data-stu-id="60b61-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="60b61-119">Weryfikuje, że domena jest dostępne z serwera Azure Połącz AD.</span><span class="sxs-lookup"><span data-stu-id="60b61-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="60b61-120">Sprawdza, czy konta Usługi domenowe w usłudze Active Directory (AD DS), używane przez łącznik usługi Active Directory na lokalnym ma poprawną nazwę użytkownika, hasło i uprawnienia wymagane dla synchronizacji haseł.</span><span class="sxs-lookup"><span data-stu-id="60b61-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="60b61-121">Aby uzyskać pomoc, rozwiązywanie problemów z synchronizacji haseł zobacz [Rozwiązywanie problemów z synchronizacji haseł z Azure AD Connect synchronizacją](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="60b61-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

