---
title: Ustawienia uruchamiania w systemie Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751145"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="c7683-102">Ustawienia uruchamiania w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="c7683-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="c7683-103">**Zmienianie aplikacji uruchamianych automatycznie podczas uruchamiania**</span><span class="sxs-lookup"><span data-stu-id="c7683-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="c7683-104">Przejdź do obszaru [ustawienia > aplikacje > uruchamiania](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c7683-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="c7683-105">Upewnij się, że wszystkie aplikacje, które chcesz uruchomić podczas uruchamiania, są **włączone.**</span><span class="sxs-lookup"><span data-stu-id="c7683-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="c7683-106">**Dodawanie aplikacji w celu automatycznego uruchamiania podczas uruchamiania**</span><span class="sxs-lookup"><span data-stu-id="c7683-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="c7683-107">Kliknij lub naciśnij pozycję **Rozpocznij** i Znajdź aplikację, którą chcesz uruchomić podczas uruchamiania.</span><span class="sxs-lookup"><span data-stu-id="c7683-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="c7683-108">Kliknij prawym przyciskiem myszy aplikację, kliknij pozycję **więcej**, a następnie kliknij pozycję **Otwórz lokalizację pliku**.</span><span class="sxs-lookup"><span data-stu-id="c7683-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="c7683-109">Spowoduje to otwarcie lokalizacji, w której zostanie zapisany skrót do aplikacji.</span><span class="sxs-lookup"><span data-stu-id="c7683-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="c7683-110">Jeśli nie ma opcji otwierania lokalizacji pliku, oznacza to, że aplikacja nie będzie działać podczas uruchamiania.</span><span class="sxs-lookup"><span data-stu-id="c7683-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="c7683-111">Po otwarciu lokalizacji pliku naciśnij klawisze **logo Windows + R**, wpisz **powłokę: uruchamianie**, a następnie kliknij przycisk **OK**.</span><span class="sxs-lookup"><span data-stu-id="c7683-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="c7683-112">Zostanie otwarty folder Autostart.</span><span class="sxs-lookup"><span data-stu-id="c7683-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="c7683-113">Skopiuj i Wklej skrót do aplikacji z lokalizacji pliku do folderu Autostart.</span><span class="sxs-lookup"><span data-stu-id="c7683-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="c7683-114">**Zaawansowane opcje uruchamiania (w tym tryb awaryjny, ustawienia UEFI i rozruch z innego urządzenia)**</span><span class="sxs-lookup"><span data-stu-id="c7683-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="c7683-115">Zapisz swoją pracę i Zamknij wszystkie otwarte dokumenty, ponieważ te czynności spowodują ponowne uruchomienie komputera.</span><span class="sxs-lookup"><span data-stu-id="c7683-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="c7683-116">Przejdź do obszaru [ustawienia > aktualizowanie & zabezpieczenia > odzyskiwanie](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="c7683-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="c7683-117">W obszarze **Uruchamianie zaawansowane**kliknij pozycję **Uruchom ponownie teraz**.</span><span class="sxs-lookup"><span data-stu-id="c7683-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="c7683-118">Po ponownym uruchomieniu komputera na ekranie wybierz opcję:</span><span class="sxs-lookup"><span data-stu-id="c7683-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="c7683-119">Aby wykonać rozruch z urządzenia podobnego do dysku USB, kliknij pozycję **Użyj urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="c7683-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="c7683-120">Aby wprowadzić ustawienia interfejsu UEFI (czasami nazywane konfiguracją systemu BIOS), kliknij pozycję **Rozwiązywanie problemów > opcje zaawansowane > ustawienia oprogramowania UEFI**.</span><span class="sxs-lookup"><span data-stu-id="c7683-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="c7683-121">Aby wprowadzić tryb awaryjny lub zmienić zaawansowane ustawienia uruchamiania, kliknij pozycję **Rozwiązywanie problemów > opcje zaawansowane > ustawienia uruchamiania**, a następnie kliknij pozycję **Uruchom ponownie**.</span><span class="sxs-lookup"><span data-stu-id="c7683-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="c7683-122">Może zostać wyświetlony monit o wprowadzenie [klucza odzyskiwania funkcji BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="c7683-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="c7683-123">Po ponownym uruchomieniu komputera kliknij ustawienie uruchamiania, którego chcesz użyć.</span><span class="sxs-lookup"><span data-stu-id="c7683-123">After your PC restarts again, click the startup setting you want to use.</span></span>