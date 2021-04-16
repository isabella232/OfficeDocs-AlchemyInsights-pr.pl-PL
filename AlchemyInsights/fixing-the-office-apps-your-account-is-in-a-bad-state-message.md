---
title: Naprawianie aplikacji platformy Microsoft 365 Twoje konto jest w stanie błędu
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812546"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="88623-102">Naprawianie błędu "Twoje konto jest w złym stanie" w aplikacjach platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="88623-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="88623-103">Aby naprawić ten błąd, wypróbuj następujące opcje na komputerze, którego dotyczy problem:</span><span class="sxs-lookup"><span data-stu-id="88623-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="88623-104">Otwórz aplikację pakietu Office i wybierz **pozycję Konto**  >  **pliku**  >  **Wyloguj się ze wszystkich kont.**</span><span class="sxs-lookup"><span data-stu-id="88623-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="88623-105">Zaloguj się ponownie przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="88623-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="88623-106">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="88623-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="88623-107">[Wyczyść poświadczenia pakietu Office za](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocą Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="88623-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="88623-108">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0.</span><span class="sxs-lookup"><span data-stu-id="88623-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="88623-109">Na przykład\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="88623-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="88623-110">Jeśli podczas nawiązywania połączenia z usługą Office 365 za pomocą pakietu Office 2013 wystąpi błąd, włącz [nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="88623-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="88623-111">Aby uzyskać więcej informacji, zobacz Jak rozwiązywać problemy z aplikacjami nie przeglądarki, które nie mogą zalogować się do platformy [Microsoft 365, platformy Azure lub Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="88623-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

