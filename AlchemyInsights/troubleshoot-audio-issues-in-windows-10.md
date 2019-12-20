---
title: Rozwiązywanie problemów z dźwiękiem w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796283"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="83e3c-102">Rozwiązywanie problemów z dźwiękiem w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="83e3c-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="83e3c-103">**Uruchom narzędzie do rozwiązywania problemów z dźwiękiem**</span><span class="sxs-lookup"><span data-stu-id="83e3c-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="83e3c-104">Narzędzie do rozwiązywania problemów z dźwiękiem może automatycznie naprawiać problemy z dźwiękiem:</span><span class="sxs-lookup"><span data-stu-id="83e3c-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="83e3c-105">Wybierz **Start**, wpisz **Rozwiązywanie problemów**, a następnie wybierz **Rozwiązywanie problemów** z listy wyników.</span><span class="sxs-lookup"><span data-stu-id="83e3c-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="83e3c-106">Wybierz opcję **odtwarzanie dźwięku** > **Uruchom narzędzie do rozwiązywania problemów**.</span><span class="sxs-lookup"><span data-stu-id="83e3c-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="83e3c-107">**Sprawdź przewody, głośność, głośniki i słuchawki**</span><span class="sxs-lookup"><span data-stu-id="83e3c-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="83e3c-108">Sprawdź połączenia głośników i słuchawek, aby poluzować przewody i upewnij się, że są podłączone do odpowiedniego gniazda.</span><span class="sxs-lookup"><span data-stu-id="83e3c-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="83e3c-109">Sprawdź poziom mocy i głośności, a następnie spróbuj wyłączyć wszystkie regulatory głośności.</span><span class="sxs-lookup"><span data-stu-id="83e3c-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="83e3c-110">Niektóre głośniki i aplikacje mają własne regulatory głośności, a może trzeba sprawdzić je wszystkie, aby upewnić się, że są na właściwym poziomie.</span><span class="sxs-lookup"><span data-stu-id="83e3c-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="83e3c-111">Spróbuj połączyć się przy użyciu innego portu USB.</span><span class="sxs-lookup"><span data-stu-id="83e3c-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="83e3c-112">**Uwaga:** Pamiętaj, że głośniki mogą nie działać, gdy podłączone są słuchawki.</span><span class="sxs-lookup"><span data-stu-id="83e3c-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="83e3c-113">**Sprawdzanie Menedżera urządzeń**</span><span class="sxs-lookup"><span data-stu-id="83e3c-113">**Check Device Manager**</span></span>

<span data-ttu-id="83e3c-114">Aby upewnić się, że sterowniki są aktualne:</span><span class="sxs-lookup"><span data-stu-id="83e3c-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="83e3c-115">Wybierz pozycję **Start**, wpisz **Menedżer urządzeń**, a następnie z listy wyników wybierz pozycję **Menedżer urządzeń** .</span><span class="sxs-lookup"><span data-stu-id="83e3c-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="83e3c-116">W obszarze **Kontrolery dźwięku, wideo i gier**wybierz kartę dźwiękową, otwórz ją, wybierz kartę **Sterownik** i wybierz pozycję **Aktualizuj sterownik**.</span><span class="sxs-lookup"><span data-stu-id="83e3c-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="83e3c-117">**Uwaga:** Jeśli system Windows nie znajdzie nowego sterownika, poszukaj go w witrynie sieci Web producenta urządzenia i postępuj zgodnie z instrukcjami.</span><span class="sxs-lookup"><span data-stu-id="83e3c-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="83e3c-118">**Ponowna instalacja sterownika**</span><span class="sxs-lookup"><span data-stu-id="83e3c-118">**Reinstall the driver**</span></span>

<span data-ttu-id="83e3c-119">Jeśli nie można zaktualizować za pomocą Menedżera urządzeń lub znaleźć nowego sterownika w witrynie sieci Web producenta, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="83e3c-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="83e3c-120">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio, a następnie wybierz pozycję **Odinstaluj**.</span><span class="sxs-lookup"><span data-stu-id="83e3c-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="83e3c-121">Uruchom ponownie urządzenie, a system Windows spróbuje ponownie zainstalować sterownik.</span><span class="sxs-lookup"><span data-stu-id="83e3c-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="83e3c-122">Jeśli ponowna instalacja sterownika nie działa, spróbuj użyć ogólnego sterownika audio, który jest dostarczany z systemem Windows.</span><span class="sxs-lookup"><span data-stu-id="83e3c-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="83e3c-123">W Menedżerze urządzeń kliknij prawym przyciskiem myszy (lub naciśnij i przytrzymaj) Sterownik audio > **Aktualizuj oprogramowanie** > **sterownika Przeglądaj mój komputer w poszukiwaniu oprogramowania** > sterownika**pozwól mi wybrać z listy sterowników urządzeń na moim komputerze**, wybierz **urządzenie audio High Definition**, wybierz **dalej**i postępuj zgodnie z instrukcjami, aby go zainstalować.</span><span class="sxs-lookup"><span data-stu-id="83e3c-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="83e3c-124">**Ustawianie domyślnego urządzenia**</span><span class="sxs-lookup"><span data-stu-id="83e3c-124">**Set the default device**</span></span>

<span data-ttu-id="83e3c-125">Jeśli łączysz się z urządzeniem audio za pomocą USB lub HDMI, może być konieczne ustawienie tego urządzenia jako domyślnego:</span><span class="sxs-lookup"><span data-stu-id="83e3c-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="83e3c-126">Wybierz **Start**, wpisz **dźwięk**, a następnie wybierz **dźwięk** lub **Zmień dźwięki systemu** z listy wyników.</span><span class="sxs-lookup"><span data-stu-id="83e3c-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="83e3c-127">Na karcie **odtwarzanie** wybierz urządzenie, wybierz opcję **Ustaw domyślne**, a następnie wybierz **przycisk OK**.</span><span class="sxs-lookup"><span data-stu-id="83e3c-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

