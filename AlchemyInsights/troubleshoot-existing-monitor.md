---
title: Rozwiązywanie problemów z istniejącym monitorem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738578"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="1260e-102">Rozwiązywanie problemów z istniejącym monitorem</span><span class="sxs-lookup"><span data-stu-id="1260e-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="1260e-103">Wypróbuj te rozwiązania, aby rozwiązać problem z monitorem.</span><span class="sxs-lookup"><span data-stu-id="1260e-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="1260e-104">**Odśwież ekran monitora:**</span><span class="sxs-lookup"><span data-stu-id="1260e-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="1260e-105">Naciśnij jednocześnie następujące przyciski: klucz systemu Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji ze sterownikiem graficznym.</span><span class="sxs-lookup"><span data-stu-id="1260e-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="1260e-106">Monitory będą migać chwilowo i wrócić po kilku sekundach.</span><span class="sxs-lookup"><span data-stu-id="1260e-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="1260e-107">**Rozwiązywanie problemów ze sprzętem monitora:**</span><span class="sxs-lookup"><span data-stu-id="1260e-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="1260e-108">Odłącz przewód łączący komputer z monitorem i podłącz go ponownie.</span><span class="sxs-lookup"><span data-stu-id="1260e-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="1260e-109">Odłącz wszystkie urządzenia inne niż istotne z komputera (takie jak karty lub stacje dokujące).</span><span class="sxs-lookup"><span data-stu-id="1260e-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="1260e-110">**Jeśli niedawno zainstalowano aktualizację na komputerze, można wycofać sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="1260e-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="1260e-111">Wybierz **Start**, wpisz **Menedżer urządzeń**i wybierz **Menedżer urządzeń** z wyników.</span><span class="sxs-lookup"><span data-stu-id="1260e-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1260e-112">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną, a następnie wybierz polecenie **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="1260e-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="1260e-113">Przejdź do zakładki **Sterownik** i wybierz **Przywróć sterownik**.</span><span class="sxs-lookup"><span data-stu-id="1260e-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="1260e-114">Uwaga: Jeśli ta opcja nie jest dostępna lub jest wyszarzona, wybierz opcję **nie** z poniższych opcji, aby przejść do kolejnego kroku.</span><span class="sxs-lookup"><span data-stu-id="1260e-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="1260e-115">Zanim zmiany zostaną uwzględnione, może być konieczne ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="1260e-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="1260e-116">**Odinstaluj i ponownie zainstaluj sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="1260e-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="1260e-117">Wybierz **Start**, wpisz **Menedżer urządzeń**i wybierz **Menedżer urządzeń** z wyników.</span><span class="sxs-lookup"><span data-stu-id="1260e-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1260e-118">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną, a następnie wybierz pozycję **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="1260e-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="1260e-119">Zaznacz pole wyboru obok opcji **Usuń oprogramowanie sterownika dla tego urządzenia** i wybierz opcję **Odinstaluj**.</span><span class="sxs-lookup"><span data-stu-id="1260e-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="1260e-120">Uwaga: na tym etapie może zostać wyświetlony monit o ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="1260e-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="1260e-121">Pamiętaj, aby zapisać pozostałe instrukcje przed ponownym uruchomieniem.</span><span class="sxs-lookup"><span data-stu-id="1260e-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="1260e-122">Ponownie otwórz Menedżera urządzeń.</span><span class="sxs-lookup"><span data-stu-id="1260e-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="1260e-123">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę wyświetlaną i wybierz polecenie **Aktualizuj sterownik**.</span><span class="sxs-lookup"><span data-stu-id="1260e-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="1260e-124">Wybierz opcję **Wyszukaj automatycznie, aby zaktualizować oprogramowanie sterownika** i postępuj zgodnie z instrukcjami instalacji.</span><span class="sxs-lookup"><span data-stu-id="1260e-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>