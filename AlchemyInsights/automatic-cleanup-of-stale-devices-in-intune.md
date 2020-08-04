---
title: Automatyczne oczyszczanie starych urządzeń w usłudze Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555226"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="d4585-102">Automatyczne oczyszczanie starych urządzeń w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="d4585-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="d4585-103">Usługa Intune umożliwia administratorowi skonfigurowanie przedziału czasu między 90 a 270 dniami, po czym przestarzałe urządzenia są usuwane z usługi.</span><span class="sxs-lookup"><span data-stu-id="d4585-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="d4585-104">To ustawienie jest w całej organizacji i po aktywacji wchodzi w życie natychmiast.</span><span class="sxs-lookup"><span data-stu-id="d4585-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="d4585-105">Wszystkie urządzenia niezaewidencjonowane na serwerze usługi Intune przez okres przekraczający to ustawienie są trwale usuwane.</span><span class="sxs-lookup"><span data-stu-id="d4585-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="d4585-106">**Uwaga** Tylko obiekty urządzenia MDM kwalifikują się do tej akcji oczyszczania.</span><span class="sxs-lookup"><span data-stu-id="d4585-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="d4585-107">Obiekty urządzenia EAS są wykluczone.</span><span class="sxs-lookup"><span data-stu-id="d4585-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="d4585-108">Aby uzyskać dodatkowe informacje o tym, kiedy urządzenie kwalifikuje się do usunięcia na podstawie ustawienia oczyszczania urządzenia i jego "stanu":</span><span class="sxs-lookup"><span data-stu-id="d4585-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="d4585-109">Ustawienie: **Usuwanie urządzeń po ostatniej dacie ewidencjonowania: Tak (określona wartość (N) w określonych dniach)**</span><span class="sxs-lookup"><span data-stu-id="d4585-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="d4585-110">Na podstawie wartości (N) skonfigurowanych w ustawieniu usługa Intune usuwa urządzenie w określonych dniach po jego ostatnim pomyślnym zaewidencjonowania.</span><span class="sxs-lookup"><span data-stu-id="d4585-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="d4585-111">Ustawienie: **Usuwanie urządzeń po ostatniej dacie zameldowania: Nie**</span><span class="sxs-lookup"><span data-stu-id="d4585-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="d4585-112">180 dni po wygaśnięciu certyfikatu urządzenia i nie odnowieniu urządzenie zostanie usunięte.</span><span class="sxs-lookup"><span data-stu-id="d4585-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="d4585-113">**Uwaga** W obu przypadkach urządzenie musi zostać pomyślnie zarejestrowane w usłudze Intune.</span><span class="sxs-lookup"><span data-stu-id="d4585-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="d4585-114">Rejestracja odbywa się podczas pierwszego zaewidencjonowania urządzenia za pomocą usługi Intune.</span><span class="sxs-lookup"><span data-stu-id="d4585-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="d4585-115">Jeśli urządzenie pomyślnie zarejestruje się w usłudze Intune, ale nie zostanie zarejestrowane w usłudze Intune, urządzenie zostanie usunięte 270 dni po rejestracji.</span><span class="sxs-lookup"><span data-stu-id="d4585-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="d4585-116">(90 dni, aby oznaczyć urządzenie jako odwołane, a następnie kolejne 180 dni na usunięcie rekordu).</span><span class="sxs-lookup"><span data-stu-id="d4585-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="d4585-117">Obecnie w konsoli usługi Intune nie istnieje mechanizm służący do określania daty wygaśnięcia certyfikacji urządzenia dla danego urządzenia.</span><span class="sxs-lookup"><span data-stu-id="d4585-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>