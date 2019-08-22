---
title: Naprawianie błędu 0x8004de40 w OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525069"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="55842-102">Naprawianie błędu 0x8004de40 w OneDrive</span><span class="sxs-lookup"><span data-stu-id="55842-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="55842-103">Jeśli komunikat o błędzie 0x8004de40 z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="55842-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="55842-104">Uruchom ponownie dotyczy komputera podłączonego do domeny katalogu substancje czynne.</span><span class="sxs-lookup"><span data-stu-id="55842-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="55842-105">Jeśli ponowny rozruch nie rozwiąże problemu, odłączyć i ponownie dołączyć urządzenie z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="55842-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="55842-106">**Uwaga**: należy zachować w sieci firmowej podczas wykonywania tych kroków.</span><span class="sxs-lookup"><span data-stu-id="55842-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="55842-107">Nie wykonanie tych kroków, gdy nie są w stanie nawiązać połączenia sieci firmowej infrastruktury (na przykład podczas podróży).</span><span class="sxs-lookup"><span data-stu-id="55842-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="55842-108">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień.</span><span class="sxs-lookup"><span data-stu-id="55842-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="55842-109">Aby otworzyć wiersz polecenia, kliknij przycisk - **Start**, kliknij prawym przyciskiem myszy **Wiersz polecenia**, a następnie kliknij **Uruchom jako administrator**.</span><span class="sxs-lookup"><span data-stu-id="55842-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="55842-110">*Dsregcmd /leave* i naciśnij klawisz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="55842-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="55842-111">Po zakończeniu, *wpisz/JOIN dsregcmd* i naciśnij klawisz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="55842-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="55842-112">Po zakończeniu zamknij okno wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="55842-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="55842-113">Uruchom ponownie komputer i zaloguj się do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="55842-113">Reboot the computer, and log into OneDrive.</span></span>