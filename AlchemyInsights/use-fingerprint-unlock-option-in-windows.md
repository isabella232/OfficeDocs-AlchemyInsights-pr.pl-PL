---
title: Korzystanie z opcji odblokowania odcisków palców w systemie Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588325"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2da09-102">Korzystanie z opcji odblokowania odcisków palców w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="2da09-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2da09-103">**Włączanie odcisku palca funkcji Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="2da09-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2da09-104">Aby odblokować system Windows 10 za pomocą odcisku palca, musisz skonfigurować odcisk palca Windows Hello, dodając (pozwalając systemowi Windows nauczyć się rozpoznawać) co najmniej jednym palcem.</span><span class="sxs-lookup"><span data-stu-id="2da09-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2da09-105">Przejdź do **pozycji Ustawienia > konta > opcje logowania** (lub kliknij [tutaj](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="2da09-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2da09-106">Zostaną wyświetlone dostępne opcje logowania.</span><span class="sxs-lookup"><span data-stu-id="2da09-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2da09-107">Na przykład:</span><span class="sxs-lookup"><span data-stu-id="2da09-107">For example:</span></span>

    ![Opcje logowania.](media/sign-in-options.png)

2. <span data-ttu-id="2da09-109">Kliknij lub naciśnij pozycję **Odcisk palca Funkcji Rozpoznawania systemu Windows**, a następnie kliknij pozycję **Konfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="2da09-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2da09-110">W oknie konfiguracji funkcji Windows Hello kliknij pozycję **Wprowadzenie**.</span><span class="sxs-lookup"><span data-stu-id="2da09-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2da09-111">Czujnik odcisków palców zostanie aktywowany, a ty zostaniesz poproszony o umieszczenie palca na czujniku:</span><span class="sxs-lookup"><span data-stu-id="2da09-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Linii papilarnych.](media/fingerprint-sensor.png)

3. <span data-ttu-id="2da09-113">Postępuj zgodnie z instrukcjami, które proszą o wielokrotne skanowanie palca.</span><span class="sxs-lookup"><span data-stu-id="2da09-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2da09-114">Po zakończeniu tej opcji możesz dodać inne palce, których możesz użyć do logowania.</span><span class="sxs-lookup"><span data-stu-id="2da09-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2da09-115">Następnym razem, gdy zalogujesz się do systemu Windows 10, będziesz mieć możliwość użycia odcisku palca.</span><span class="sxs-lookup"><span data-stu-id="2da09-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2da09-116">**Windows Hello Fingerprint nie jest dostępny jako opcja logowania**</span><span class="sxs-lookup"><span data-stu-id="2da09-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2da09-117">Jeśli odcisk palca Windows Hello nie jest wyświetlany jako opcja w **opcjach logowania,** oznacza to, że system Windows nie jest świadomy czytnika linii papilarnych / skanera podłączonego do komputera lub że zasady systemowe uniemożliwiają jego użycie (jeśli na przykład komputer jest zarządzany przez miejsce pracy).</span><span class="sxs-lookup"><span data-stu-id="2da09-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2da09-118">Aby rozwiązać problem:</span><span class="sxs-lookup"><span data-stu-id="2da09-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2da09-119">Wybierz przycisk **Start** na pasku zadań i wyszukaj **pozycję Menedżer urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="2da09-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2da09-120">Kliknij lub naciśnij, aby otworzyć **menedżera urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="2da09-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2da09-121">W Menedżerze urządzeń rozwiń urządzenia biometryczne, klikając jego szewron.</span><span class="sxs-lookup"><span data-stu-id="2da09-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. <span data-ttu-id="2da09-123">Skaner linii papilarnych powinien być wymieniony jako urządzenie biometryczne, takie jak skaner Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="2da09-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2da09-125">Jeśli skaner linii papilarnych nie jest wyświetlany, a skaner jest zintegrowany z komputerem, przejdź do witryny producenta komputera w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="2da09-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2da09-126">W sekcji pomocy technicznej dla modelu komputera wyszukaj sterownik systemu Windows 10 dla skanera, który można zainstalować.</span><span class="sxs-lookup"><span data-stu-id="2da09-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2da09-127">Jeśli skaner jest oddzielony od komputera (podłączonego przez USB), przejdź do witryny producenta skanera w sieci Web, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia systemu Windows 10 dla posiadanej modelu skanera.</span><span class="sxs-lookup"><span data-stu-id="2da09-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
