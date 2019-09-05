---
title: Wygasający certyfikat Federacji programu ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737199"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="f2f34-102">Wygasający certyfikat Federacji programu ADFS</span><span class="sxs-lookup"><span data-stu-id="f2f34-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="f2f34-103">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="f2f34-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="f2f34-104">Zainstaluj Microsoft Azure Active Directory moduł dla środowiska Windows PowerShell na komputerze (Jeśli moduł nie jest jeszcze zainstalowany).</span><span class="sxs-lookup"><span data-stu-id="f2f34-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f2f34-105">Aby to zrobić, przejdź do [zarządzania Azure AD przy użyciu środowiska Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="f2f34-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="f2f34-106">Wykonaj kroki opisane w sekcji "scenariusz 1: certyfikat podpisywania tokenu usług AD FS wygasł" błąd "wystąpił [problem podczas uzyskiwania dostępu do witryny" z usług AD FS, gdy użytkownik federacyjny loguje się do pakietu Office 365, Azure lub Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="f2f34-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="f2f34-107">Wykonaj kroki opisane w [Aktualizowanie lub naprawianie ustawień domeny federacyjnej w pakiecie Office 365, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="f2f34-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="f2f34-108">Aby dowiedzieć się więcej na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów federacyjnych dla pakietu Office 365 i usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="f2f34-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
