---
title: Problem z buforem wydruku został rozwiązany
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088403"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="b0c4b-102">Problem z buforem wydruku został rozwiązany</span><span class="sxs-lookup"><span data-stu-id="b0c4b-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="b0c4b-103">Jeśli urządzenie zostało zaktualizowane o kompilację systemu operacyjnego Systemu Windows 10 **19041.329,** być może zauważyłeś problem, w którym niektóre drukarki nie mogą drukować.</span><span class="sxs-lookup"><span data-stu-id="b0c4b-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="b0c4b-104">Bufor wydruku może zgłosić błąd lub zamknąć nieoczekiwanie podczas próby drukowania, a żadne dane wyjściowe nie pochodzą z drukarki, którego dotyczy problem.</span><span class="sxs-lookup"><span data-stu-id="b0c4b-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="b0c4b-105">Ten problem został rozwiązany w kompilacji systemu operacyjnego **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="b0c4b-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="b0c4b-106">**Trwające dochodzenie**</span><span class="sxs-lookup"><span data-stu-id="b0c4b-106">**Ongoing investigation**</span></span>

<span data-ttu-id="b0c4b-107">Plik LSASS (Local Security Authority Subsystem Service)\*\* (Isass.exe) \*\*może zakończyć się niepowodzeniem na niektórych urządzeniach z komunikatem o błędzie "Krytyczny proces systemowy, C:\WINDOWS\system32\Isass.exe, nie powiódł się z kodem stanu c0000008.</span><span class="sxs-lookup"><span data-stu-id="b0c4b-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="b0c4b-108">Urządzenie musi zostać ponownie uruchomione".</span><span class="sxs-lookup"><span data-stu-id="b0c4b-108">The machine must now be restarted".</span></span>  <span data-ttu-id="b0c4b-109">**Firma Microsoft pracuje nad rozdzielczością i udostępni aktualizację w nadchodzącej wersji.**</span><span class="sxs-lookup"><span data-stu-id="b0c4b-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="b0c4b-110">Aby uzyskać więcej informacji, sprawdź [windows 10 wersja 2004 znane problemy](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="b0c4b-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>