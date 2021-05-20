---
title: Problemy z usuwaniem wyeksłowanych lub likwidowanych urządzeń ze spisu urządzeń
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564344"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="27ac5-102">Problemy z usuwaniem wyeksłowanych lub likwidowanych urządzeń ze spisu urządzeń</span><span class="sxs-lookup"><span data-stu-id="27ac5-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="27ac5-103">Usługa Microsoft Defender for Endpoint obecnie nie pozwala na ręczne usuwanie rekordu urządzenia wyzysłowego lub likwidowanego z wykazu urządzeń.</span><span class="sxs-lookup"><span data-stu-id="27ac5-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="27ac5-104">Ze względów bezpieczeństwa urządzenie pozostaje w portalu jako rekord historyczny przez maksymalnie 180 dni.</span><span class="sxs-lookup"><span data-stu-id="27ac5-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="27ac5-105">Jednak dane urządzenia są czyszowane zgodnie ze skonfigurowanym okresem przechowywania.</span><span class="sxs-lookup"><span data-stu-id="27ac5-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="27ac5-106">**Uwaga:** Urządzenie wyeksłowane lub  likwidowane jest automatycznie przełączane do stanu nieaktywnego po upływie siedmiu dni.</span><span class="sxs-lookup"><span data-stu-id="27ac5-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="27ac5-107">Ponadto urządzenia, które nie są aktywne w ciągu ostatnich 30 dni, nie są odzwierciedlane w danych, które odzwierciedlają twoją organizację Zarządzanie zagrożeniami i lukami wyników ekspozycji lub bezpiecznego wyniku działania firmy Microsoft dla urządzeń.</span><span class="sxs-lookup"><span data-stu-id="27ac5-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="27ac5-108">Jeśli nadal nie chcesz wyświetlać niektórych urządzeń w widoku Spis urządzeń, spróbuj użyć tagu urządzenia w celu odfiltrowanie zlikwidowanych urządzeń w widoku Spis urządzeń.</span><span class="sxs-lookup"><span data-stu-id="27ac5-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="27ac5-109">Aby uzyskać więcej informacji, zobacz:</span><span class="sxs-lookup"><span data-stu-id="27ac5-109">For more information, see:</span></span>

[<span data-ttu-id="27ac5-110">Urządzenia wye webboard z usługi Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="27ac5-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="27ac5-111">Wynik ekspozycji w Zarządzanie zagrożeniami i lukami</span><span class="sxs-lookup"><span data-stu-id="27ac5-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="27ac5-112">Naprawianie czujników o złej kondycji w programie Microsoft Defender dla punktu końcowego</span><span class="sxs-lookup"><span data-stu-id="27ac5-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="27ac5-113">Jak efektywnie korzystać z otagowania (część 1)</span><span class="sxs-lookup"><span data-stu-id="27ac5-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="27ac5-114">Jak efektywnie korzystać z otagowania (część 2)</span><span class="sxs-lookup"><span data-stu-id="27ac5-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="27ac5-115">Jak efektywnie korzystać z otagowania (część 3)</span><span class="sxs-lookup"><span data-stu-id="27ac5-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




