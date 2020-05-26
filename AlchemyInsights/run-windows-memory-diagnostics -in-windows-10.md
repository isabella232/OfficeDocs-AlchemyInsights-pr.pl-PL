---
title: Uruchamianie diagnostyki pamięci systemu Windows w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357786"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="1421e-102">Uruchamianie diagnostyki pamięci systemu Windows w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="1421e-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="1421e-103">Jeśli system Windows i aplikacje na komputerze ulegają awarii, zamrożeniu lub działają w niestabilny sposób, może to spowodować problem z pamięcią (RAM) komputera.</span><span class="sxs-lookup"><span data-stu-id="1421e-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="1421e-104">Można uruchomić diagnostykę pamięci systemu Windows, aby sprawdzić, czy nie występują problemy z pamięcią RAM komputera.</span><span class="sxs-lookup"><span data-stu-id="1421e-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="1421e-105">W polu wyszukiwania na pasku zadań wpisz polecenie **Diagnostyka pamięci,** a następnie wybierz pozycję **Diagnostyka pamięci systemu Windows**.</span><span class="sxs-lookup"><span data-stu-id="1421e-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="1421e-106">Aby uruchomić diagnostykę, komputer musi zostać ponownie uruchomiony.</span><span class="sxs-lookup"><span data-stu-id="1421e-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="1421e-107">Możesz natychmiast ponownie uruchomić ponownie (zapisz najpierw swoje prace i zamknij otwarte dokumenty i wiadomości e-mail) lub zaplanuj automatyczne uruchomienie diagnostyki przy następnym ponownym uruchomieniu komputera:</span><span class="sxs-lookup"><span data-stu-id="1421e-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostyka pamięci systemu Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="1421e-109">Po ponownym uruchomieniu komputera **narzędzie diagnostyki pamięci systemu Windows** zostanie uruchomione automatycznie.</span><span class="sxs-lookup"><span data-stu-id="1421e-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="1421e-110">Stan i postęp będą wyświetlane jako uruchomienie diagnostyki i masz możliwość anulowania diagnostyki, naciskając klawisz **ESC** na klawiaturze.</span><span class="sxs-lookup"><span data-stu-id="1421e-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="1421e-111">Po zakończeniu diagnostyki system Windows zostanie uruchomiony normalnie.</span><span class="sxs-lookup"><span data-stu-id="1421e-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="1421e-112">Natychmiast po ponownym uruchomieniu komputera zostanie wyświetlone powiadomienie (obok **ikony Centrum akcji** na pasku zadań), aby wskazać, czy zostały znalezione błędy pamięci.</span><span class="sxs-lookup"><span data-stu-id="1421e-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="1421e-113">Przykład:</span><span class="sxs-lookup"><span data-stu-id="1421e-113">For example:</span></span>

<span data-ttu-id="1421e-114">Oto ikona Centrum akcji:</span><span class="sxs-lookup"><span data-stu-id="1421e-114">Here's the Action Center icon:</span></span> ![Ikona Centrum akcji](media/action-center-icon.png) 

<span data-ttu-id="1421e-116">I przykładowe powiadomienie:</span><span class="sxs-lookup"><span data-stu-id="1421e-116">And a sample notification:</span></span> ![Brak błędów pamięci](media/no-memory-errors.png)

<span data-ttu-id="1421e-118">Jeśli powiadomienie nie zostanie odebrane, możesz wybrać ikonę **Centrum akcji** na pasku zadań, aby wyświetlić **Centrum akcji** i wyświetlić przewijaną listę powiadomień.</span><span class="sxs-lookup"><span data-stu-id="1421e-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="1421e-119">Aby przejrzeć szczegółowe informacje, wpisz **zdarzenie** w polu wyszukiwania na pasku zadań, a następnie wybierz pozycję **Podgląd zdarzeń**.</span><span class="sxs-lookup"><span data-stu-id="1421e-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="1421e-120">W okienku po lewej **stronie Podglądu zdarzeń**przejdź do pozycji **Dzienniki systemu Windows > System**.</span><span class="sxs-lookup"><span data-stu-id="1421e-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="1421e-121">W okienku po prawej stronie skanuj listę, patrząc na kolumnę **Źródło,** aż zobaczysz zdarzenia o wartości źródłowej **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="1421e-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="1421e-122">Wyróżnij każde takie zdarzenie i zobacz informacje o wyniku w polu pod kartą **Ogólne** poniżej listy.</span><span class="sxs-lookup"><span data-stu-id="1421e-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
