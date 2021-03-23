---
title: Wolne miejsce na dysku w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037955"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="e9748-102">Wolne miejsce na dysku w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="e9748-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="e9748-103">Oto dwie opcje, które można zrobić, aby uwolnić miejsce na dysku w systemie Windows:</span><span class="sxs-lookup"><span data-stu-id="e9748-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="e9748-104">Uwolnij miejsce na dysku w systemie Windows 10.</span><span class="sxs-lookup"><span data-stu-id="e9748-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="e9748-105">Uwolnij miejsce na aktualizacje systemu Windows 10 za pomocą zewnętrznego urządzenia magazynującego.</span><span class="sxs-lookup"><span data-stu-id="e9748-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="e9748-106">Jeśli po użyciu funkcji Oczyszczanie dysku nadal masz mało miejsca na dysku, możliwe, że folder Temp szybko wypełnia pliki aplikacji (appx) używane w Sklepie Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e9748-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="e9748-107">Aby rozwiązać ten problem, zresetuj Sklep, wyczyść pamięć podręczną Sklepu, a następnie uruchom narzędzie do rozwiązywania problemów z usługą Windows Update.</span><span class="sxs-lookup"><span data-stu-id="e9748-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="e9748-108">Przed kontynuowaniem tej procedury upewnij się, że Sklep Microsoft jest zamknięty.</span><span class="sxs-lookup"><span data-stu-id="e9748-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="e9748-109">**Krok 1. Resetowanie Sklepu Microsoft**</span><span class="sxs-lookup"><span data-stu-id="e9748-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="e9748-110">**Uwaga** Spowoduje to trwałe usunięcie danych aplikacji na urządzeniu, w tym Twoich preferencji i szczegółów logowania.</span><span class="sxs-lookup"><span data-stu-id="e9748-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="e9748-111">Wybierz **pozycję Start**  >  **Ustawienia**  >  **Aplikacje**&  >  **funkcje**.</span><span class="sxs-lookup"><span data-stu-id="e9748-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="e9748-112">Na liście aplikacji znajdź i wybierz pozycję Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="e9748-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="e9748-113">Wybierz **pozycję Opcje zaawansowane.**</span><span class="sxs-lookup"><span data-stu-id="e9748-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="e9748-114">Przewiń w dół i **wybierz pozycję Resetuj**, a następnie **Potwierdź resetowanie**.</span><span class="sxs-lookup"><span data-stu-id="e9748-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="e9748-115">**Krok 2. Wyczyszczenie pamięci podręcznej Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="e9748-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="e9748-116">Naciśnij klawisze logo Windows + R, aby otworzyć okno dialogowe Uruchamianie.</span><span class="sxs-lookup"><span data-stu-id="e9748-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="e9748-117">Wpisz wsreset.exe i wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="e9748-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="e9748-118">Zostanie otwarte puste okno wiersza polecenia.</span><span class="sxs-lookup"><span data-stu-id="e9748-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="e9748-119">Po upływie około 10 sekund okno zostaje zamknięte, a Sklep jest otwierany automatycznie.</span><span class="sxs-lookup"><span data-stu-id="e9748-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="e9748-120">**Krok 3. Resetowanie usługi Windows Update**</span><span class="sxs-lookup"><span data-stu-id="e9748-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="e9748-121">Wybierz **pozycję Uruchom**  >    >  **aktualizację ustawień i & rozwiązywanie problemów z**  >  **zabezpieczeniami.**</span><span class="sxs-lookup"><span data-stu-id="e9748-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="e9748-122">Przewiń w dół i wybierz z listy usługę **Windows Update,** a następnie **wybierz pozycję Uruchom narzędzie do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="e9748-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="e9748-123">Uruchom ponownie komputer i sprawdź, czy problem nadal występuje.</span><span class="sxs-lookup"><span data-stu-id="e9748-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

