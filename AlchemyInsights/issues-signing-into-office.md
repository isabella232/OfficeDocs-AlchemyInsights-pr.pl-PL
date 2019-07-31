---
title: Problemy z zalogowaniem się do aplikacji pakietu Office
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938294"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="d2e76-102">Problemy z zalogowaniem się do aplikacji pakietu Office</span><span class="sxs-lookup"><span data-stu-id="d2e76-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="d2e76-103">Aby rozwiązać problemy z logowaniem z aplikacji pakietu Office, wypróbuj następujące rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="d2e76-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="d2e76-104">Usuń wszystkie konta pracy, z wyjątkiem dotkniętych konta, przy użyciu ustawień systemu Windows > **dostępu do pracy i w szkole**.</span><span class="sxs-lookup"><span data-stu-id="d2e76-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d2e76-105">[Wyczyść Office poświadczeń](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="d2e76-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d2e76-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="d2e76-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d2e76-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d2e76-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d2e76-108">Otwórz aplikację pakietu Office, wybierz polecenie **plik** > **konta** > **Wyloguj się**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="d2e76-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d2e76-109">Aby uzyskać szczegółowe informacje zobacz [konta w biurze](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d2e76-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d2e76-110">Dla komputerów Macintosh Zobacz [nie można zalogować się do 2016 pakietu Office dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="d2e76-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="d2e76-111">W przypadku błędów podczas nawiązywania połączenia za pomocą pakietu Office 2013 Office 365, należy włączyć uwierzytelnianie nowoczesnych dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="d2e76-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="d2e76-112">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="d2e76-112">For more information, see:</span></span>
- [<span data-ttu-id="d2e76-113">Nie możesz się zarejestrować usłudze Office 365, Azure lub Intune</span><span class="sxs-lookup"><span data-stu-id="d2e76-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="d2e76-114">Problemy z połączeniem w logowanie po aktualizacji do pakietu Office 2016 budować 16.0.7967 w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="d2e76-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="d2e76-115">"Niestety, innego konta z organizacji jest już zarejestrowany na tym komputerze" w pakiecie Office</span><span class="sxs-lookup"><span data-stu-id="d2e76-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="d2e76-116">Logowanie Rozwiązywanie problemów związanych z uwierzytelnianiem nowoczesnych pakietu Office podczas korzystania z programu ADFS</span><span class="sxs-lookup"><span data-stu-id="d2e76-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)