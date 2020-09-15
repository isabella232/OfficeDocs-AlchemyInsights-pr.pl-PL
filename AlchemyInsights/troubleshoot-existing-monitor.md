---
title: Rozwiązywanie problemów z istniejącym monitorem
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690721"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="36cf9-102">Rozwiązywanie problemów z istniejącym monitorem</span><span class="sxs-lookup"><span data-stu-id="36cf9-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="36cf9-103">Wypróbuj te rozwiązania, aby rozwiązać problem z monitorem.</span><span class="sxs-lookup"><span data-stu-id="36cf9-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="36cf9-104">**Odśwież ekran monitora:**</span><span class="sxs-lookup"><span data-stu-id="36cf9-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="36cf9-105">Naciśnij następujące klawisze w tym samym czasie: klawisz Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji za pomocą sterownika graficznego.</span><span class="sxs-lookup"><span data-stu-id="36cf9-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="36cf9-106">Twoje monitory będą migać, a po kilku sekundach rozpocznie się odtwarzanie.</span><span class="sxs-lookup"><span data-stu-id="36cf9-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="36cf9-107">**Rozwiązywanie problemów ze sprzętem monitora:**</span><span class="sxs-lookup"><span data-stu-id="36cf9-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="36cf9-108">Odłącz kabel łączący komputer z monitorem i podłącz go ponownie.</span><span class="sxs-lookup"><span data-stu-id="36cf9-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="36cf9-109">Odłączanie wszelkich nieistotnych urządzeń z komputera (takich jak karty lub stacje dokujące).</span><span class="sxs-lookup"><span data-stu-id="36cf9-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="36cf9-110">**Jeśli niedawno zainstalowano aktualizację na komputerze PC, możesz wycofać sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="36cf9-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="36cf9-111">Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z wyników.</span><span class="sxs-lookup"><span data-stu-id="36cf9-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="36cf9-112">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, ands wybierz pozycję **Właściwości**.</span><span class="sxs-lookup"><span data-stu-id="36cf9-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="36cf9-113">Przejdź do karty **Sterownik** i wybierz pozycję **Przywróć sterownik**.</span><span class="sxs-lookup"><span data-stu-id="36cf9-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="36cf9-114">Uwaga: Jeśli ta funkcja jest niedostępna lub jest wyszarzona, wybierz pozycję **nie** z poniższych opcji, aby przejść do następnego kroku.</span><span class="sxs-lookup"><span data-stu-id="36cf9-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="36cf9-115">Aby zmiany zostały wprowadzone, może być konieczne ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="36cf9-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="36cf9-116">**Odinstaluj i ponownie zainstaluj sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="36cf9-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="36cf9-117">Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z wyników.</span><span class="sxs-lookup"><span data-stu-id="36cf9-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="36cf9-118">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, ands wybierz pozycję **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="36cf9-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="36cf9-119">Zaznacz pole wyboru obok pozycji **Usuń oprogramowanie sterownika dla tego urządzenia** i wybierz pozycję **Odinstaluj**.</span><span class="sxs-lookup"><span data-stu-id="36cf9-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="36cf9-120">Uwaga: może zostać wyświetlony monit o ponowne uruchomienie komputera na tym etapie.</span><span class="sxs-lookup"><span data-stu-id="36cf9-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="36cf9-121">Przed ponownym uruchomieniem upewnij się, że Zanotuj pozostałe instrukcje.</span><span class="sxs-lookup"><span data-stu-id="36cf9-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="36cf9-122">Ponownie otwórz Menedżera urządzeń.</span><span class="sxs-lookup"><span data-stu-id="36cf9-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="36cf9-123">Rozwiń sekcję **karty graficzne** , kliknij prawym przyciskiem myszy kartę graficzną, a następnie wybierz polecenie **Aktualizuj sterownik**.</span><span class="sxs-lookup"><span data-stu-id="36cf9-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="36cf9-124">Wybierz pozycję **Wyszukaj automatycznie w celu zaktualizowania oprogramowania sterownika** i postępuj zgodnie z instrukcjami instalacji.</span><span class="sxs-lookup"><span data-stu-id="36cf9-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>