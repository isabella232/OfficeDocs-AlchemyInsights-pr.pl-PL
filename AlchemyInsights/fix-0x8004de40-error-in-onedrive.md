---
title: Napraw błąd 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052047"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="06463-102">Napraw błąd 0x8004de40 w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="06463-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="06463-103">Jeśli zostanie wyświetlony błąd 0x8004de40 z OneDrive:</span><span class="sxs-lookup"><span data-stu-id="06463-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="06463-104">Uruchom ponownie komputer, którego dotyczy problem, po podłączeniu do domeny katalogu Acitve.</span><span class="sxs-lookup"><span data-stu-id="06463-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="06463-105">Jeśli ponowne uruchomienie nie rozwiąże problemu, odłączenie i ponowne dołączenie urządzenia z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="06463-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="06463-106">**Uwaga**: podczas wykonywania tych czynności powinieneś być w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="06463-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="06463-107">Nie wykonuj tych czynności, gdy nie możesz nawiązać połączenia z infrastrukturą firmową (na przykład podczas podróży).</span><span class="sxs-lookup"><span data-stu-id="06463-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="06463-108">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień.</span><span class="sxs-lookup"><span data-stu-id="06463-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="06463-109">Aby otworzyć wiersz polecenia z podwyższonym poziomem uprawnień, kliknij przycisk **Start**, kliknij prawym przyciskiem myszy **wiersz polecenia**, a następnie kliknij polecenie **Uruchom jako administrator**.</span><span class="sxs-lookup"><span data-stu-id="06463-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="06463-110">Wpisz *polecenie dsregcmd/Leave* i naciśnij **Enter**.</span><span class="sxs-lookup"><span data-stu-id="06463-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="06463-111">Po zakończeniu wpisz *polecenie dsregcmd/Join* i naciśnij **Enter**.</span><span class="sxs-lookup"><span data-stu-id="06463-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="06463-112">Po zakończeniu Zamknij wiersz polecenia.</span><span class="sxs-lookup"><span data-stu-id="06463-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="06463-113">Uruchom ponownie komputer i zaloguj się do usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="06463-113">Reboot the computer, and log into OneDrive.</span></span>