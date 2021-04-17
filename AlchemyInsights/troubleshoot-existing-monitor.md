---
title: Rozwiązywanie problemów z istniejącym monitorem
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824589"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="bf029-102">Rozwiązywanie problemów z istniejącym monitorem</span><span class="sxs-lookup"><span data-stu-id="bf029-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="bf029-103">Wypróbuj poniższe rozwiązania, aby rozwiązać problemy z monitorem.</span><span class="sxs-lookup"><span data-stu-id="bf029-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="bf029-104">**Odświeżanie ekranu monitora:**</span><span class="sxs-lookup"><span data-stu-id="bf029-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="bf029-105">Naciśnij jednocześnie następujące klawisze: klawisz systemu Windows + Ctrl + Shift + B. Spowoduje to odświeżenie komunikacji ze sterownikem graficznym.</span><span class="sxs-lookup"><span data-stu-id="bf029-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="bf029-106">Monitory będą migać chwilę i odwrócić po upływie kilku sekund.</span><span class="sxs-lookup"><span data-stu-id="bf029-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="bf029-107">**Rozwiązywanie problemów ze sprzętem monitorów:**</span><span class="sxs-lookup"><span data-stu-id="bf029-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="bf029-108">Odłącz kabel od podłączania komputera do monitora i podłącz go z powrotem.</span><span class="sxs-lookup"><span data-stu-id="bf029-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="bf029-109">Odłącz od komputera wszystkie nieistnikowe urządzenia (takie jak adaptery lub stacje dokujące).</span><span class="sxs-lookup"><span data-stu-id="bf029-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="bf029-110">**Jeśli niedawno na komputerze została zainstalowana aktualizacja, możesz wycofać sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="bf029-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="bf029-111">Wybierz **pozycję Start**, wpisz menedżer **urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach.</span><span class="sxs-lookup"><span data-stu-id="bf029-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bf029-112">Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Właściwości.**</span><span class="sxs-lookup"><span data-stu-id="bf029-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="bf029-113">Przejdź do karty **Sterownik i** wybierz pozycję **Przywróć sterownik.**</span><span class="sxs-lookup"><span data-stu-id="bf029-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="bf029-114">Uwaga: Jeśli ta opcja jest niedostępne lub jest wyszarzona, wybierz pozycję **Nie** z poniższych opcji, aby przejść do następnego kroku.</span><span class="sxs-lookup"><span data-stu-id="bf029-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="bf029-115">Zanim te zmiany zajdą w życie, może być konieczne ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="bf029-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="bf029-116">**Odinstaluj i ponownie zainstaluj sterownik ekranu:**</span><span class="sxs-lookup"><span data-stu-id="bf029-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="bf029-117">Wybierz **pozycję Start**, wpisz menedżer **urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** w wynikach.</span><span class="sxs-lookup"><span data-stu-id="bf029-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="bf029-118">Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Odinstaluj urządzenie**.</span><span class="sxs-lookup"><span data-stu-id="bf029-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="bf029-119">Zaznacz pole wyboru Usuń oprogramowanie sterownika **dla tego urządzenia** i wybierz pozycję Odinstaluj . </span><span class="sxs-lookup"><span data-stu-id="bf029-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="bf029-120">Uwaga: na tym etapie może pojawić się monit o ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="bf029-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="bf029-121">Przed ponownym uruchomieniem zapisz pozostałe instrukcje.</span><span class="sxs-lookup"><span data-stu-id="bf029-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="bf029-122">Otwórz ponownie Menedżera urządzeń.</span><span class="sxs-lookup"><span data-stu-id="bf029-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="bf029-123">Rozwiń **sekcję Karty graficzne,** kliknij prawym przyciskiem myszy kartę graficzną i wybierz pozycję **Aktualizuj sterownik**.</span><span class="sxs-lookup"><span data-stu-id="bf029-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="bf029-124">Wybierz **pozycję Wyszukaj automatycznie, aby zaktualizować oprogramowanie sterownika** i postępuj zgodnie z instrukcjami instalacji.</span><span class="sxs-lookup"><span data-stu-id="bf029-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>