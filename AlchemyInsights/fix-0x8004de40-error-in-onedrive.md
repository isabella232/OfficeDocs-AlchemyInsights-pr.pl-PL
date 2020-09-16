---
title: Naprawianie błędu 0x8004de40 w usłudze OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745140"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="0b607-102">Naprawianie błędu 0x8004de40 w usłudze OneDrive</span><span class="sxs-lookup"><span data-stu-id="0b607-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="0b607-103">Jeśli podczas korzystania z usługi OneDrive Wystąpił błąd 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="0b607-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="0b607-104">Uruchom ponownie komputer, którego dotyczy problem, gdy połączysz się z domeną usługi Acitve.</span><span class="sxs-lookup"><span data-stu-id="0b607-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="0b607-105">Jeśli ponowne uruchomienie komputera nie rozwiązało problemu, odłączanie i ponowne dołączanie do urządzenia z usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0b607-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="0b607-106">**Uwaga**: w celu wykonania tych czynności należy korzystać z sieci firmowej.</span><span class="sxs-lookup"><span data-stu-id="0b607-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="0b607-107">Nie wykonuj tych czynności, gdy nie możesz połączyć się z infrastrukturą firmową (na przykład podczas podróży).</span><span class="sxs-lookup"><span data-stu-id="0b607-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="0b607-108">Otwórz wiersz polecenia z podwyższonym poziomem uprawnień.</span><span class="sxs-lookup"><span data-stu-id="0b607-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="0b607-109">Aby otworzyć wiersz polecenia z podwyższonym poziomem uprawnień, kliknij przycisk **Start**, kliknij prawym przyciskiem myszy pozycję **wiersz polecenia**, a następnie kliknij polecenie **Uruchom jako administrator**.</span><span class="sxs-lookup"><span data-stu-id="0b607-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="0b607-110">Wpisz *dsregcmd/Leave* i naciśnij klawisz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="0b607-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="0b607-111">Po zakończeniu wpisz *dsregcmd/Join* i naciśnij klawisz **Enter**.</span><span class="sxs-lookup"><span data-stu-id="0b607-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="0b607-112">Po zakończeniu Zamknij wiersz polecenia.</span><span class="sxs-lookup"><span data-stu-id="0b607-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="0b607-113">Uruchom ponownie komputer i zaloguj się do usługi OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0b607-113">Reboot the computer, and log into OneDrive.</span></span>