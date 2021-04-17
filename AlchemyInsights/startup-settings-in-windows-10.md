---
title: Ustawienia uruchamiania w systemie Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828162"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="65222-102">Ustawienia uruchamiania w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="65222-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="65222-103">**Zmienianie aplikacji uruchomionych automatycznie podczas uruchamiania**</span><span class="sxs-lookup"><span data-stu-id="65222-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="65222-104">Przejdź do [strony Ustawienia > Uruchamianie > uruchamianie.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="65222-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="65222-105">Upewnij się, że każda aplikacja, która ma być uruchamiana podczas uruchamiania, jest **włączona.**</span><span class="sxs-lookup"><span data-stu-id="65222-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="65222-106">**Dodawanie aplikacji, która będzie uruchamiana automatycznie przy uruchamianiu**</span><span class="sxs-lookup"><span data-stu-id="65222-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="65222-107">Kliknij lub naciśnij **przycisk Start** i znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.</span><span class="sxs-lookup"><span data-stu-id="65222-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="65222-108">Kliknij aplikację prawym przyciskiem myszy, kliknij pozycję **Więcej**, a następnie kliknij **pozycję Otwórz lokalizację pliku**.</span><span class="sxs-lookup"><span data-stu-id="65222-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="65222-109">Spowoduje to otwarcie lokalizacji, w której został zapisany skrót do aplikacji.</span><span class="sxs-lookup"><span data-stu-id="65222-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="65222-110">Jeśli nie ma opcji Otwórz lokalizację pliku, oznacza to, że aplikacja nie może być uruchamiana podczas uruchamiania.</span><span class="sxs-lookup"><span data-stu-id="65222-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="65222-111">Po otwarciu lokalizacji pliku naciśnij klawisze **logo Windows + R,** wpisz **shell:startup,** a następnie kliknij przycisk **OK.**</span><span class="sxs-lookup"><span data-stu-id="65222-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="65222-112">Zostanie otwarty folder Autostart.</span><span class="sxs-lookup"><span data-stu-id="65222-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="65222-113">Skopiuj skrót do aplikacji i wklej go z lokalizacji pliku do folderu Autostart.</span><span class="sxs-lookup"><span data-stu-id="65222-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="65222-114">**Zaawansowane opcje uruchamiania (w tym tryb awaryjny, ustawienia UEFI i rozruch z innego urządzenia)**</span><span class="sxs-lookup"><span data-stu-id="65222-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="65222-115">Zapisz pracę i zamknij wszystkie otwarte dokumenty, ponieważ spowoduje to ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="65222-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="65222-116">Przejdź do [strony Ustawienia > i & w celu > zabezpieczeń.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="65222-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="65222-117">W **obszarze Uruchamianie zaawansowane** kliknij pozycję Uruchom ponownie **teraz.**</span><span class="sxs-lookup"><span data-stu-id="65222-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="65222-118">Po ponownym uruchomieniu komputera i wybraniu ekranu Wybierz opcję:</span><span class="sxs-lookup"><span data-stu-id="65222-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="65222-119">Aby uruchomić komputer z urządzenia, takiego jak dysk USB, kliknij **pozycję Użyj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="65222-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="65222-120">Aby wprowadzić ustawienia UEFI (czasami nazywane konfiguracją KARTO), kliknij pozycję Rozwiązywanie problemów z > zaawansowane opcje > ustawienia oprogramowania **układowego UEFI.**</span><span class="sxs-lookup"><span data-stu-id="65222-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="65222-121">Aby wejść w tryb awaryjny lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję Rozwiązywanie problemów z > zaawansowane > Ustawienia **uruchamiania**, a następnie kliknij pozycję Uruchom **ponownie.**</span><span class="sxs-lookup"><span data-stu-id="65222-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="65222-122">Może pojawić się monit o wprowadzenie klucza [odzyskiwania funkcji BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="65222-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="65222-123">Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.</span><span class="sxs-lookup"><span data-stu-id="65222-123">After your PC restarts again, click the startup setting you want to use.</span></span>