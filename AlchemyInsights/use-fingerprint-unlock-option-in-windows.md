---
title: Używanie opcji odblokowywania odcisku palca w systemie Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795254"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="dd6f2-102">Używanie opcji odblokowywania odcisku palca w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="dd6f2-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="dd6f2-103">**Włączanie odcisku palca Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="dd6f2-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="dd6f2-104">Aby odblokować system Windows 10 przy użyciu odcisku palca, musisz skonfigurować odcisk cyfrowy funkcji Windows Hello, dodając (pozwalając systemowi Windows na rozpoznanie) co najmniej jednego palca.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="dd6f2-105">Przejdź do obszaru **ustawienia > konta > opcji logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="dd6f2-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="dd6f2-106">Zostaną wyświetlone dostępne opcje logowania.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="dd6f2-107">Przykład:</span><span class="sxs-lookup"><span data-stu-id="dd6f2-107">For example:</span></span>

    ![Opcje logowania.](media/sign-in-options.png)

2. <span data-ttu-id="dd6f2-109">Kliknij lub naciśnij pozycję **odciskiem palca Windows Hello**, a następnie kliknij pozycję **Konfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="dd6f2-110">W oknie Konfiguracja usługi Windows Hello kliknij pozycję **Rozpocznij**.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="dd6f2-111">Czujnik linii papilarnych zostanie aktywowany, a użytkownik zostanie poproszony o umieszczenie palca na czujniku:</span><span class="sxs-lookup"><span data-stu-id="dd6f2-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Czujnik odcisku palca.](media/fingerprint-sensor.png)

3. <span data-ttu-id="dd6f2-113">Postępuj zgodnie z instrukcjami, co spowoduje wyświetlenie monitu o powtarzanie skanowania palca.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="dd6f2-114">Po zakończeniu tej opcji będziesz mieć możliwość dodawania innych palców, których możesz użyć do logowania się.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="dd6f2-115">Gdy następnym razem zalogujesz się do systemu Windows 10, będziesz mieć możliwość skorzystania z odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="dd6f2-116">**Odcisk palca Windows Hello niedostępny jako opcja logowania**</span><span class="sxs-lookup"><span data-stu-id="dd6f2-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="dd6f2-117">Jeśli odcisk palca funkcji Windows Hello nie jest widoczny jako opcja w **opcjach logowania**, oznacza to, że system Windows nie rozpoznaje żadnego czytnika linii papilarnych ani skanera podłączonego do komputera lub zasady systemowe uniemożliwiają korzystanie z nich (Jeśli na przykład komputer jest zarządzany przez miejsce pracy).</span><span class="sxs-lookup"><span data-stu-id="dd6f2-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="dd6f2-118">Aby rozwiązać problem:</span><span class="sxs-lookup"><span data-stu-id="dd6f2-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="dd6f2-119">Wybierz przycisk **Start** na pasku zadań i Wyszukaj pozycję **Menedżer urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="dd6f2-120">Kliknij lub naciśnij, aby otworzyć **Menedżera urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="dd6f2-121">W Menedżerze urządzeń rozwiń węzeł Urządzenia biometryczne, klikając jego Pagon.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. <span data-ttu-id="dd6f2-123">Skaner linii papilarnych powinien być wymieniony na urządzeniu biometrycznym, na przykład w skanerze Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="dd6f2-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="dd6f2-125">Jeśli skaner linii papilarnych nie jest widoczny, a skaner jest zintegrowany z komputerem, przejdź do witryny producenta komputera w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="dd6f2-126">W sekcji Pomoc techniczna dotycząca modelu komputerów Wyszukaj sterownik systemu Windows 10, aby skaner mógł zostać zainstalowany.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="dd6f2-127">Jeśli skaner jest niezależny od komputera (dołączonego za pośrednictwem magistrali USB), przejdź do witryny producenta skanera w sieci Web, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia w systemie Windows 10 dla modelu skanera.</span><span class="sxs-lookup"><span data-stu-id="dd6f2-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
