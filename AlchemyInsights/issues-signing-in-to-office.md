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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938295"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="ce099-102">Puste — ekran logowania w aplikacjach pakietu Office</span><span class="sxs-lookup"><span data-stu-id="ce099-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="ce099-103">Aby rozwiązać ten problem, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="ce099-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="ce099-104">Zainstaluj najnowsze aktualizacje dla [systemu Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [pakietu Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="ce099-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ce099-105">Resetowanie opcji programu Internet Explorer: Przejdź do **Narzędzia** > **Opcje internetowe** > **Zaawansowane** > **Resetowanie ustawień programu Internet Explorer** (należy zauważyć, że ustawienia niestandardowe zostaną utracone), a następnie spróbuj ponownie zalogować się do urzędu.</span><span class="sxs-lookup"><span data-stu-id="ce099-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="ce099-106">Wyłącz Windows Defender aplikacji Guard (WDAG) lub podobny program zapory lub oprogramowania antywirusowego:</span><span class="sxs-lookup"><span data-stu-id="ce099-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="ce099-107">W Panelu sterowania przejdź do **apletu Programy**, a następnie wybierz polecenie **Włącz lub wyłącz funkcje systemu Windows**.</span><span class="sxs-lookup"><span data-stu-id="ce099-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="ce099-108">Jeśli straży aplikacji systemu Windows Defender jest włączona, spróbuj ją wyłączyć.</span><span class="sxs-lookup"><span data-stu-id="ce099-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="ce099-109">**Uwaga:** Konieczne może być ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="ce099-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="ce099-110">Upewnij się, że Microsoft.AAD.BrokerPlugin [WAM AAD dodatek typu plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie są blokowane przez aplikację lub program zapory/anty-wirus.</span><span class="sxs-lookup"><span data-stu-id="ce099-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="ce099-111">[Wyczyść Office poświadczeń](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) przy użyciu Menedżera poświadczeń systemu Windows.</span><span class="sxs-lookup"><span data-stu-id="ce099-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ce099-112">**Uwaga:** Ścieżki rejestru dla pakietu Office 2016 zostały zmienione na 16,0.</span><span class="sxs-lookup"><span data-stu-id="ce099-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ce099-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ce099-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="ce099-114">Aby uzyskać więcej informacji zobacz [w logowanie po aktualizacji do pakietu Office 2016 build 16.0.7967 w systemie Windows 10 problemy z połączeniem](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="ce099-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>