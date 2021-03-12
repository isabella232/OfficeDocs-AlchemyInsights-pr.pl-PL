---
title: Problemy z logowaniem się do aplikacji platformy Microsoft 365
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
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709116"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="34ab8-102">Naprawianie komunikatu "Moduł Zaufana platforma komputera nie działa poprawnie" w aplikacjach platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="34ab8-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="34ab8-103">Aby naprawić ten błąd, wypróbuj poniższe rozwiązania:</span><span class="sxs-lookup"><span data-stu-id="34ab8-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="34ab8-104">Zainstaluj najnowsze aktualizacje dla systemu [Windows i](https://support.microsoft.com/help/4027667/windows-10-update) pakietu [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="34ab8-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="34ab8-105">[Wyczyść poświadczenia pakietu Office przy](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="34ab8-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="34ab8-106">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zmieniły się na 16.0.</span><span class="sxs-lookup"><span data-stu-id="34ab8-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="34ab8-107">(Np.: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="34ab8-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="34ab8-108">Wypróbuj proces [odzyskiwania użytkowników, aby](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) naprawić błędy modułu TRUSTED Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="34ab8-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="34ab8-109">Ustaw wartość EnableADAL = 0, korzystając z następujących kroków:</span><span class="sxs-lookup"><span data-stu-id="34ab8-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="34ab8-110">Kliknij prawym przyciskiem myszy przycisk Start systemu Windows, wybierz polecenie **Uruchom,** wpisz **polecenie regedit,** a następnie wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="34ab8-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="34ab8-111">Wybierz **pozycję Tak,** aby zezwolić Edytorowi rejestru na wprowadzanie zmian na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="34ab8-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="34ab8-112">W Edytorze rejestru dodaj wartość DWORD wartości **EnableADAL** z ustawieniem **0** w obszarze HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="34ab8-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="34ab8-113">Aby uzyskać więcej informacji, zobacz Problemy z połączeniem podczas logowania się po aktualizacji do pakietu [Office 2016 kompilacja 16.0.7967 w systemie Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="34ab8-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>