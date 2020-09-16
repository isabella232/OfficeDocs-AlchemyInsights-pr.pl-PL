---
title: Rozwiązywanie problemów z aplikacjami Microsoft 365 Twoje konto jest w nieprawidłowym stanie
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744555"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="8aebd-102">Błąd podczas rozwiązywania problemów z aplikacjami Microsoft 365 "Twoje konto jest w nieprawidłowym stanie"</span><span class="sxs-lookup"><span data-stu-id="8aebd-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="8aebd-103">Aby rozwiązać ten problem, wypróbuj następujące opcje na komputerze, którego dotyczy problem:</span><span class="sxs-lookup"><span data-stu-id="8aebd-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="8aebd-104">Otwórz aplikację pakietu Office, wybierz **File**pozycję  >  **konto**plików  >  **Wyloguj się z wszystkich kont**.</span><span class="sxs-lookup"><span data-stu-id="8aebd-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="8aebd-105">Zaloguj się ponownie przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="8aebd-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="8aebd-106">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8aebd-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8aebd-107">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="8aebd-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="8aebd-108">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="8aebd-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8aebd-109">Na przykład \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="8aebd-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="8aebd-110">Jeśli podczas nawiązywania połączenia z pakietem Office 365 przy użyciu pakietu Office 2013 wystąpi błąd, [Włącz nowoczesne uwierzytelnianie](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="8aebd-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="8aebd-111">Aby uzyskać więcej informacji, zobacz [Rozwiązywanie problemów z aplikacjami nieobsługującymi przeglądarki, które nie mogą zalogować się do aplikacji Microsoft 365, Azure lub Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="8aebd-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

