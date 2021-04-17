---
title: Problemy z logowaniem się do aplikacji platformy Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836613"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="ff284-102">Problemy z logowaniem do aplikacji platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ff284-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="ff284-103">Aby rozwiązać problemy z logowaniem w aplikacjach platformy Microsoft 365, wypróbuj następujące opcje na komputerze, którego dotyczy problem:</span><span class="sxs-lookup"><span data-stu-id="ff284-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="ff284-104">W przypadku systemu Windows zobacz Zalecenia dotyczące rozwiązywania typowych problemów [z logowaniem.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="ff284-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="ff284-105">W przypadku komputerów Mac zobacz  [Nie można zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="ff284-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="ff284-106">**Porada** Na komputerach z systemem Windows możemy diagnozować i automatycznie rozwiązywać wiele typowych problemów z logowaniem do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ff284-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="ff284-107">Pobierz i uruchom  **[Asystenta odzyskiwania i pomocy technicznej dla usługi Office 365](https://aka.ms/SaRA-OfficeSignInScenario)**, aby skorzystać z naszego zautomatyzowanego narzędzia.</span><span class="sxs-lookup"><span data-stu-id="ff284-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="ff284-108">**Uwaga:** Nie zaleca się wyłączania nowoczesnego uwierzytelniania (ADAL, Modern Authentication) ani zarządzania kontem sieci Web (WAM, Web Account Management) w celu rozwiązywania problemów z logowaniem **lub aktywacją.**</span><span class="sxs-lookup"><span data-stu-id="ff284-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="ff284-109">Jeśli podczas nawiązywania połączenia z platformą Microsoft 365 za pomocą pakietu Office 2013 wystąpią błędy, włącz [nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ff284-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="ff284-110">Aby uzyskać szczegółowe działania rozwiązywania problemów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="ff284-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="ff284-111">Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="ff284-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="ff284-112">Nie możesz zalogować się do konta organizacji, takiego jak usługa Office 365, Azure lub Intune</span><span class="sxs-lookup"><span data-stu-id="ff284-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="ff284-113">Jak rozwiązywać problemy z aplikacjami nie przeglądarki, które nie mogą zalogować się do usługi Office 365, platformy Azure lub Intune</span><span class="sxs-lookup"><span data-stu-id="ff284-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="ff284-114">Wielokrotnie wyświetlany jest monit o poświadczenia w psłudze Office</span><span class="sxs-lookup"><span data-stu-id="ff284-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)