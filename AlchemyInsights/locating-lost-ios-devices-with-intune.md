---
title: Lokalizowanie utraconych urządzeń z systemem iOS za pomocą usługi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440424"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="a1dc2-102">Lokalizowanie utraconych urządzeń z systemem iOS za pomocą usługi Intune</span><span class="sxs-lookup"><span data-stu-id="a1dc2-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="a1dc2-103">Włączenie trybu utraconego na urządzeniu z systemem iOS umożliwia administratorowi wyświetlanie na ekranie blokady wiadomości i numeru telefonu kontaktowego.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="a1dc2-104">Po włączeniu trybu utraconego administrator może użyć akcji Znajdź urządzenie, aby zidentyfikować fizyczną lokalizację urządzenia.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="a1dc2-105">Akcja Znajdź urządzenie w usłudze Intune współpracuje z urządzeniami z systemem iOS, aby wyświetlić lokalizację określonego urządzenia na mapie.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="a1dc2-106">Użycie tej akcji wymaga, aby urządzenie z systemem iOS było w:</span><span class="sxs-lookup"><span data-stu-id="a1dc2-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="a1dc2-107">Tryb nadzorowany</span><span class="sxs-lookup"><span data-stu-id="a1dc2-107">Supervised mode</span></span>
- <span data-ttu-id="a1dc2-108">Tryb utracony</span><span class="sxs-lookup"><span data-stu-id="a1dc2-108">Lost mode</span></span>

<span data-ttu-id="a1dc2-109">Aby uzyskać więcej informacji, zobacz [Włączanie trybu utraconego na urządzeniach z systemem iOS/iPadOS z usłudze Intune](https://docs.microsoft.com/intune/device-lost-mode) i [lokalizowanie utraconych lub skradzionych urządzeń z systemem iOS/iPadOS za pomocą usługi Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="a1dc2-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="a1dc2-110">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="a1dc2-110">**FAQ**</span></span>

<span data-ttu-id="a1dc2-111">P: Wydałem zdalną akcję, aby usunąć dane firmy z urządzenia, a teraz utknął w stanie oczekiwania.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="a1dc2-112">Odp.: Aby akcja zdalna została pomyślnie ukończona, urządzenie docelowe musi być w trybie online i w dobrej kondycji.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="a1dc2-113">W następujących sytuacjach akcja zdalna pozostaje w stanie oczekiwania przez 30 dni lub do momentu, gdy urządzenie potwierdzi polecenie:</span><span class="sxs-lookup"><span data-stu-id="a1dc2-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="a1dc2-114">Gdy urządzenie nie ma łączności</span><span class="sxs-lookup"><span data-stu-id="a1dc2-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="a1dc2-115">Gdy urządzenie utraci stan zarządzania w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="a1dc2-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="a1dc2-116">Jeśli uważasz, że urządzenie już nie zaewidencjonuje się i nie będzie można usunąć danych firmowych, wybierz pozycję Usuń.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="a1dc2-117">Usunięcie powoduje usunięcie rekordu urządzenia, tak aby nie był już wyświetlany na liście urządzeń usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="a1dc2-118">Jeśli urządzenie stanie się ponownie aktywne, jego użytkownik będzie musiał go ponownie zarejestrować.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="a1dc2-119">Pyt.: Dlaczego niektóre akcje zdalne nie są dostępne do użycia?</span><span class="sxs-lookup"><span data-stu-id="a1dc2-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="a1dc2-120">Odp.: Nie wszystkie platformy obsługują wszystkie akcje urządzenia zdalnego.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="a1dc2-121">Następujące akcje zdalne są specyficzne dla platformy, więc są one dostępne tylko dla zaznaczonych platform.</span><span class="sxs-lookup"><span data-stu-id="a1dc2-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="a1dc2-122">Blokada aktywacji obejścia (tylko system iOS)</span><span class="sxs-lookup"><span data-stu-id="a1dc2-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="a1dc2-123">Nowy start (tylko windows)</span><span class="sxs-lookup"><span data-stu-id="a1dc2-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="a1dc2-124">Tryb utracony (tylko iOS)</span><span class="sxs-lookup"><span data-stu-id="a1dc2-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="a1dc2-125">Lokalizowanie urządzenia (tylko w systemem iOS)</span><span class="sxs-lookup"><span data-stu-id="a1dc2-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="a1dc2-126">Ponowne uruchomienie (tylko system Windows)</span><span class="sxs-lookup"><span data-stu-id="a1dc2-126">Restart (Windows only)</span></span>

<span data-ttu-id="a1dc2-127">Aby uzyskać więcej informacji na temat każdej akcji, zobacz [Dostępne akcje urządzenia](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="a1dc2-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>