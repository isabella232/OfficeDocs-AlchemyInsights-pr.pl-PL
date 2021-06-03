---
title: Tworzenie tagów lub grup urządzeń i zarządzanie nimi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731671"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="c3177-102">Tworzenie tagów lub grup urządzeń i zarządzanie nimi</span><span class="sxs-lookup"><span data-stu-id="c3177-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="c3177-103">Dodawanie tagów na urządzeniach w celu utworzenia logicznego przynależności do grupy.</span><span class="sxs-lookup"><span data-stu-id="c3177-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="c3177-104">Tagi urządzeń obsługują prawidłowe mapowanie sieci, umożliwiając dołączanie różnych tagów w celu przechwytywania kontekstu i umożliwienia dynamicznego tworzenia list w ramach zdarzenia.</span><span class="sxs-lookup"><span data-stu-id="c3177-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="c3177-105">Tagi mogą być używane jako filtr w widoku listy Urządzenia lub do grupowania urządzeń.</span><span class="sxs-lookup"><span data-stu-id="c3177-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="c3177-106">Aby uzyskać więcej informacji na temat grupowania urządzeń, zobacz [Tworzenie tagów urządzeń i zarządzanie nimi.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="c3177-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="c3177-107">Do urządzeń można dodawać tagi, takie jak:</span><span class="sxs-lookup"><span data-stu-id="c3177-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="c3177-108">Korzystanie z portalu</span><span class="sxs-lookup"><span data-stu-id="c3177-108">Using the portal</span></span>

- <span data-ttu-id="c3177-109">Ustawianie wartości klucza rejestru</span><span class="sxs-lookup"><span data-stu-id="c3177-109">Setting a registry key value</span></span>
 
<span data-ttu-id="c3177-110">**Uwaga:** Może brakować opóźnienia między dodaniem tagu do urządzenia a jego dostępnością na liście urządzeń i na stronie urządzenia.</span><span class="sxs-lookup"><span data-stu-id="c3177-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="c3177-111">Aby dodać tagi urządzeń przy użyciu interfejsu API, zobacz [Dodawanie lub usuwanie interfejsu API tagów urządzeń.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="c3177-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="c3177-112">Dodawanie tagów urządzeń i zarządzanie nimi za pomocą portalu</span><span class="sxs-lookup"><span data-stu-id="c3177-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="c3177-113">Wybierz urządzenie, na którym chcesz zarządzać tagami.</span><span class="sxs-lookup"><span data-stu-id="c3177-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="c3177-114">Możesz wybrać lub wyszukać urządzenie w dowolnym z następujących widoków:</span><span class="sxs-lookup"><span data-stu-id="c3177-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="c3177-115">**Pulpit nawigacyjny operacji zabezpieczeń** Wybierz nazwę urządzenia w sekcji Najważniejsze urządzenia z aktywnymi alertami.</span><span class="sxs-lookup"><span data-stu-id="c3177-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="c3177-116">**Kolejka alertów** — wybierz nazwę urządzenia obok ikony urządzenia w kolejce alertów.</span><span class="sxs-lookup"><span data-stu-id="c3177-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="c3177-117">**Lista Urządzenia** — wybierz nazwę urządzenia z listy urządzeń.</span><span class="sxs-lookup"><span data-stu-id="c3177-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="c3177-118">**Pole wyszukiwania** — wybierz pozycję Urządzenie z menu rozwijanego i wprowadź nazwę urządzenia.</span><span class="sxs-lookup"><span data-stu-id="c3177-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="c3177-119">Możesz również przejść do strony alertu za pośrednictwem widoków pliku i adresów IP.</span><span class="sxs-lookup"><span data-stu-id="c3177-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="c3177-120">Wybierz **pozycję Zarządzaj tagami** w wierszu akcji odpowiedzi.</span><span class="sxs-lookup"><span data-stu-id="c3177-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="c3177-121">Wpisz, aby znaleźć lub utworzyć tagi.</span><span class="sxs-lookup"><span data-stu-id="c3177-121">Type to find or create tags.</span></span>

<span data-ttu-id="c3177-122">Tagi są dodawane do widoku urządzenia i są odzwierciedlane w widoku listy Urządzenia.</span><span class="sxs-lookup"><span data-stu-id="c3177-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="c3177-123">Następnie możesz użyć filtru Tagi, aby wyświetlić odpowiednią listę urządzeń.</span><span class="sxs-lookup"><span data-stu-id="c3177-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="c3177-124">Aby uzyskać więcej informacji, [zobacz Tworzenie tagów urządzeń i zarządzanie nimi.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="c3177-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>