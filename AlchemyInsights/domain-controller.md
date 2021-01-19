---
title: Kontroler domeny
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901309"
---
# <a name="domain-controller"></a><span data-ttu-id="06359-102">Kontroler domeny</span><span class="sxs-lookup"><span data-stu-id="06359-102">Domain controller</span></span>

<span data-ttu-id="06359-103">**Nie można włączyć usługi AAD — w usłudze domenowych lub rozmieszczeniu jest niepowodzenie**</span><span class="sxs-lookup"><span data-stu-id="06359-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="06359-104">Aby rozwiązać problem z usługą domenowych w usłudze Azure AD (AAD-DS), która nie jest włączona lub nie ma zostać wdrożona, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="06359-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="06359-105">Jeśli używasz już istniejącej sieci wirtualnej, zapoznaj się z NSG, aby uzyskać reguły blokujące porty potrzebne do synchronizacji w usłudze AAD-DS w portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="06359-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="06359-106">Sprawdź, czy w tym przewodniku podczas rozwiązywania problemów jest dostępny komunikat o błędzie  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="06359-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="06359-107">Spróbuj wdrożyć usługi domenowe w usłudze Azure AD w nowej sieci wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="06359-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="06359-108">Postępuj zgodnie z instrukcjami dotyczącymi wdrażania usługi AAD-DS, która jest dostępna w [samouczku dotyczącego tworzenia usług domenowych w usłudze Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="06359-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="06359-109">Jeśli masz problemy z wdrażaniem usług domenowych w usłudze Azure AD, zobacz [Rozwiązywanie problemów z usługami domenowymi usługi Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , aby rozwiązać typowe błędy ułatwiające ponowne rozpoczęcie pracy.</span><span class="sxs-lookup"><span data-stu-id="06359-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="06359-110">**Nie można wyłączyć usługi AAD — DS**</span><span class="sxs-lookup"><span data-stu-id="06359-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="06359-111">Nie można wstrzymać usługi AAD — DS.</span><span class="sxs-lookup"><span data-stu-id="06359-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="06359-112">Jeśli chcesz zatrzymać korzystanie z domeny zarządzanej, należy ją usunąć.</span><span class="sxs-lookup"><span data-stu-id="06359-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="06359-113">Jeśli występują problemy, aby rozwiązać typowe komunikaty o błędach i skojarzone kroki rozwiązywania problemów ułatwiające ponowne uruchomienie uruchamiania, zobacz [Rozwiązywanie problemów z usługami domenowymi Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="06359-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
