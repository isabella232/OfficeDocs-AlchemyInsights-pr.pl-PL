---
title: Rozwiązywanie problemów z bluetooth w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268703"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="9ed0b-102">Rozwiązywanie problemów z bluetooth w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="9ed0b-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="9ed0b-103">Jeśli brakuje ikony Bluetooth lub nie można włączyć lub wyłączyć funkcji Bluetooth, możesz uruchomić narzędzie do rozwiązywania problemów z bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="9ed0b-104">[Otwórz ustawienia rozwiązywania problemów](ms-settings:troubleshoot), kliknij **pozycję Bluetooth** w obszarze Znajdź **i rozwiąż inne problemy**, kliknij pozycję Uruchom narzędzie do rozwiązywania **problemów**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="9ed0b-105">Jeśli nie widzisz ikony Bluetooth, ale funkcja Bluetooth jest wyświetlana w Menedżerze urządzeń:</span><span class="sxs-lookup"><span data-stu-id="9ed0b-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="9ed0b-106">W Menedżerze urządzeń kliknij pozycję **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="9ed0b-107">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) nazwę karty Bluetooth i kliknij polecenie **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="9ed0b-108">Zamknij urządzenie z systemem Windows, odczekaj kilka sekund, a następnie włącz je z powrotem.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="9ed0b-109">System Windows spróbuje ponownie zainstalować sterownik.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="9ed0b-110">Jeśli niedawno zainstalowano aktualizacje systemu Windows 10 lub uaktualniono system Windows 10, możesz sprawdzić dostępność aktualizacji sterowników:</span><span class="sxs-lookup"><span data-stu-id="9ed0b-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="9ed0b-111">W Menedżerze urządzeń kliknij pozycję **Bluetooth**, a następnie kliknij nazwę karty Bluetooth (która może zawierać słowo "radio").</span><span class="sxs-lookup"><span data-stu-id="9ed0b-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="9ed0b-112">Naciśnij i przytrzymaj (lub kliknij prawym przyciskiem myszy) kartę Bluetooth, a następnie automatycznie kliknij przycisk **Aktualizuj sterownik** > **Wyszukaj zaktualizowane oprogramowanie sterownika**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="9ed0b-113">Wykonaj kroki, a następnie kliknij przycisk **Zamknij**.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="9ed0b-114">Jeśli system Windows nie może znaleźć nowego sterownika Bluetooth, odwiedź witrynę producenta komputera i pobierz stamtąd najnowszy sterownik Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="9ed0b-115">Po pobraniu kliknij przycisk **Aktualizuj sterownik** > **Przeglądaj mój komputer w poszukiwaniu oprogramowania** > sterownika**Przeglądaj** lokalizację, w której pliki sterowników są przechowywane > **OK** > **Next**, i postępuj zgodnie z instrukcjami, aby zainstalować.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="9ed0b-116">Po zainstalowaniu zaktualizowanego sterownika uruchom ponownie komputer, a następnie sprawdź, czy rozwiązuje on problem z połączeniem.</span><span class="sxs-lookup"><span data-stu-id="9ed0b-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="9ed0b-117">Aby uzyskać więcej informacji na temat rozwiązywania problemów z Bluetooth, zobacz cały artykuł, [Rozwiązywanie problemów Bluetooth w systemie Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="9ed0b-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
