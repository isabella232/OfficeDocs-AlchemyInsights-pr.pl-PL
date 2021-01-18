---
title: Problem z łączeniem maszyn wirtualnych
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885666"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="2c7b7-102">Problem z łączeniem maszyn wirtualnych</span><span class="sxs-lookup"><span data-stu-id="2c7b7-102">Issue joining VMs</span></span>

<span data-ttu-id="2c7b7-103">Aby wyeliminować problemy występujące podczas próby dołączenia do maszyn wirtualnych, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="2c7b7-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="2c7b7-104">Spróbuj zalogować się przy użyciu formatu **UPN** (na przykład "JoeUser@contoso.com") zamiast formatu **sAMAccountName** ("CONTOSO\joeuser").</span><span class="sxs-lookup"><span data-stu-id="2c7b7-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="2c7b7-105">Upewnij się, że włączono synchronizację haseł, zgodnie z instrukcjami przedstawionymi w przewodniku *wprowadzenie* .</span><span class="sxs-lookup"><span data-stu-id="2c7b7-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="2c7b7-106">Upewnij się, że konto użytkownika, którego dotyczy problem, nie jest kontem zewnętrznym w dzierżawie usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="2c7b7-107">Użytkownicy zewnętrzni nie mogą zalogować się w zarządzanej domenie, ponieważ usługi domenowe w usłudze Azure AD nie mają poświadczeń dla takich kont użytkowników.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="2c7b7-108">Jeśli konto użytkownika, którego dotyczy problem, jest kontem użytkownika tylko w chmurze, upewnij się, że użytkownicy zmienili swoje hasło po włączeniu usług domenowych w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="2c7b7-109">Wykonanie tej czynności powoduje generowanie skrótów poświadczeń wymaganych do generowania usług domenowych w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="2c7b7-110">Jeśli konta użytkowników, których dotyczy problem, są synchronizowane z katalogu lokalnego, upewnij się, że zalecana wersja usługi Azure AD Connect została skonfigurowana w celu przeprowadzania pełnej synchronizacji.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="2c7b7-111">Jeśli po potwierdzeniu kroku 4 nadal występują problemy, wykonaj następujące polecenia na komputerze z synchronizacją:</span><span class="sxs-lookup"><span data-stu-id="2c7b7-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="2c7b7-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="2c7b7-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>