---
title: W systemie Windows 10 brakuje ikony zasilania lub baterii
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
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790558"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="6d290-102">W systemie Windows 10 brakuje ikony zasilania lub baterii</span><span class="sxs-lookup"><span data-stu-id="6d290-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="6d290-103">Jeśli Twoje urządzenie z systemem Windows 10 ma baterię (np. laptop lub tablet albo komputer podłączony przez USB do zasilacza awaryjnego), zwykle ikona zasilania/baterii jest wyświetlana na pasku zadań obok zegara, na przykład:</span><span class="sxs-lookup"><span data-stu-id="6d290-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona baterii](media/battery-icon.png)

<span data-ttu-id="6d290-105">Jeśli ta ikona nie jest wyświetlana, może być ukryta:</span><span class="sxs-lookup"><span data-stu-id="6d290-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="6d290-106">Przejdź do pozycji **[Ustawienia > Personalizacji > Pasek zadań](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="6d290-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="6d290-107">W obszarze powiadomień kliknij pozycję **Wybierz ikony, które będą wyświetlane na pasku zadań**.</span><span class="sxs-lookup"><span data-stu-id="6d290-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="6d290-108">Następnie znajdź na liście element **Zasilanie** i przełącz jego ustawienie na wartość **Wł.**.</span><span class="sxs-lookup"><span data-stu-id="6d290-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Pokazywanie ikony zasilania na pasku zadań](media/power-icon-on.png)

<span data-ttu-id="6d290-110">**Rozwiązywanie problemów**</span><span class="sxs-lookup"><span data-stu-id="6d290-110">**Troubleshooting**</span></span>

<span data-ttu-id="6d290-111">Jeśli po wykonaniu powyższych instrukcji przełącznik **Zasilanie** jest wyszarzony lub niewidoczny, w polu wyszukiwania na pasku zadań wpisz **menedżer urządzeń**, a następnie na liście wyników wybierz pozycję **Menedżer urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="6d290-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="6d290-112">W obszarze **Baterie** kliknij prawym przyciskiem myszy baterię urządzenia, kliknij pozycję **Wyłącz**, a następnie kliknij pozycję **Tak**.</span><span class="sxs-lookup"><span data-stu-id="6d290-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="6d290-113">Poczekaj kilka sekund, a następnie kliknij prawym przyciskiem myszy baterię i kliknij pozycję **Włącz**.</span><span class="sxs-lookup"><span data-stu-id="6d290-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="6d290-114">Następnie ponownie uruchom urządzenie.</span><span class="sxs-lookup"><span data-stu-id="6d290-114">Then restart your device.</span></span>

<span data-ttu-id="6d290-115">Jeśli po wykonaniu powyższych instrukcji ikona baterii nie jest wyświetlana na pasku zadań, w polu wyszukiwania na pasku zadań wpisz **menedżer zadań**, a następnie na liście wyników kliknij pozycję **Menedżer zadań**.</span><span class="sxs-lookup"><span data-stu-id="6d290-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="6d290-116">Na karcie **Procesy** w obszarze **Nazwa** kliknij prawym przyciskiem myszy pozycję **Eksplorator**, a następnie kliknij pozycję **Uruchom ponownie**.</span><span class="sxs-lookup"><span data-stu-id="6d290-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
