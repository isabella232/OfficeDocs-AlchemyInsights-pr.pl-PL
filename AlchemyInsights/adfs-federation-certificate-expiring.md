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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737199"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="34b3a-102">Wygasający certyfikat Federacji programu ADFS</span><span class="sxs-lookup"><span data-stu-id="34b3a-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="34b3a-103">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="34b3a-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="34b3a-104">Zainstaluj Microsoft Azure Active Directory moduł dla środowiska Windows PowerShell na komputerze (Jeśli moduł nie jest jeszcze zainstalowany).</span><span class="sxs-lookup"><span data-stu-id="34b3a-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="34b3a-105">Aby to zrobić, przejdź do [zarządzania Azure AD przy użyciu środowiska Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="34b3a-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="34b3a-106">Wykonaj kroki opisane w sekcji "scenariusz 1: certyfikat podpisywania tokenu usług AD FS wygasł" błąd "wystąpił [problem podczas uzyskiwania dostępu do witryny" z usług AD FS, gdy użytkownik federacyjny loguje się do pakietu Office 365, Azure lub Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="34b3a-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="34b3a-107">Wykonaj kroki opisane w [Aktualizowanie lub naprawianie ustawień domeny federacyjnej w pakiecie Office 365, Azure lub Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="34b3a-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="34b3a-108">Aby dowiedzieć się więcej na temat odnawiania certyfikatów federacyjnych, zobacz [Odnawianie certyfikatów federacyjnych dla pakietu Office 365 i usługi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="34b3a-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
