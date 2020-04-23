---
title: Rozwiązywanie problemów z synchronizacją haseł
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732520"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="5cb4b-102">Rozwiązywanie problemów z synchronizacją haseł</span><span class="sxs-lookup"><span data-stu-id="5cb4b-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="5cb4b-103">Aby rozwiązać problemy, w których żadne hasła nie są synchronizowane z usługą Azure AD Connect w wersji 1.1.614.0 lub nowszej:</span><span class="sxs-lookup"><span data-stu-id="5cb4b-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="5cb4b-104">Otwórz nową sesję programu Windows PowerShell na serwerze usługi Azure AD Connect z opcją **Uruchom jako administrator.**</span><span class="sxs-lookup"><span data-stu-id="5cb4b-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="5cb4b-105">Uruchom **Set-ExecutionPolicy RemoteSigned** lub **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="5cb4b-106">Uruchom kreatora usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="5cb4b-107">Przejdź do strony **Zadania dodatkowe,** wybierz pozycję **Rozwiązywanie problemów**i kliknij przycisk **Dalej**.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="5cb4b-108">Na stronie Rozwiązywanie problemów kliknij przycisk **Uruchom, aby uruchomić** menu rozwiązywania problemów w programie PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="5cb4b-109">W menu głównym wybierz pozycję **Rozwiązywanie problemów z synchronizacją haseł**.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="5cb4b-110">W menu podrzędnym wybierz opcję **Synchronizacja haseł w ogóle nie działa**.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="5cb4b-111">**Opis wyników zadania rozwiązywania problemów**</span><span class="sxs-lookup"><span data-stu-id="5cb4b-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="5cb4b-112">Zadanie rozwiązywania problemów wykonuje następujące kontrole:</span><span class="sxs-lookup"><span data-stu-id="5cb4b-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="5cb4b-113">Sprawdza, czy funkcja synchronizacji haseł jest włączona dla dzierżawy usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="5cb4b-114">Sprawdza, czy serwer usługi Azure AD Connect nie jest w trybie przemieszczania.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="5cb4b-115">Dla każdego istniejącego lokalnego łącznika usługi Active Directory (który odpowiada istniejącemu lasowi usługi Active Directory):</span><span class="sxs-lookup"><span data-stu-id="5cb4b-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="5cb4b-116">Sprawdza, czy funkcja synchronizacji haseł jest włączona.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="5cb4b-117">Wyszukuje zdarzenia pulsu synchronizacji haseł w dziennikach zdarzeń aplikacji systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="5cb4b-118">Dla każdej domeny usługi Active Directory w ramach lokalnego łącznika usługi Active Directory:</span><span class="sxs-lookup"><span data-stu-id="5cb4b-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="5cb4b-119">Sprawdza, czy domena jest osiągalna z serwera usługi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="5cb4b-120">Sprawdza, czy konta Usług domenowych Active Directory (AD DS) używane przez lokalny łącznik usługi Active Directory mają poprawną nazwę użytkownika, hasło i uprawnienia wymagane do synchronizacji haseł.</span><span class="sxs-lookup"><span data-stu-id="5cb4b-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="5cb4b-121">Aby uzyskać więcej pomocy w rozwiązywaniu problemów z synchronizacją haseł, zobacz [Rozwiązywanie problemów z synchronizacją haseł za pomocą synchronizacji usługi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="5cb4b-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  