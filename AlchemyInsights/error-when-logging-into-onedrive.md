---
title: błąd 0x8004de40 podczas uruchamiania usługi OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813662"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="35c2e-102">błąd 0x8004de40 podczas uruchamiania usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="35c2e-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="35c2e-103">Jeśli podczas logowania się **do usługi** OneDrive 0x8004de40 komunikat o błędzie, uruchom ponownie komputer, gdy komputer jest połączony z domeną służbowej lub szkolnej.</span><span class="sxs-lookup"><span data-stu-id="35c2e-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="35c2e-104">Jeśli po ponownym uruchomieniu komputera zostanie wyświetlony ten błąd, spróbuj wykonać tę próbę, gdy komputer jest połączony z domeną służbowej lub szkolnej:</span><span class="sxs-lookup"><span data-stu-id="35c2e-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="35c2e-105">Kliknij przycisk Start i wpisz **cmd** lub **wiersz** polecenia w polu wyszukiwania, kliknij prawym przyciskiem myszy aplikację wiersza polecenia i wybierz **pozycję Uruchom jako administrator.**</span><span class="sxs-lookup"><span data-stu-id="35c2e-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="35c2e-106">Jeśli zostanie wyświetlony monit o hasło administratora lub potwierdzenie, wpisz hasło lub kliknij przycisk **Zezwalaj**.</span><span class="sxs-lookup"><span data-stu-id="35c2e-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="35c2e-107">W oknie Wiersz polecenia wpisz **dsregcmd /leave**  i poczekaj na ukończenie polecenia.</span><span class="sxs-lookup"><span data-stu-id="35c2e-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="35c2e-108">Następnie wpisz **dsregcmd /join** i poczekaj na ukończenie polecenia.</span><span class="sxs-lookup"><span data-stu-id="35c2e-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="35c2e-109">Uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="35c2e-109">Reboot your computer.</span></span>
