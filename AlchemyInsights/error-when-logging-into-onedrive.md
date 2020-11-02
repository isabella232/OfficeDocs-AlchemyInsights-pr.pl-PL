---
title: 0x8004de40 błąd podczas uruchamiania usługi OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823113"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="a25a0-102">0x8004de40 błąd podczas uruchamiania usługi OneDrive</span><span class="sxs-lookup"><span data-stu-id="a25a0-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="a25a0-103">Jeśli podczas logowania do usługi OneDrive zostanie wyświetlony komunikat o błędzie **0x8004de40** , uruchom ponownie komputer po połączeniu z domeną służbową lub szkolną.</span><span class="sxs-lookup"><span data-stu-id="a25a0-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="a25a0-104">Jeśli po ponownym uruchomieniu komputera pojawi się ten błąd, spróbuj wykonać tę czynność po połączeniu z domeną służbową lub szkolną:</span><span class="sxs-lookup"><span data-stu-id="a25a0-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="a25a0-105">Kliknij przycisk Start, a następnie wpisz ciąg **cmd** lub **Command**  w polu wyszukiwania, kliknij prawym przyciskiem myszy aplikację wiersza polecenia, a następnie wybierz pozycję  **Uruchom jako administrator** .</span><span class="sxs-lookup"><span data-stu-id="a25a0-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="a25a0-106">Jeśli zostanie wyświetlony monit o podanie hasła administratora lub potwierdzenie, wpisz hasło lub kliknij pozycję **Zezwalaj** .</span><span class="sxs-lookup"><span data-stu-id="a25a0-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="a25a0-107">W oknie wiersza polecenia wpisz **dsregcmd/Leave**  i poczekaj na ukończenie polecenia.</span><span class="sxs-lookup"><span data-stu-id="a25a0-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="a25a0-108">Następnie wpisz **dsregcmd/Join** i poczekaj na ukończenie polecenia.</span><span class="sxs-lookup"><span data-stu-id="a25a0-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="a25a0-109">Uruchom ponownie komputer.</span><span class="sxs-lookup"><span data-stu-id="a25a0-109">Reboot your computer.</span></span>
