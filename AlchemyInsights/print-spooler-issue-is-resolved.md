---
title: Rozwiązano problem z buforem wydruku
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801851"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="d7c7f-102">Rozwiązano problem z buforem wydruku</span><span class="sxs-lookup"><span data-stu-id="d7c7f-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="d7c7f-103">Jeśli urządzenie zostało zaktualizowane w systemie operacyjnym Windows 10  **OS kompilacja 19041,329**, być może wystąpił problem polegający na tym, że niektóre drukarki nie są drukowane.</span><span class="sxs-lookup"><span data-stu-id="d7c7f-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="d7c7f-104">Bufor wydruku może zgłosić błąd lub nieoczekiwane zamknięcie podczas próby wydrukowania, a żadne dane wyjściowe nie pochodzą z drukarki, której dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="d7c7f-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="d7c7f-105">Ten problem został rozwiązany w systemie operacyjnym [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) **19041,331**.</span><span class="sxs-lookup"><span data-stu-id="d7c7f-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="d7c7f-106">**Prowadzone badanie**</span><span class="sxs-lookup"><span data-stu-id="d7c7f-106">**Ongoing investigation**</span></span>

<span data-ttu-id="d7c7f-107">Plik usługi LSASS**Isass.exe**(Local Security Authority Subsystem Service) może się nie udać na niektóre urządzenia z komunikatem o błędzie "krytyczny proces systemowy, C:\WINDOWS\system32\Isass.exe, którego nie można znaleźć w kodzie statusu c0000008.</span><span class="sxs-lookup"><span data-stu-id="d7c7f-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="d7c7f-108">Komputer musi być teraz ponownie uruchomiony.</span><span class="sxs-lookup"><span data-stu-id="d7c7f-108">The machine must now be restarted".</span></span>  <span data-ttu-id="d7c7f-109">**Firma Microsoft pracuje nad rozróżnieniem i będzie dostarczać aktualizację w nadchodzącej wersji.**</span><span class="sxs-lookup"><span data-stu-id="d7c7f-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="d7c7f-110">Aby uzyskać więcej informacji, zobacz  [znane problemy dotyczące systemu Windows 10 w wersji 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="d7c7f-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>