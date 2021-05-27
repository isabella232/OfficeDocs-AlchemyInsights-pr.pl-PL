---
title: Stan czujnika sprawdzania punktu końcowego programu Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676341"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="4690a-102">Stan czujnika sprawdzania punktu końcowego programu Defender</span><span class="sxs-lookup"><span data-stu-id="4690a-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="4690a-103">Kafelek **Urządzenia z problemami z** czujnikiem znajduje się na pulpicie nawigacyjnym Operacje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="4690a-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="4690a-104">Ten kafelek zawiera informacje o możliwościach poszczególnych urządzeń w celu przekazywania danych czujnika i komunikowania się z usługą Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="4690a-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="4690a-105">Raportuje ono, ile urządzeń wymaga uwagi i ułatwia zidentyfikowanie urządzeń sprawiających problem oraz podejmie działania w celu poprawienia znanych problemów.</span><span class="sxs-lookup"><span data-stu-id="4690a-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="4690a-106">Dwa wskaźniki stanu na kafelku zapewniają informacje o liczbie urządzeń, które nie zgłaszają poprawnie usługi:</span><span class="sxs-lookup"><span data-stu-id="4690a-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="4690a-107">**Błędnie skonfigurowane** Urządzenia, które mogą częściowo raportować dane czujnika do usługi Defender for Endpoint i mogą mieć błędy konfiguracji, które wymagają korekty.</span><span class="sxs-lookup"><span data-stu-id="4690a-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="4690a-108">**Nieaktywny** Urządzenia, które w ciągu ostatniego miesiąca przestały zgłaszać się do usługi Defender for Endpoint przez ponad siedem dni.</span><span class="sxs-lookup"><span data-stu-id="4690a-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="4690a-109">Kliknięcie dowolnej grupy pokieruje Cię do listy Urządzenia przefiltrowane według twoich opcji.</span><span class="sxs-lookup"><span data-stu-id="4690a-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="4690a-110">Na liście Urządzenia możesz filtrować listę stanu kondycji według następującego stanu:</span><span class="sxs-lookup"><span data-stu-id="4690a-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="4690a-111">**Aktywny** Urządzenia, które aktywnie zgłaszają się do usługi Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="4690a-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="4690a-112">**Błędnie skonfigurowane** Urządzenia, które mogą częściowo raportować dane czujnika do usługi Defender for Endpoint, ale mają błędy konfiguracji, które trzeba poprawić.</span><span class="sxs-lookup"><span data-stu-id="4690a-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="4690a-113">Błędnie skonfigurowane urządzenia mogą mieć jeden lub połączenie następujących problemów:</span><span class="sxs-lookup"><span data-stu-id="4690a-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="4690a-114">Brak danych czujnika — urządzenia przestały wysyłać dane czujnika.</span><span class="sxs-lookup"><span data-stu-id="4690a-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="4690a-115">Z urządzenia można wyzwolić ograniczone alerty.</span><span class="sxs-lookup"><span data-stu-id="4690a-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="4690a-116">Ograniczona komunikacja — możliwość komunikowania się z urządzeniem jest ograniczona.</span><span class="sxs-lookup"><span data-stu-id="4690a-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="4690a-117">Wysyłanie plików do dogłębnej analizy, blokowanie plików, odizolowanie urządzenia od sieci i inne akcje, które wymagają komunikacji z urządzeniem, mogą nie działać.</span><span class="sxs-lookup"><span data-stu-id="4690a-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="4690a-118">**Nieaktywny** Urządzenia, które przestały zgłaszać się do usługi Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="4690a-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="4690a-119">Za pomocą funkcji Eksportowanie możesz pobrać całą listę w formacie CSV.</span><span class="sxs-lookup"><span data-stu-id="4690a-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="4690a-120">Aby uzyskać więcej informacji, [zobacz Sprawdzanie stanu kondycji czujnika w programie Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="4690a-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="4690a-121">Aby uzyskać więcej informacji o tym, co spowodowało, że urządzenie było nieaktywne lub nieprawidłowo skonfigurowane, zobacz Naprawianie czujniki o złej kondycji w programie [Microsoft Defender for Endpoint.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="4690a-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
