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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695297"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="f8d49-102">Pusty ekran logowania w aplikacji Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f8d49-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="f8d49-103">Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="f8d49-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="f8d49-104">Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="f8d49-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="f8d49-105">Resetowanie opcji programu Internet Explorer: Przejdź do **menu Narzędzia**  >  **Opcje internetowe**  >  **Advanced**  >  **Resetowanie ustawień programu Internet Explorer** (Zauważ, że ustawienia niestandardowe zostaną utracone), a następnie ponownie spróbuj zalogować się do pakietu Office.</span><span class="sxs-lookup"><span data-stu-id="f8d49-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="f8d49-106">Wyłącz funkcję Windows Defender Application Guard (WDAG) lub jakąkolwiek podobną zaporę lub program antywirusowy:</span><span class="sxs-lookup"><span data-stu-id="f8d49-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="f8d49-107">W panelu sterowania przejdź do pozycji **programy**, a następnie wybierz pozycję **Włącz lub wyłącz funkcje systemu Windows**.</span><span class="sxs-lookup"><span data-stu-id="f8d49-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="f8d49-108">Jeśli funkcja Windows Defender Application Guard jest włączona, spróbuj ją wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="f8d49-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="f8d49-109">**Uwaga:** Być może będzie konieczne ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="f8d49-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="f8d49-110">Upewnij się, że [wtyczka wam](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BrokerPlugin AAD nie jest blokowana przez żadną aplikację lub zaporę bądź program antywirusowy.</span><span class="sxs-lookup"><span data-stu-id="f8d49-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="f8d49-111">[Wyczyść poświadczenia pakietu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="f8d49-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="f8d49-112">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="f8d49-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f8d49-113">(Np. \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="f8d49-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="f8d49-114">Aby uzyskać więcej informacji, zobacz [problemy z połączeniem po zaktualizowaniu do pakietu Office 2016 kompilacja 16.0.7967 w systemie Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="f8d49-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>