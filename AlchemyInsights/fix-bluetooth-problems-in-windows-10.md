---
title: Rozwiązywanie problemów z Bluetooth w systemie Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730169"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="676b3-102">Rozwiązywanie problemów z Bluetooth w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="676b3-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="676b3-103">Jeśli brakuje ikony Bluetooth lub nie można włączyć lub wyłączyć protokołu Bluetooth, może być konieczne uruchomienie narzędzia do rozwiązywania problemów z funkcją Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="676b3-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="676b3-104">[Otwórz ustawienia rozwiązywania problemów](ms-settings:troubleshoot), kliknij pozycję **Bluetooth** w obszarze **Znajdź i Rozwiąż inne problemy**, kliknij pozycję **Uruchom narzędzie do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="676b3-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="676b3-105">Jeśli nie widzisz ikony Bluetooth, ale protokół Bluetooth jest wyświetlany w Menedżerze urządzeń:</span><span class="sxs-lookup"><span data-stu-id="676b3-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="676b3-106">W Menedżerze urządzeń kliknij pozycję **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="676b3-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="676b3-107">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) nazwę karty Bluetooth i kliknij pozycję **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="676b3-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="676b3-108">Zamknij urządzenie z systemem Windows, poczekaj kilka sekund, a następnie włącz je ponownie.</span><span class="sxs-lookup"><span data-stu-id="676b3-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="676b3-109">System Windows podejmie próbę ponownego zainstalowania sterownika.</span><span class="sxs-lookup"><span data-stu-id="676b3-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="676b3-110">Jeśli ostatnio zainstalowano aktualizacje systemu Windows 10 lub uaktualniono do systemu Windows 10, warto sprawdzić dostępność aktualizacji sterowników:</span><span class="sxs-lookup"><span data-stu-id="676b3-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="676b3-111">W Menedżerze urządzeń kliknij pozycję **Bluetooth**, a następnie kliknij nazwę karty Bluetooth (która może zawierać wyraz "Radio").</span><span class="sxs-lookup"><span data-stu-id="676b3-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="676b3-112">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) kartę Bluetooth, a następnie kliknij pozycję **Aktualizuj**  >  **Wyszukiwanie sterowników automatycznie, aby uzyskać zaktualizowane oprogramowanie sterownika**.</span><span class="sxs-lookup"><span data-stu-id="676b3-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="676b3-113">Postępuj zgodnie z instrukcjami, a następnie kliknij przycisk **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="676b3-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="676b3-114">Jeśli system Windows nie może znaleźć nowego sterownika Bluetooth, odwiedź witrynę internetową producenta komputera i Pobierz z niego najnowszą wersję sterownika Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="676b3-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="676b3-115">Po pobraniu pliku kliknij pozycję **Aktualizuj sterownik**  >  **Przeglądaj mój komputer w poszukiwaniu oprogramowania sterownika**  >  **Wyszukaj** lokalizację, w której są przechowywane pliki sterowników, > **OK**  >  **Next**, a następnie postępuj zgodnie z instrukcjami instalacji.</span><span class="sxs-lookup"><span data-stu-id="676b3-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="676b3-116">Po zainstalowaniu zaktualizowanego sterownika Uruchom ponownie komputer, a następnie sprawdź, czy rozwiązanie problemu z połączeniem jest rozwiązywane.</span><span class="sxs-lookup"><span data-stu-id="676b3-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="676b3-117">Aby uzyskać więcej informacji na temat rozwiązywania problemów z funkcją Bluetooth, zobacz pełny artykuł [Rozwiązywanie problemów z Bluetooth w systemie Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="676b3-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
