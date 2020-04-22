---
title: Problemy z logowaniem się do aplikacji pakietu Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763011"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="a8f84-102">Problemy z logowaniem się do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="a8f84-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="a8f84-103">Aby rozwiązać problemy z logowaniem w aplikacjach pakietu Office, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="a8f84-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="a8f84-104">Usuń wszystkie konta służbowe, z wyjątkiem konta, którego dotyczy problem, korzystając z ustawień systemu Windows > **access work or school**.</span><span class="sxs-lookup"><span data-stu-id="a8f84-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="a8f84-105">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="a8f84-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a8f84-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16.0.</span><span class="sxs-lookup"><span data-stu-id="a8f84-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a8f84-107">(Np.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a8f84-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="a8f84-108">Otwórz aplikację pakietu Office, wybierz pozycję**Account** > **Wyloguj konto** **pliku** > . Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="a8f84-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="a8f84-109">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a8f84-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a8f84-110">Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="a8f84-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="a8f84-111">Jeśli podczas nawiązywania błędów podczas łączenia się z programem Microsoft 365 przy użyciu pakietu Office 2013 wystąpią błędy, włącz nowoczesne uwierzytelnianie dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="a8f84-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="a8f84-112">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="a8f84-112">For more information, see:</span></span>
- [<span data-ttu-id="a8f84-113">Nie można zalogować się do usługi Microsoft 365, azure lub intune</span><span class="sxs-lookup"><span data-stu-id="a8f84-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="a8f84-114">Problemy z połączeniem podczas logowania po aktualizacji do kompilacji pakietu Office 2016 16.0.7967 w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="a8f84-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="a8f84-115">"Niestety, inne konto w organizacji jest już zalogowane na tym komputerze" w pakiecie Office</span><span class="sxs-lookup"><span data-stu-id="a8f84-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="a8f84-116">Rozwiązywanie problemów z logowaniem z nowoczesnym uwierzytelnianiem pakietu Office podczas korzystania z usługi ADFS</span><span class="sxs-lookup"><span data-stu-id="a8f84-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)