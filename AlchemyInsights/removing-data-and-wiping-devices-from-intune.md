---
title: Usuwanie danych i wycieranie urządzeń z usługi Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440471"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="f0868-102">Usuwanie danych i wycieranie urządzeń z usługi Intune</span><span class="sxs-lookup"><span data-stu-id="f0868-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="f0868-103">Akcje zdalne Dotyczące wycofywania urządzeń i czyszczenia urządzenia mogą służyć do usuwania danych firmowych zarządzanych przez usługę Intune lub do przywracania ustawień fabrycznych i przywracania ustawień domyślnych urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f0868-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="f0868-104">Zaloguj się do zarządzania urządzeniami w usłudze Microsoft 365 i przejdź do **urządzenia**  >  **Wszystkie urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="f0868-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="f0868-105">Wybierz urządzenie, które chcesz wyczyścić.</span><span class="sxs-lookup"><span data-stu-id="f0868-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="f0868-106">Wybierz typ zdalnego czyszczenia, które chcesz wykonać.</span><span class="sxs-lookup"><span data-stu-id="f0868-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="f0868-107">Wycofanie powoduje usunięcie tylko informacji organizacji, a pełne czyszczenie przywraca urządzenie do ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="f0868-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="f0868-108">Wybierz **pozycję Tak,** aby potwierdzić.</span><span class="sxs-lookup"><span data-stu-id="f0868-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="f0868-109">Dopóki czyszczenie nie zostanie wykończęce, stan akcji Urządzenie jest wyświetlany jako Oczekujące na wycofanie.</span><span class="sxs-lookup"><span data-stu-id="f0868-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="f0868-110">Po zakończeniu akcji urządzenie przenośne nie będzie już widoczne na liście zarządzanych urządzeń.</span><span class="sxs-lookup"><span data-stu-id="f0868-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="f0868-111">**Uwaga** Nie można usunąć danych firmy z urządzeń przyłączonych do usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f0868-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="f0868-112">Aby uzyskać szczegółowe informacje na temat efektu akcji Wycofywanie i czyszczenie, w tym tego, co jest zachowywane i co jest usuwane, zobacz [Usuwanie urządzeń za pomocą czyszczenia, wycofywania lub ręcznego wyrejestrowywania urządzenia](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="f0868-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="f0868-113">Aby wymazać wszystkie dane z urządzenia z systemem macOS, zobacz [Wymazywanie wszystkich danych z urządzenia z systemem macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="f0868-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>