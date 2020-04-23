---
title: Napraw błąd 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716038"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="6fce5-102">Napraw błąd 0x8004de40 w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="6fce5-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="6fce5-103">Jeśli w usłudze OneDrive zostanie wyświetlony błąd 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="6fce5-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="6fce5-104">Uruchom ponownie komputer, którego dotyczy problem, po podłączeniu do domeny katalogu Acitve.</span><span class="sxs-lookup"><span data-stu-id="6fce5-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="6fce5-105">Jeśli ponowne uruchomienie nie rozwiąże problemu, odłącz urządzenie i dołącz ponownie do urządzenia z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6fce5-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="6fce5-106">**Uwaga:** Podczas wykonywania tych czynności powinien znajdować się w sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="6fce5-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="6fce5-107">Nie wykonuj tych czynności, gdy nie możesz połączyć się z infrastrukturą firmową (na przykład podczas podróży).</span><span class="sxs-lookup"><span data-stu-id="6fce5-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="6fce5-108">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień.</span><span class="sxs-lookup"><span data-stu-id="6fce5-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="6fce5-109">Aby otworzyć wiersz polecenia z podwyższonem poziomem uprawnień, kliknij przycisk - **Start**, kliknij prawym przyciskiem myszy **wiersz polecenia**, a następnie kliknij polecenie Uruchom **jako administrator**.</span><span class="sxs-lookup"><span data-stu-id="6fce5-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="6fce5-110">Wpisz *dsregcmd /leave* i naciśnij **klawisz Enter**.</span><span class="sxs-lookup"><span data-stu-id="6fce5-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="6fce5-111">Po zakończeniu wpisz *dsregcmd /join* i naciśnij **klawisz Enter**.</span><span class="sxs-lookup"><span data-stu-id="6fce5-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="6fce5-112">Po zakończeniu zamknij wiersz polecenia.</span><span class="sxs-lookup"><span data-stu-id="6fce5-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="6fce5-113">Uruchom ponownie komputer i zaloguj się do usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6fce5-113">Reboot the computer, and log into OneDrive.</span></span>