---
title: Rozwiązywanie problemów z dźwiękiem w systemie Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833301"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="41b3d-102">Rozwiązywanie problemów z dźwiękiem w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="41b3d-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="41b3d-103">**Uruchamianie narzędzia do rozwiązywania problemów z dźwiękiem**</span><span class="sxs-lookup"><span data-stu-id="41b3d-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="41b3d-104">Otwórz ustawienia [rozwiązywania problemów.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="41b3d-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="41b3d-105">Wybierz **pozycję Odtwarzanie dźwięku** Uruchom narzędzie do  >  **rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="41b3d-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="41b3d-106">**Ustawianie urządzenia domyślnego**</span><span class="sxs-lookup"><span data-stu-id="41b3d-106">**Set the default device**</span></span>

<span data-ttu-id="41b3d-107">Jeśli łączysz się z urządzeniem audio za pomocą portu USB lub HDMI, może być konieczne ustawienie tego urządzenia jako domyślnego:</span><span class="sxs-lookup"><span data-stu-id="41b3d-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="41b3d-108">Otwórz **menu Start** Dźwięk , a następnie wybierz z listy wyników pozycję Dźwięk lub Zmień dźwięki  >  systemowe.  </span><span class="sxs-lookup"><span data-stu-id="41b3d-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="41b3d-109">Na karcie **Odtwarzanie** wybierz urządzenie, wybierz pozycję Ustaw **domyślne**, a następnie wybierz przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="41b3d-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="41b3d-110">**Sprawdzanie kabli, głośności, głośników i słuchawek**</span><span class="sxs-lookup"><span data-stu-id="41b3d-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="41b3d-111">Sprawdź połączenia głośników i słuchawek podejściem luźnych kabli i upewnij się, że są podłączone do właściwego gniazda.</span><span class="sxs-lookup"><span data-stu-id="41b3d-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="41b3d-112">Sprawdź poziomy zasilania i głośności, a następnie obróć wszystkie kontrolki głośności do góry.</span><span class="sxs-lookup"><span data-stu-id="41b3d-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="41b3d-113">Niektóre głośniki i aplikacje mają własne kontrolki głośności. być może trzeba będzie je wszystkie sprawdzić, aby upewnić się, że są one na właściwych poziomach.</span><span class="sxs-lookup"><span data-stu-id="41b3d-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="41b3d-114">Spróbuj nałączyć połączenie przy użyciu innego portu USB.</span><span class="sxs-lookup"><span data-stu-id="41b3d-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="41b3d-115">**Uwaga:** Pamiętaj, że głośniki mogą nie działać po podłączeniu słuchawek.</span><span class="sxs-lookup"><span data-stu-id="41b3d-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="41b3d-116">**Sprawdzanie Menedżera urządzeń**</span><span class="sxs-lookup"><span data-stu-id="41b3d-116">**Check Device Manager**</span></span>

<span data-ttu-id="41b3d-117">Aby upewnić się, że sterowniki są aktualne:</span><span class="sxs-lookup"><span data-stu-id="41b3d-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="41b3d-118">Wybierz **przycisk Start,** wpisz **Menedżer urządzeń**, a następnie wybierz pozycję Menedżer **urządzeń** z listy wyników.</span><span class="sxs-lookup"><span data-stu-id="41b3d-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="41b3d-119">W **obszarze Kontrolery dźwięku, wideo** i gier wybierz kartę dźwiękową, otwórz ją, wybierz **kartę Sterownik** i wybierz pozycję Aktualizuj **sterownik.**</span><span class="sxs-lookup"><span data-stu-id="41b3d-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="41b3d-120">**Uwaga:** Jeśli system Windows nie znajduje nowego sterownika, poszukaj go w witrynie internetowej producenta urządzenia i postępuj zgodnie z podanymi instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="41b3d-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="41b3d-121">**Ponowne instalowanie sterownika**</span><span class="sxs-lookup"><span data-stu-id="41b3d-121">**Reinstall the driver**</span></span>

<span data-ttu-id="41b3d-122">Jeśli nie możesz zaktualizować za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie internetowej producenta, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="41b3d-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="41b3d-123">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) sterownik audio i wybierz polecenie **Odinstaluj**.</span><span class="sxs-lookup"><span data-stu-id="41b3d-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="41b3d-124">Uruchom ponownie urządzenie, a system Windows spróbuje ponownie zainstalować sterownik.</span><span class="sxs-lookup"><span data-stu-id="41b3d-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="41b3d-125">Jeśli ponowna instalacja sterownika nie działa, spróbuj użyć ogólnego sterownika audio, który jest dostarczany z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="41b3d-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="41b3d-126">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) sterownik audio > Aktualizuj oprogramowanie sterownika Przeglądaj mój komputer w celu wybrania oprogramowania sterownika Pozwól mi wybrać z listy sterowników urządzeń na moim komputerze , wybierz pozycję Urządzenie audio Hd , wybierz pozycję Dalej i postępuj zgodnie z instrukcjami, aby je  >    >  zainstalować.  </span><span class="sxs-lookup"><span data-stu-id="41b3d-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
