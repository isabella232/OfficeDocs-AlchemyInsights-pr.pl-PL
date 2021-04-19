---
title: Uruchamianie Diagnostyki pamięci systemu Windows w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826677"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="296d6-102">Uruchamianie Diagnostyki pamięci systemu Windows w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="296d6-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="296d6-103">Jeśli system Windows i aplikacje na komputerze ulega awarii, zawieszają się lub działają niestabilnie, może wystąpić problem z pamięcią RAM komputera.</span><span class="sxs-lookup"><span data-stu-id="296d6-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="296d6-104">Możesz uruchomić Narzędzie Diagnostyka pamięci systemu Windows, aby sprawdzić, czy nie występują problemy z pamięcią RAM komputera.</span><span class="sxs-lookup"><span data-stu-id="296d6-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="296d6-105">W polu wyszukiwania na pasku zadań wpisz diagnostykę pamięci **,** a następnie wybierz pozycję **Diagnostyka pamięci systemu Windows**.</span><span class="sxs-lookup"><span data-stu-id="296d6-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="296d6-106">Aby uruchomić diagnostykę, komputer musi zostać uruchomiony ponownie.</span><span class="sxs-lookup"><span data-stu-id="296d6-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="296d6-107">Masz możliwość natychmiastowego ponownego uruchomienia (zapisz najpierw swoją pracę i zamknij otwarte dokumenty i wiadomości e-mail) lub zaplanuj automatyczne uruchamianie diagnostyczne przy następnym ponownym uruchomieniu komputera:</span><span class="sxs-lookup"><span data-stu-id="296d6-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostyka pamięci systemu Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="296d6-109">Po ponownym uruchomieniu komputera narzędzie **Diagnostyka pamięci** systemu Windows zostanie uruchomione automatycznie.</span><span class="sxs-lookup"><span data-stu-id="296d6-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="296d6-110">Stan i postęp będą wyświetlane jako diagnostyka, a Ty możesz anulować diagnostykę, naciskając klawisz **ESC** na klawiaturze.</span><span class="sxs-lookup"><span data-stu-id="296d6-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="296d6-111">Po zakończeniu diagnostyki system Windows zacznie normalnie.</span><span class="sxs-lookup"><span data-stu-id="296d6-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="296d6-112">Natychmiast po ponownym uruchomieniu, gdy zostanie wyświetlony pulpit, zostanie wyświetlone powiadomienie (obok ikony Centrum akcji na pasku zadań) wskazujące, czy zostały znalezione błędy pamięci. </span><span class="sxs-lookup"><span data-stu-id="296d6-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="296d6-113">Przykład:</span><span class="sxs-lookup"><span data-stu-id="296d6-113">For example:</span></span>

<span data-ttu-id="296d6-114">Oto ikona Centrum akcji:</span><span class="sxs-lookup"><span data-stu-id="296d6-114">Here's the Action Center icon:</span></span> ![Ikona Centrum akcji](media/action-center-icon.png) 

<span data-ttu-id="296d6-116">Oraz przykładowe powiadomienie:</span><span class="sxs-lookup"><span data-stu-id="296d6-116">And a sample notification:</span></span> ![Brak błędów pamięci](media/no-memory-errors.png)

<span data-ttu-id="296d6-118">Jeśli przegapisz powiadomienie, możesz  wybrać ikonę Centrum akcji na  pasku zadań, aby wyświetlić Centrum akcji i wyświetlać przewijaną listę powiadomień.</span><span class="sxs-lookup"><span data-stu-id="296d6-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="296d6-119">Aby przejrzeć szczegółowe informacje, wpisz **zdarzenie** w polu wyszukiwania na pasku zadań, a następnie wybierz pozycję **Podgląd zdarzeń**.</span><span class="sxs-lookup"><span data-stu-id="296d6-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="296d6-120">W **okienku podglądu** zdarzeń po lewej stronie przejdź do okna Dzienniki **systemu Windows > systemu**.</span><span class="sxs-lookup"><span data-stu-id="296d6-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="296d6-121">W okienku po prawej stronie zeskanuj  listę w dół, patrząc na kolumnę Źródło, aż zobaczysz zdarzenia z wartością źródłową **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="296d6-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="296d6-122">Wyróżnij każde takie zdarzenie i wyświetl informacje o wynikach w polu pod **kartą** Ogólne poniżej listy.</span><span class="sxs-lookup"><span data-stu-id="296d6-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
