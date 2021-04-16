---
title: Rozwiązywanie problemów z funkcją Bluetooth w systemie Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812942"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="ae37f-102">Rozwiązywanie problemów z funkcją Bluetooth w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="ae37f-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="ae37f-103">Jeśli ikony Bluetooth brakuje lub nie można włączyć lub wyłączyć łączności Bluetooth, warto uruchomić narzędzie do rozwiązywania problemów z funkcją Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="ae37f-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="ae37f-104">[Otwórz ustawienia rozwiązywania problemów,](ms-settings:troubleshoot)kliknij pozycję **Bluetooth** w obszarze **Znajdź i rozwiąż** inne problemy , kliknij pozycję Uruchom narzędzie **do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="ae37f-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="ae37f-105">Jeśli nie widzisz ikony Bluetooth, ale bluetooth pojawia się w Menedżerze urządzeń:</span><span class="sxs-lookup"><span data-stu-id="ae37f-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="ae37f-106">W Menedżerze urządzeń kliknij pozycję **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="ae37f-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="ae37f-107">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) nazwę karty Bluetooth i kliknij polecenie **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="ae37f-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="ae37f-108">Zamknij urządzenie z systemem Windows, poczekaj kilka sekund, a następnie włącz je ponownie.</span><span class="sxs-lookup"><span data-stu-id="ae37f-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="ae37f-109">System Windows spróbuje ponownie zainstalować sterownik.</span><span class="sxs-lookup"><span data-stu-id="ae37f-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="ae37f-110">Jeśli ostatnio zainstalowano aktualizacje systemu Windows 10 lub system został uaktualniony do systemu Windows 10, możesz sprawdzić, czy są dostępne aktualizacje sterowników:</span><span class="sxs-lookup"><span data-stu-id="ae37f-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="ae37f-111">W Menedżerze urządzeń kliknij **pozycję Bluetooth,** a następnie kliknij nazwę karty Bluetooth (która może zawierać słowo "radio").</span><span class="sxs-lookup"><span data-stu-id="ae37f-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="ae37f-112">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) kartę Bluetooth, a następnie kliknij pozycję Aktualizuj sterownik Wyszukaj automatycznie   >  **zaktualizowane oprogramowanie sterownika.**</span><span class="sxs-lookup"><span data-stu-id="ae37f-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="ae37f-113">Postępuj zgodnie z instrukcjami, a następnie kliknij **przycisk Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="ae37f-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="ae37f-114">Jeśli system Windows nie może znaleźć nowego sterownika Bluetooth, odwiedź witrynę internetową producenta komputera i pobierz z tej witryny najnowszy sterownik Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="ae37f-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="ae37f-115">Po pobraniu pliku > kliknij pozycję Aktualizuj sterownik Przeglądaj mój komputer w celu pobrania oprogramowania sterownika Przejdź do lokalizacji, w której są przechowywane pliki sterowników, i kliknij przycisk OK Dalej, a następnie postępuj zgodnie z instrukcjami, aby  >    >     >  je zainstalować.</span><span class="sxs-lookup"><span data-stu-id="ae37f-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="ae37f-116">Po zainstalowaniu zaktualizowanego sterownika uruchom ponownie komputer, a następnie sprawdź, czy rozwiązuje to problem z połączeniem.</span><span class="sxs-lookup"><span data-stu-id="ae37f-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="ae37f-117">Aby uzyskać więcej szczegółowych informacji na temat rozwiązywania problemów z funkcją Bluetooth, zobacz pełny artykuł Rozwiązywanie problemów [z funkcją Bluetooth w systemie Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="ae37f-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
