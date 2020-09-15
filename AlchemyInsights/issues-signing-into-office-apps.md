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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695189"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="49858-102">Rozwiązywanie problemów z aplikacjami Microsoft 365 "moduł zaufanej platformy na komputerze nie działa prawidłowo"</span><span class="sxs-lookup"><span data-stu-id="49858-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="49858-103">Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="49858-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="49858-104">Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="49858-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="49858-105">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="49858-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="49858-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="49858-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="49858-107">(Np. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="49858-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="49858-108">Spróbuj naprawić błędy modułu TPM (Trusted Platform Module) za pomocą [procesu odzyskiwania](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .</span><span class="sxs-lookup"><span data-stu-id="49858-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="49858-109">Ustaw EnableADAL = 0, wykonując następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="49858-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="49858-110">Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz pozycję **Uruchom**, wpisz ciąg **regedit**, a następnie wybierz przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="49858-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="49858-111">Wybierz pozycję **tak** , aby zezwolić edytorowi rejestru na wprowadzanie zmian na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="49858-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="49858-112">W Edytorze rejestru Dodaj wartość DWORD **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="49858-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="49858-113">Aby uzyskać więcej informacji, zobacz [problemy z połączeniem po zaktualizowaniu do pakietu Office 2016 kompilacja 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="49858-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>