---
title: Naprawianie aplikacji pakietu Office Twoje konto jest w złym stanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969671"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="62816-102">Naprawianie błędu aplikacji pakietu Office "Twoje konto jest w złym stanie"</span><span class="sxs-lookup"><span data-stu-id="62816-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="62816-103">Aby naprawić ten błąd, wypróbuj następujące opcje na komputerze, którego dotyczy problem:</span><span class="sxs-lookup"><span data-stu-id="62816-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="62816-104">Otwórz aplikację pakietu Office, wybierz pozycję**Wyloguj\*\*\*\*konto** >  **pliku** > wszystkich kont .</span><span class="sxs-lookup"><span data-stu-id="62816-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="62816-105">Zaloguj się ponownie przy użyciu konta użytkownika z ważną licencją.</span><span class="sxs-lookup"><span data-stu-id="62816-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="62816-106">Aby uzyskać szczegółowe informacje, zobacz [Konta w pakiecie Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="62816-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="62816-107">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="62816-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="62816-108">**Uwaga:** Ścieżki rejestru pakietu Office 2016 zostały zmienione na 16.0.</span><span class="sxs-lookup"><span data-stu-id="62816-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="62816-109">Na przykład \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="62816-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="62816-110">Na komputerze, którego dotyczy problem, ustaw enableadal = 0, wykonując następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="62816-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="62816-111">Kliknij prawym przyciskiem myszy przycisk Windows i wybierz polecenie **Uruchom**.</span><span class="sxs-lookup"><span data-stu-id="62816-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="62816-112">W polu **Otwórz** wpisz **regedit,** a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="62816-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="62816-113">Po wyświetleniu monitu wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="62816-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="62816-114">W Edytorze rejestru dodaj wartość DWORD EnableADAL z ustawieniem 0 w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="62816-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="62816-115">Jeśli podczas łączenia się z usługi Office 365 przy użyciu pakietu Office 2013 wystąpi błąd, [włącz nowoczesne uwierzytelnianie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) dla klienta pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="62816-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="62816-116">Aby uzyskać więcej informacji, zobacz [Jak rozwiązywać problemy z aplikacjami nieprzeglądarkowymi, które nie mogą zalogować się do usługi Office 365, platformy Azure lub usługi Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="62816-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

