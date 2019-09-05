---
title: Napraw błąd 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755858"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a82f8-102">Napraw błąd 0x8004de40 w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="a82f8-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a82f8-103">Jeśli zostanie wyświetlony błąd 0x8004de40 z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a82f8-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a82f8-104">Uruchom ponownie komputer, którego dotyczy problem, po podłączeniu do domeny katalogu Acitve.</span><span class="sxs-lookup"><span data-stu-id="a82f8-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a82f8-105">Jeśli ponowne uruchomienie nie rozwiąże problemu, odłączenie i ponowne dołączenie urządzenia z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a82f8-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a82f8-106">**Uwaga**: podczas wykonywania tych czynności powinieneś być w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="a82f8-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a82f8-107">Nie wykonuj tych czynności, gdy nie możesz nawiązać połączenia z infrastrukturą firmową (na przykład podczas podróży).</span><span class="sxs-lookup"><span data-stu-id="a82f8-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="a82f8-108">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień.</span><span class="sxs-lookup"><span data-stu-id="a82f8-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="a82f8-109">Aby otworzyć wiersz polecenia z podwyższonym poziomem uprawnień, kliknij przycisk **Start**, kliknij prawym przyciskiem myszy **wiersz polecenia**, a następnie kliknij polecenie **Uruchom jako administrator**.</span><span class="sxs-lookup"><span data-stu-id="a82f8-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="a82f8-110">Wpisz *polecenie dsregcmd/Leave* i naciśnij **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a82f8-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="a82f8-111">Po zakończeniu wpisz *polecenie dsregcmd/Join* i naciśnij **Enter**.</span><span class="sxs-lookup"><span data-stu-id="a82f8-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="a82f8-112">Po zakończeniu Zamknij wiersz polecenia.</span><span class="sxs-lookup"><span data-stu-id="a82f8-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="a82f8-113">Uruchom ponownie komputer i zaloguj się do usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a82f8-113">Reboot the computer, and log into OneDrive.</span></span>