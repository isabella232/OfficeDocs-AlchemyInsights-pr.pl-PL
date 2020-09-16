---
title: Rozwiązywanie problemów z dźwiękiem w systemie Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750321"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="bdb32-102">Rozwiązywanie problemów z dźwiękiem w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="bdb32-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="bdb32-103">**Uruchamianie narzędzia do rozwiązywania problemów z dźwiękiem**</span><span class="sxs-lookup"><span data-stu-id="bdb32-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="bdb32-104">Otwórz [Ustawienia rozwiązywania problemów](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="bdb32-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="bdb32-105">Wybieranie opcji **odtwarzania audio**  >  **Uruchom narzędzie do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="bdb32-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="bdb32-106">**Ustawianie urządzenia domyślnego**</span><span class="sxs-lookup"><span data-stu-id="bdb32-106">**Set the default device**</span></span>

<span data-ttu-id="bdb32-107">Jeśli łączysz się z urządzeniem audio przy użyciu magistrali USB lub HDMI, być może trzeba ustawić to urządzenie jako domyślne:</span><span class="sxs-lookup"><span data-stu-id="bdb32-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="bdb32-108">Otwórz **Start**  >  **dźwięk**Start, a następnie wybierz pozycję **dźwięk** lub **Zmień dźwięki systemowe** z listy wyników.</span><span class="sxs-lookup"><span data-stu-id="bdb32-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="bdb32-109">Na karcie **odtwarzanie** wybierz urządzenie, wybierz pozycję **Ustaw domyślne**, a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="bdb32-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="bdb32-110">**Sprawdzanie kabli, głośności, głośników i słuchawek**</span><span class="sxs-lookup"><span data-stu-id="bdb32-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="bdb32-111">Sprawdź połączenia głośników i słuchawek, aby uzyskać kable i upewnić się, że są podłączone do właściwego złącza.</span><span class="sxs-lookup"><span data-stu-id="bdb32-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="bdb32-112">Sprawdź poziomy zasilania i głośności, a następnie spróbuj wyłączyć regulatory głośności.</span><span class="sxs-lookup"><span data-stu-id="bdb32-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="bdb32-113">Niektóre głośniki i aplikacje mają własne regulatory głośności; może być konieczne sprawdzenie wszystkich, aby upewnić się, że są na odpowiednim poziomie.</span><span class="sxs-lookup"><span data-stu-id="bdb32-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="bdb32-114">Spróbuj połączyć się przy użyciu innego portu USB.</span><span class="sxs-lookup"><span data-stu-id="bdb32-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="bdb32-115">**Uwaga**: Pamiętaj, że głośniki mogą nie działać po podłączeniu słuchawek.</span><span class="sxs-lookup"><span data-stu-id="bdb32-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="bdb32-116">**Sprawdzanie Menedżera urządzeń**</span><span class="sxs-lookup"><span data-stu-id="bdb32-116">**Check Device Manager**</span></span>

<span data-ttu-id="bdb32-117">Aby upewnić się, że sterowniki są aktualne:</span><span class="sxs-lookup"><span data-stu-id="bdb32-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="bdb32-118">Wybierz pozycję **Start**, wpisz polecenie **Menedżer urządzeń**, a następnie wybierz pozycję **Menedżer urządzeń** z listy wyników.</span><span class="sxs-lookup"><span data-stu-id="bdb32-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="bdb32-119">W obszarze **Kontrolery dźwięku, wideo i gier**wybierz kartę dźwiękową, otwórz ją, wybierz kartę **Sterownik** i wybierz pozycję **Aktualizuj sterownik**.</span><span class="sxs-lookup"><span data-stu-id="bdb32-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="bdb32-120">**Uwaga**: Jeśli system Windows nie znajdzie nowego sterownika, poszukaj go w witrynie internetowej producenta urządzenia i postępuj zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="bdb32-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="bdb32-121">**Ponowne instalowanie sterownika**</span><span class="sxs-lookup"><span data-stu-id="bdb32-121">**Reinstall the driver**</span></span>

<span data-ttu-id="bdb32-122">Jeśli nie możesz zaktualizować się za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie internetowej producenta, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="bdb32-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="bdb32-123">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, a następnie wybierz pozycję **Odinstaluj**.</span><span class="sxs-lookup"><span data-stu-id="bdb32-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="bdb32-124">Uruchom ponownie urządzenie, a system Windows podejmie próbę ponownego zainstalowania sterownika.</span><span class="sxs-lookup"><span data-stu-id="bdb32-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="bdb32-125">Jeśli ponowna instalacja sterownika nie zadziała, spróbuj użyć uniwersalnego sterownika audio, który jest dostarczany z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="bdb32-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="bdb32-126">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, > **Aktualizuj oprogramowanie sterownika**  >  **Przeglądaj mój komputer w poszukiwaniu oprogramowania sterownika**  >  **umożliwia mi wybieranie z listy sterowników urządzeń na komputerze**, wybieranie **urządzenia audio High Definition**, wybieranie **pozycji dalej**i postępuj zgodnie z instrukcjami, aby go zainstalować.</span><span class="sxs-lookup"><span data-stu-id="bdb32-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
