---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924706"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="ab98a-102">Rozwiązywanie problemów z synchronizacją haseł</span><span class="sxs-lookup"><span data-stu-id="ab98a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="ab98a-103">Aby rozwiązać problemy, których hasła nie są zsynchronizowane z Azure AD Connect w wersji 1.1.614.0 lub nowszej:</span><span class="sxs-lookup"><span data-stu-id="ab98a-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="ab98a-104">Otwórz sesję środowiska Windows PowerShell na serwerze Azure Połącz AD za pomocą opcji **Uruchom jako Administrator** .</span><span class="sxs-lookup"><span data-stu-id="ab98a-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="ab98a-105">Uruchom **zestaw ExecutionPolicy RemoteSigned** lub **zestaw ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="ab98a-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="ab98a-106">Uruchom kreatora Połącz AD Azure.</span><span class="sxs-lookup"><span data-stu-id="ab98a-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="ab98a-107">Przejdź do \*\* dodatkowe zadania \*\* wybierz \*\* Rozwiązywanie \*\* i kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="ab98a-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="ab98a-108">Na stronie Rozwiązywanie problemów kliknij przycisk **Uruchom, aby uruchomić Rozwiązywanie problemów** menu w programie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ab98a-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="ab98a-109">W menu głównym wybierz **Rozwiązywanie problemów z synchronizacją haseł**.</span><span class="sxs-lookup"><span data-stu-id="ab98a-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="ab98a-110">W podmenu wybierz **Synchronizacja haseł nie działać wcale**.</span><span class="sxs-lookup"><span data-stu-id="ab98a-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="ab98a-111">**Zrozumieć wyniki zadań rozwiązywania problemów**</span><span class="sxs-lookup"><span data-stu-id="ab98a-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="ab98a-112">Zadania dotyczące rozwiązywania problemów, wykonuje następujące kontrole:</span><span class="sxs-lookup"><span data-stu-id="ab98a-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="ab98a-113">Sprawdza, czy funkcja synchronizacji hasła jest włączona dla dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ab98a-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="ab98a-114">Sprawdza, czy serwer Azure Połącz AD nie jest w trybie tymczasowej.</span><span class="sxs-lookup"><span data-stu-id="ab98a-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="ab98a-115">Dla każdego istniejącego lokalnego łącznika usługi Active Directory (która odnosi się do istniejącego lasu usługi Active Directory):</span><span class="sxs-lookup"><span data-stu-id="ab98a-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="ab98a-116">Walidacja będzie przeprowadzana, że włączona jest funkcja synchronizacji hasła.</span><span class="sxs-lookup"><span data-stu-id="ab98a-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="ab98a-117">Wyszukuje hasło synchronizacji pulsu zdarzenia w dzienniku zdarzeń aplikacji systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="ab98a-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="ab98a-118">Dla każdej domeny usługi Active Directory w lokalnym łącznika usługi Active Directory:</span><span class="sxs-lookup"><span data-stu-id="ab98a-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="ab98a-119">Weryfikuje, że domena jest dostępne z serwera Azure Połącz AD.</span><span class="sxs-lookup"><span data-stu-id="ab98a-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="ab98a-120">Sprawdza, czy konta Usługi domenowe w usłudze Active Directory (AD DS), używane przez łącznik usługi Active Directory na lokalnym ma poprawną nazwę użytkownika, hasło i uprawnienia wymagane dla synchronizacji haseł.</span><span class="sxs-lookup"><span data-stu-id="ab98a-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="ab98a-121">Aby uzyskać pomoc, rozwiązywanie problemów z synchronizacji haseł zobacz [Rozwiązywanie problemów z synchronizacji haseł z Azure AD Connect synchronizacją](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="ab98a-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

