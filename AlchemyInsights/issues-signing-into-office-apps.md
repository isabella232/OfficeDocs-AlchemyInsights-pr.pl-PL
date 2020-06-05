---
title: Problemy z logowaniem się do aplikacji usługi Microsoft 365
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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579875"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="fb427-102">Naprawianie komunikatu "Moduł Zaufana platforma komputera komputera nie działa prawidłowo"</span><span class="sxs-lookup"><span data-stu-id="fb427-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="fb427-103">Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="fb427-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="fb427-104">Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="fb427-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="fb427-105">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="fb427-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="fb427-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16.0.</span><span class="sxs-lookup"><span data-stu-id="fb427-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="fb427-107">(Np.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="fb427-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="fb427-108">Wypróbuj [proces odzyskiwania użytkownika,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) aby naprawić błędy modułu TPM (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="fb427-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="fb427-109">Ustaw EnableADAL = 0, wykonując następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="fb427-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="fb427-110">Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz polecenie **Uruchom**, wpisz **regedit**, a następnie wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="fb427-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="fb427-111">Wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="fb427-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="fb427-112">W Edytorze rejestru dodaj wartość DWORD **enableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="fb427-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="fb427-113">Aby uzyskać więcej informacji, zobacz [Problemy z połączeniem w logowanie po aktualizacji do pakietu Office 2016 kompilacji 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="fb427-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>