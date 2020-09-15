---
title: Trwa wygasanie jednego z certyfikatów usług federacyjnych lokalnie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673507"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="5d192-102">Trwa wygasanie jednego z certyfikatów usług federacyjnych lokalnie</span><span class="sxs-lookup"><span data-stu-id="5d192-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="5d192-103">Aby rozwiązać ten problem, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="5d192-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="5d192-104">Zainstaluj moduł Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (Jeśli moduł nie jest jeszcze zainstalowany).</span><span class="sxs-lookup"><span data-stu-id="5d192-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="5d192-105">Aby to zrobić, przejdź do [programu Azure Active Directory PowerShell dla wykresu ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="5d192-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="5d192-106">Postępuj zgodnie z instrukcjami podanymi w sekcji "scenariusz 1: certyfikat podpisywania tokenu usług AD FS wygasł" [w usłudze AD FS — błąd "Wystąpił problem z dostępem do witryny", gdy użytkownik federacyjny loguje się do usługi Microsoft 365, Azure lub Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="5d192-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="5d192-107">Postępuj zgodnie z instrukcjami w temacie [Aktualizowanie lub naprawianie ustawień domeny federacyjnej w programie Microsoft 365, Azure lub Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="5d192-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="5d192-108">Aby uzyskać więcej informacji na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów w usłudze Office 365 i usłudze Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="5d192-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

