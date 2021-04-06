---
title: Zwalnianie miejsca na dysku w systemie Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505366"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="322ba-102">Zwalnianie miejsca na dysku w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="322ba-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="322ba-103">Oto dwie metody zwalniania miejsca na dysku w systemie Windows:</span><span class="sxs-lookup"><span data-stu-id="322ba-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="322ba-104">Zwalnianie miejsca na dysku w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="322ba-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="322ba-105">Zwolnij miejsce na aktualizacje systemu Windows 10 za pomocą zewnętrznego urządzenia pamięci masowej.</span><span class="sxs-lookup"><span data-stu-id="322ba-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="322ba-106">Jeśli po użyciu narzędzia Oczyszczanie dysku nadal masz mało miejsca na dysku, możliwe, że folder Temp szybko zapełnia się plikami aplikacji (.appx) używanymi przez Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="322ba-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="322ba-107">Aby rozwiązać ten problem, zresetuj sklep Microsoft Store, wyczyść jego pamięć podręczną, a następnie uruchom narzędzie do rozwiązywania problemów usługi Windows Update.</span><span class="sxs-lookup"><span data-stu-id="322ba-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="322ba-108">Przed wykonaniem tych czynności upewnij się, że sklep Microsoft Store jest zamknięty.</span><span class="sxs-lookup"><span data-stu-id="322ba-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="322ba-109">**Krok 1. Resetowanie sklepu Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="322ba-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="322ba-110">**Uwaga** Spowoduje to trwałe usunięcie danych aplikacji z urządzenia, w tym preferencji i danych logowania.</span><span class="sxs-lookup"><span data-stu-id="322ba-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="322ba-111">Wybierz pozycję **Start** > **Ustawienia** > **Aplikacje** > **Aplikacje i funkcje**.</span><span class="sxs-lookup"><span data-stu-id="322ba-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="322ba-112">Na liście aplikacji znajdź i wybierz sklep Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="322ba-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="322ba-113">Wybierz **Opcje zaawansowane**.</span><span class="sxs-lookup"><span data-stu-id="322ba-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="322ba-114">Przewiń w dół i wybierz **Resetowanie**, a następnie **Potwierdź resetowanie**.</span><span class="sxs-lookup"><span data-stu-id="322ba-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="322ba-115">**Krok 2. Wyczyść pamięć podręczną sklepu Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="322ba-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="322ba-116">Naciśnij klawisze logo Windows+R, aby otworzyć okno dialogowe Uruchamianie.</span><span class="sxs-lookup"><span data-stu-id="322ba-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="322ba-117">Wpisz wsreset.exe i wybierz **OK**.</span><span class="sxs-lookup"><span data-stu-id="322ba-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="322ba-118">Otwarte zostanie puste okno wiersza poleceń.</span><span class="sxs-lookup"><span data-stu-id="322ba-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="322ba-119">Po upływie około 10 sekund okno zostanie zamknięte, a sklep zostanie automatycznie otwarty.</span><span class="sxs-lookup"><span data-stu-id="322ba-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="322ba-120">**Krok 3. Resetowanie usługi Windows Update**</span><span class="sxs-lookup"><span data-stu-id="322ba-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="322ba-121">Wybierz **Start** > **Ustawienia** > **Aktualizacja i zabezpieczenia** > **Rozwiązywanie problemów**.</span><span class="sxs-lookup"><span data-stu-id="322ba-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="322ba-122">Przewiń w dół i wybierz **Windows Update** z listy, a następnie wybierz pozycję **Uruchom narzędzie do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="322ba-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="322ba-123">Uruchom ponownie komputer i sprawdź, czy problem nadal występuje.</span><span class="sxs-lookup"><span data-stu-id="322ba-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

