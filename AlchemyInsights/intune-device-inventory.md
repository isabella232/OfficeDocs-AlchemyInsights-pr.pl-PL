---
title: Spis urządzeń w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667888"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="83474-102">Spis urządzeń w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="83474-102">Intune Device Inventory</span></span>

<span data-ttu-id="83474-103">Blok urządzenia zapewnia administratorowi wgląd w urządzenia w obszarze Zarządzanie w usłudze Intune na zasadzie na urządzenie.</span><span class="sxs-lookup"><span data-stu-id="83474-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="83474-104">Wyświetlane informacje obejmują: Sprzęt, odnalezione aplikacje, stan zgodności urządzenia i stan konfiguracji urządzenia.</span><span class="sxs-lookup"><span data-stu-id="83474-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="83474-105">Dane spisu dla sprzętu i wykrytych aplikacji są zbierane w cyklu siedmiu dni.</span><span class="sxs-lookup"><span data-stu-id="83474-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="83474-106">Aplikacje i określone elementy sprzętu są różne w zależności od systemu operacyjnego urządzenia oraz tego, czy jest to urządzenie osobiste, czy firmowe.</span><span class="sxs-lookup"><span data-stu-id="83474-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="83474-107">Aby uzyskać więcej informacji, zobacz [Wyświetlanie szczegółów urządzenia w usłudze Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="83474-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="83474-108">**CZĘSTO ZADAWANE PYTANIA**</span><span class="sxs-lookup"><span data-stu-id="83474-108">**FAQ**</span></span>

<span data-ttu-id="83474-109">P: nie otrzymuję pełnej listy spisu aplikacji obecnej na urządzeniu z systemem Windows, na których zarejestrowano usługę Intune.</span><span class="sxs-lookup"><span data-stu-id="83474-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="83474-110">Dlaczego nie?</span><span class="sxs-lookup"><span data-stu-id="83474-110">Why not?</span></span>

<span data-ttu-id="83474-111">O: w tym momencie są wyświetlane tylko aplikacje nowoczesne dla komputerów z systemem Windows 10, które są zidentyfikowane jako urządzenia firmowe.</span><span class="sxs-lookup"><span data-stu-id="83474-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="83474-112">Usługa Intune nie gromadzi informacji o aplikacjach Win32 zainstalowanych na tych urządzeniach.</span><span class="sxs-lookup"><span data-stu-id="83474-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="83474-113">P: Dlaczego numery telefonów nie są zbierane ze wszystkich urządzeń?</span><span class="sxs-lookup"><span data-stu-id="83474-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="83474-114">A: telefony skategoryzowane jako urządzenia firmowe w usłudze Intune nie są zidentyfikowane wraz z pełnym numerem telefonu, na przykład na potrzeby uruchamiania raportu spisu urządzeń przenośnych.</span><span class="sxs-lookup"><span data-stu-id="83474-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="83474-115">Poręczne numery telefonów urządzeń są zawsze częściowo maskowane znakami gwiazdki (\* \* \* \*) i są wyświetlane tylko cztery ostatnie cyfry.</span><span class="sxs-lookup"><span data-stu-id="83474-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>