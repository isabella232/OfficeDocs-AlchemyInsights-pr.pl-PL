---
title: Problemy z logowaniem się do aplikacji Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: a1e9844094dd164ca8bd5fb2a196161a5de0282f
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236135"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="ed3f1-102">Problemy z logowaniem się do aplikacji Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ed3f1-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="ed3f1-103">Aby rozwiązać problemy z logowaniem się do aplikacji Microsoft 365, wypróbuj następujące opcje na komputerze, którego dotyczy problem:</span><span class="sxs-lookup"><span data-stu-id="ed3f1-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="ed3f1-104">W przypadku systemu Windows Zobacz [zalecenia dotyczące rozwiązywania typowych problemów z logowaniem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="ed3f1-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="ed3f1-105">Dla komputerów Mac zobacz  [nie można zalogować się do aplikacji Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="ed3f1-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="ed3f1-106">**Porada** Na urządzeniach z systemem Windows możemy zdiagnozować i automatycznie rozwiązać kilka typowych problemów z logowaniem do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ed3f1-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="ed3f1-107">Pobierz i uruchom  **[asystenta odzyskiwania i pomocy technicznej firmy Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** , aby korzystać z naszego narzędzia zautomatyzowanego.</span><span class="sxs-lookup"><span data-stu-id="ed3f1-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="ed3f1-108">**Uwaga:** Wyłączenie nowoczesnego uwierzytelniania (ADAL) lub zarządzania kontami sieci Web (WAM) w celu naprawienia problemów logowania lub aktywacji  **nie jest zalecane**.</span><span class="sxs-lookup"><span data-stu-id="ed3f1-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="ed3f1-109">Jeśli podczas nawiązywania połączenia z programem Microsoft 365 przy użyciu pakietu Office 2013 występują błędy, upewnij się, że [włączono nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="ed3f1-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="ed3f1-110">Aby poznać konkretne akcje rozwiązywania problemów, zobacz:</span><span class="sxs-lookup"><span data-stu-id="ed3f1-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="ed3f1-111">Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="ed3f1-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="ed3f1-112">Nie można zalogować się do konta organizacji, takiego jak pakiet Office 365, Azure lub Intune</span><span class="sxs-lookup"><span data-stu-id="ed3f1-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="ed3f1-113">Jak rozwiązywać problemy z aplikacjami nieobsługującymi przeglądarki, które nie mogą zalogować się do pakietu Office 365, Azure lub Intune</span><span class="sxs-lookup"><span data-stu-id="ed3f1-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="ed3f1-114">Wielokrotne monity o poświadczenia w pakiecie Office</span><span class="sxs-lookup"><span data-stu-id="ed3f1-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)