---
title: Konfigurowanie usługi domeny
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885692"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="8a6e1-102">Nie można włączyć usługi AAD — w usłudze domenowych lub rozmieszczeniu jest niepowodzenie</span><span class="sxs-lookup"><span data-stu-id="8a6e1-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="8a6e1-103">Aby rozwiązać problem z usługą domenowych w usłudze Azure AD (AAD-DS), która nie jest włączona lub nie ma zostać wdrożona, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="8a6e1-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="8a6e1-104">Jeśli używasz już istniejącej sieci wirtualnej, zapoznaj się z NSG, aby uzyskać reguły blokujące porty potrzebne do synchronizacji w usłudze AAD-DS w portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="8a6e1-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="8a6e1-105">Sprawdź, czy w tym przewodniku podczas rozwiązywania problemów jest dostępny komunikat o błędzie  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="8a6e1-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="8a6e1-106">Spróbuj wdrożyć usługi domenowe w usłudze Azure AD w nowej sieci wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="8a6e1-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="8a6e1-107">Postępuj zgodnie z przewodnikiem wprowadzenie dotyczącym wdrażania usługi AAD — DS: [Tworzenie i Konfigurowanie usług domenowych w usłudze AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="8a6e1-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="8a6e1-108">Jeśli masz problemy z wdrażaniem usług domenowych w usłudze Azure AD, zobacz [Rozwiązywanie problemów z usługami domenowymi usługi Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , aby rozwiązać typowe błędy ułatwiające ponowne rozpoczęcie pracy.</span><span class="sxs-lookup"><span data-stu-id="8a6e1-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="8a6e1-109">**Nie można wyłączyć usługi AAD — DS**</span><span class="sxs-lookup"><span data-stu-id="8a6e1-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="8a6e1-110">Nie można wstrzymać usługi AAD — DS.</span><span class="sxs-lookup"><span data-stu-id="8a6e1-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="8a6e1-111">Jeśli chcesz zatrzymać korzystanie z domeny zarządzanej, należy ją usunąć.</span><span class="sxs-lookup"><span data-stu-id="8a6e1-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="8a6e1-112">Aby usunąć domenę zarządzaną, zobacz [usuwanie usługi domeny AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="8a6e1-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



