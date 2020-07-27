---
title: Obejście blokady aktywacji na nadzorowanych urządzeniach z systemem iOS za pomocą usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424217"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="5bab2-102">Obejście blokady aktywacji na nadzorowanych urządzeniach z systemem iOS za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="5bab2-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="5bab2-103">Możliwość ominięcia blokady aktywacji na urządzeniach z systemem iOS ułatwia odzyskiwanie po scenariuszu, w którym użytkownik włącza blokadę aktywacji na urządzeniu firmowym, a następnie opuszcza firmę.</span><span class="sxs-lookup"><span data-stu-id="5bab2-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="5bab2-104">Wymagania wstępne do pominięcia blokady aktywacji obejmują:</span><span class="sxs-lookup"><span data-stu-id="5bab2-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="5bab2-105">Urządzenie jest "nadzorowane".</span><span class="sxs-lookup"><span data-stu-id="5bab2-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="5bab2-106">Blokada aktywacji została pomyślnie włączona przy użyciu zasad ograniczeń urządzenia z systemem iOS w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="5bab2-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="5bab2-107">Ponadto, omijając blokadę aktywacji, należy:</span><span class="sxs-lookup"><span data-stu-id="5bab2-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="5bab2-108">Fizycznie posiadają urządzenie jest czyszczone.</span><span class="sxs-lookup"><span data-stu-id="5bab2-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="5bab2-109">Skopiuj kod przed wydaniem czyszczenia.</span><span class="sxs-lookup"><span data-stu-id="5bab2-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="5bab2-110">**Uwaga:** W kodzie czyszczenia nie jest rozróżniana wielkość liter, więc znaki "-" nie są wymagane.</span><span class="sxs-lookup"><span data-stu-id="5bab2-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="5bab2-111">Aby uzyskać szczegółowe informacje, zobacz [Ominięcie blokady aktywacji na nadzorowanych urządzeniach z systemem iOS z usłudze Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="5bab2-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="5bab2-112">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="5bab2-112">**FAQ**</span></span>

<span data-ttu-id="5bab2-113">P: **Wydałem zdalną akcję, aby usunąć dane firmy z urządzenia, a teraz utknął w stanie oczekiwania.**</span><span class="sxs-lookup"><span data-stu-id="5bab2-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="5bab2-114">Odp.: Aby akcja zdalna została pomyślnie ukończona, urządzenie docelowe musi być w trybie online i w dobrej kondycji.</span><span class="sxs-lookup"><span data-stu-id="5bab2-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="5bab2-115">W następujących sytuacjach akcja zdalna pozostaje w stanie oczekiwania przez 30 dni lub do momentu, gdy urządzenie potwierdzi polecenie, gdy urządzenie:</span><span class="sxs-lookup"><span data-stu-id="5bab2-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="5bab2-116">Nie ma łączności.</span><span class="sxs-lookup"><span data-stu-id="5bab2-116">Does not have connectivity.</span></span>
- <span data-ttu-id="5bab2-117">Traci stan zarządzania w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="5bab2-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="5bab2-118">Jeśli uważasz, że urządzenie już nie zaewidencjonuje się i nie usunie danych firmowych, wybierz pozycję Usuń.</span><span class="sxs-lookup"><span data-stu-id="5bab2-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="5bab2-119">Usunięcie powoduje usunięcie rekordu urządzenia, tak aby nie był już wyświetlany na liście urządzeń usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="5bab2-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="5bab2-120">Aby urządzenie ponownie stało się aktywne, jego użytkownik musi ponownie zarejestrować urządzenie.</span><span class="sxs-lookup"><span data-stu-id="5bab2-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="5bab2-121">**Pyt.: Dlaczego niektóre akcje zdalne nie są dostępne do użycia?**</span><span class="sxs-lookup"><span data-stu-id="5bab2-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="5bab2-122">Odp.: Nie wszystkie platformy obsługują wszystkie akcje urządzenia zdalnego.</span><span class="sxs-lookup"><span data-stu-id="5bab2-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="5bab2-123">Następujące akcje zdalne są specyficzne dla platformy.</span><span class="sxs-lookup"><span data-stu-id="5bab2-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="5bab2-124">Blokada aktywacji obejścia (tylko system iOS)</span><span class="sxs-lookup"><span data-stu-id="5bab2-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="5bab2-125">Nowy start (tylko windows)</span><span class="sxs-lookup"><span data-stu-id="5bab2-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="5bab2-126">Tryb utracony (tylko iOS)</span><span class="sxs-lookup"><span data-stu-id="5bab2-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="5bab2-127">Lokalizowanie urządzenia (tylko w systemem iOS)</span><span class="sxs-lookup"><span data-stu-id="5bab2-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="5bab2-128">Ponowne uruchomienie (tylko system Windows)</span><span class="sxs-lookup"><span data-stu-id="5bab2-128">Restart (Windows only)</span></span>

<span data-ttu-id="5bab2-129">Aby uzyskać więcej informacji na temat każdej akcji, zobacz [Dostępne akcje urządzenia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="5bab2-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>