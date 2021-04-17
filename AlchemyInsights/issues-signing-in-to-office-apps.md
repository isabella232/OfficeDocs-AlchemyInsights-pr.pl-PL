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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833085"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="000ef-102">Rozwiązywanie problemów z aplikacjami platformy Microsoft 365 "Niestety, inne konto z Twojej organizacji jest już zalogowane"</span><span class="sxs-lookup"><span data-stu-id="000ef-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="000ef-103">Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="000ef-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="000ef-104">Usuń wszystkie konta służbowe z wyjątkiem konta, którego dotyczy problem, za pomocą > systemu Windows **uzyskaj dostęp do konta służbowego.**</span><span class="sxs-lookup"><span data-stu-id="000ef-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="000ef-105">[Wyczyść poświadczenia pakietu Office za](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocą Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="000ef-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="000ef-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0.</span><span class="sxs-lookup"><span data-stu-id="000ef-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="000ef-107">(Np.: \Software\Microsoft\Office\16.0\Common\Identity)\)</span><span class="sxs-lookup"><span data-stu-id="000ef-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="000ef-108">Otwórz aplikację pakietu Office, wybierz **pozycję Wyloguj**  >  **się z konta**  >  **pliku**. Następnie zaloguj się przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="000ef-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="000ef-109">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="000ef-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="000ef-110">Jeśli używasz komputera Mac, zobacz temat [Nie mogę zalogować się do aplikacji pakietu Office 2016 dla komputerów Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="000ef-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="000ef-111">Aby uzyskać więcej informacji, zobacz "Niestety, inne konto z Twojej organizacji jest już zalogowane [na tym komputerze" w psłudze Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="000ef-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>