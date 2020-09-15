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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695333"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="0ed09-102">Rozwiązywanie problemów z aplikacjami Microsoft 365 "Niestety, inne konto w Twojej organizacji jest już zalogowane" wiadomość</span><span class="sxs-lookup"><span data-stu-id="0ed09-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="0ed09-103">Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="0ed09-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="0ed09-104">Usuwanie wszystkich kont służbowych z wyjątkiem konta, na którym znajduje się usterka, przy użyciu ustawień systemu Windows > **dostęp do służb lub szkoły**.</span><span class="sxs-lookup"><span data-stu-id="0ed09-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="0ed09-105">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="0ed09-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="0ed09-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="0ed09-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0ed09-107">(Np. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="0ed09-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="0ed09-108">Otwórz aplikację pakietu Office, wybierz **File**pozycję  >  **konto**pliku  >  **Wyloguj**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="0ed09-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="0ed09-109">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="0ed09-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0ed09-110">Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="0ed09-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="0ed09-111">Aby uzyskać więcej informacji, zobacz ["Niestety, inne konto w Twojej organizacji jest już zalogowane na tym komputerze" w pakiecie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="0ed09-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>