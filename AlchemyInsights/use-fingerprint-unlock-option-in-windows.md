---
title: Korzystanie z opcji odblokowywania za pomocą linii papilarnych w systemie Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796687"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="f1116-102">Korzystanie z opcji odblokowywania za pomocą linii papilarnych w systemie Windows 10</span><span class="sxs-lookup"><span data-stu-id="f1116-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="f1116-103">**Włącz funkcję Windows Hello Fingerprint**</span><span class="sxs-lookup"><span data-stu-id="f1116-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="f1116-104">Aby odblokować system Windows 10 przy użyciu linii papilarnych, musisz skonfigurować rozpoznawanie linii papilarnych przez dodanie co najmniej jednego palca (pozwalając systemowi Windows nauczyć się jego rozpoznawania).</span><span class="sxs-lookup"><span data-stu-id="f1116-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="f1116-105">Przejdź do **ustawień > Konta > opcje** logowania (lub kliknij [tutaj).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="f1116-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="f1116-106">Zostaną wyświetlone dostępne opcje logowania.</span><span class="sxs-lookup"><span data-stu-id="f1116-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="f1116-107">Przykład:</span><span class="sxs-lookup"><span data-stu-id="f1116-107">For example:</span></span>

    ![Opcje logowania.](media/sign-in-options.png)

2. <span data-ttu-id="f1116-109">Kliknij lub naciśnij pozycję **Linii papilarnych funkcji Windows Hello**, a następnie kliknij pozycję **Skonfiguruj**.</span><span class="sxs-lookup"><span data-stu-id="f1116-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="f1116-110">W oknie konfiguracji funkcji Windows Hello kliknij pozycję **Wprowadzenie**.</span><span class="sxs-lookup"><span data-stu-id="f1116-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="f1116-111">Czujnik linii papilarnych zostanie aktywowany i zostaniesz poproszony o włodenie palca do czujnika:</span><span class="sxs-lookup"><span data-stu-id="f1116-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Czujnik linii papilarnych.](media/fingerprint-sensor.png)

3. <span data-ttu-id="f1116-113">Postępuj zgodnie z instrukcjami, które będą zawierały prośbę o wielokrotne skanowanie palcem.</span><span class="sxs-lookup"><span data-stu-id="f1116-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="f1116-114">Po zakończeniu będziesz mieć możliwość dodawania innych palców, których możesz używać do logowania się.</span><span class="sxs-lookup"><span data-stu-id="f1116-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="f1116-115">Następnym razem, gdy zalogujesz się do systemu Windows 10, będzie można użyć odcisku palca w tym celu.</span><span class="sxs-lookup"><span data-stu-id="f1116-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="f1116-116">**Funkcja Windows Hello Fingerprint nie jest dostępna jako opcja logowania**</span><span class="sxs-lookup"><span data-stu-id="f1116-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="f1116-117">Jeśli funkcja Windows Hello Fingerprint nie jest wyświetlana jako opcja w opcjach **logowania,** oznacza to, że system Windows nie zna czytnika/skanera linii papilarnych dołączonych do komputera lub że zasady systemowe uniemożliwiają ich użycie (jeśli na przykład Twój komputer jest zarządzany przez Twoje miejsce pracy).</span><span class="sxs-lookup"><span data-stu-id="f1116-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="f1116-118">Aby rozwiązać problemy:</span><span class="sxs-lookup"><span data-stu-id="f1116-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="f1116-119">Wybierz przycisk **Start** na pasku zadań i wyszukaj menedżer **urządzeń**.</span><span class="sxs-lookup"><span data-stu-id="f1116-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="f1116-120">Kliknij lub naciśnij, aby **otworzyć Menedżera urządzeń.**</span><span class="sxs-lookup"><span data-stu-id="f1116-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="f1116-121">W Menedżerze urządzeń rozwiń pozycję Biometryczne urządzenia, klikając jej link.</span><span class="sxs-lookup"><span data-stu-id="f1116-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices.png)

4. <span data-ttu-id="f1116-123">Twój skaner linii papilarnych powinien być wymieniony jako urządzenie biometryczne, takie jak skaner WBDItics:</span><span class="sxs-lookup"><span data-stu-id="f1116-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Urządzenia biometryczne.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="f1116-125">Jeśli twój skaner linii papilarnych nie jest widoczny, a skaner jest zintegrowany z komputerem, przejdź do witryny internetowej producenta komputera.</span><span class="sxs-lookup"><span data-stu-id="f1116-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="f1116-126">W sekcji pomocy technicznej dotyczącej modelu komputera wyszukaj sterownik systemu Windows 10, który możesz zainstalować.</span><span class="sxs-lookup"><span data-stu-id="f1116-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="f1116-127">Jeśli skaner jest oddzielony od komputera (podłączony przez USB), przejdź do witryny internetowej producenta skanera, aby znaleźć i zainstalować oprogramowanie sterownika urządzenia z systemem Windows 10 dla posiadaowego modelu skanera.</span><span class="sxs-lookup"><span data-stu-id="f1116-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
