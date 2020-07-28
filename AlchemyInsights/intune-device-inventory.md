---
title: Spis urządzeń usługi Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440472"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="849a2-102">Spis urządzeń usługi Intune</span><span class="sxs-lookup"><span data-stu-id="849a2-102">Intune Device Inventory</span></span>

<span data-ttu-id="849a2-103">Blok Urządzenia zapewnia administratorowi wgląd w urządzenia pod zarządzaniem w usłudze Intune na podstawie na urządzenie.</span><span class="sxs-lookup"><span data-stu-id="849a2-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="849a2-104">Wyświetlane informacje obejmują: sprzęt, odnalezione aplikacje, stan zgodności urządzeń i stan konfiguracji urządzenia.</span><span class="sxs-lookup"><span data-stu-id="849a2-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="849a2-105">Dane spisowe sprzętu i odnalezionych aplikacji są zbierane w cyklu siedmiodniowym.</span><span class="sxs-lookup"><span data-stu-id="849a2-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="849a2-106">Aplikacje i określone elementy zgłaszanego sprzętu różnią się w zależności od systemu operacyjnego urządzenia i tego, czy urządzenie jest własnością osobistą, czy firmową.</span><span class="sxs-lookup"><span data-stu-id="849a2-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="849a2-107">Aby uzyskać więcej informacji, zobacz [Informacje o urządzeniu w usłudze Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="849a2-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="849a2-108">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="849a2-108">**FAQ**</span></span>

<span data-ttu-id="849a2-109">P: Nie otrzymuję pełnej listy zapasów aplikacji znajdujących się na urządzeniach z systemem Windows zarejestrowanych w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="849a2-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="849a2-110">Dlaczego nie?</span><span class="sxs-lookup"><span data-stu-id="849a2-110">Why not?</span></span>

<span data-ttu-id="849a2-111">Odp.: Obecnie tylko nowoczesne aplikacje są wyświetlane dla komputerów z systemem Windows 10, które są identyfikowane jako urządzenia firmowe.</span><span class="sxs-lookup"><span data-stu-id="849a2-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="849a2-112">Usługa Intune nie zbiera informacji o aplikacjach Win32 zainstalowanych na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="849a2-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="849a2-113">P: Dlaczego numery telefonów nie są zbierane ze wszystkich urządzeń?</span><span class="sxs-lookup"><span data-stu-id="849a2-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="849a2-114">Odp.: Telefony sklasyfikowane jako urządzenia firmowe w usłudze Intune nie są identyfikowane z ich pełnym numerem telefonu, gdy na przykład uruchomisz raport o spisie urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="849a2-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="849a2-115">Numery telefonów bring-you-own-device są zawsze częściowo zamaskowane gwiazdkami (\*\*\*\*) i pokazują tylko cztery ostatnie cyfry.</span><span class="sxs-lookup"><span data-stu-id="849a2-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>