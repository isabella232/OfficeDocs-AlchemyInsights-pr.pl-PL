---
title: Wygasający certyfikat federacji usług ADFS
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
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821961"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="732da-102">Wygasający certyfikat federacji usług ADFS</span><span class="sxs-lookup"><span data-stu-id="732da-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="732da-103">Aby rozwiązać ten problem, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="732da-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="732da-104">Zainstaluj moduł usługi Microsoft Azure Active Directory dla programu Windows PowerShell na komputerze (jeśli moduł nie jest jeszcze zainstalowany).</span><span class="sxs-lookup"><span data-stu-id="732da-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="732da-105">Aby to zrobić, przejdź do tematu [Zarządzanie usługą Azure AD przy użyciu programu Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="732da-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="732da-106">Wykonaj czynności opisane w sekcji "Scenariusz 1: Certyfikat podpisywania tokenu usług AD FS wygasł" w sekcji "Wystąpił problem z dostępem do witryny" z usług AD FS, gdy użytkownik federowany loguje się do platformy [Microsoft 365,](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)platformy Azure lub Intune.</span><span class="sxs-lookup"><span data-stu-id="732da-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="732da-107">Wykonaj czynności opisane w tece Aktualizowanie lub naprawianie ustawień [domeny federacji na platformie Microsoft, Azure lub Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="732da-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="732da-108">Aby dowiedzieć się więcej o odnawianiu certyfikatów federacji, zobacz Odnawianie certyfikatów federacji dla platformy [Microsoft 365 i usługi Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="732da-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
