---
title: Usuwanie danych i czyszczenie urządzeń w usłudze Intune
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416323"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="3c17b-102">Usuwanie danych i czyszczenie urządzeń w usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="3c17b-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="3c17b-103">Zdalne akcje Wycofywanie urządzenia i Czyszczenie urządzenia mogą być używane do usuwania danych firmowych zarządzanych przez usługę Intune lub do zresetowania urządzenia do ustawień fabrycznych i przywrócenia ustawień domyślnych.</span><span class="sxs-lookup"><span data-stu-id="3c17b-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="3c17b-104">Zaloguj się do usługi zarządzania urządzeniami na platformie Microsoft 365 i przejdź do opcji **Urządzenia** > **Wszystkie urządzenia**.</span><span class="sxs-lookup"><span data-stu-id="3c17b-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="3c17b-105">Wybierz urządzenie, które chcesz wyczyścić.</span><span class="sxs-lookup"><span data-stu-id="3c17b-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="3c17b-106">Wybierz wymagany typ zdalnego czyszczenia.</span><span class="sxs-lookup"><span data-stu-id="3c17b-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="3c17b-107">Opcja Wycofywanie usuwa tylko informacje o organizacji, podczas gdy pełne czyszczenie przywraca urządzenie do ustawień fabrycznych.</span><span class="sxs-lookup"><span data-stu-id="3c17b-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="3c17b-108">Wybierz pozycję **Tak**, aby potwierdzić.</span><span class="sxs-lookup"><span data-stu-id="3c17b-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="3c17b-109">Do czasu ukończenia czyszczenia status akcji urządzenia wyświetla się jako *Wycofywanie w toku*.</span><span class="sxs-lookup"><span data-stu-id="3c17b-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="3c17b-110">Po zakończeniu akcji nie zobaczysz urządzenia przenośnego na liście urządzenia zarządzanego. </span><span class="sxs-lookup"><span data-stu-id="3c17b-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="3c17b-111">Dane firmowe nie mogą zostać usunięte z urządzeń POŁĄCZONYCH z Microsoft Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c17b-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="3c17b-112">Aby uzyskać szczegółowe informacje na temat skutków akcji wycofywania i czyszczenia, w tym to, co zostało zachowane, a co usunięte, zobacz następującą dokumentację:</span><span class="sxs-lookup"><span data-stu-id="3c17b-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="3c17b-113">[Usuwanie urządzeń przy użyciu czyszczenia, wycofywania lub ręcznego wyrejestrowywania urządzenia](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="3c17b-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="3c17b-114">Jak czyścić z aplikacji usługi Intune tylko dane firmowe</span><span class="sxs-lookup"><span data-stu-id="3c17b-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="3c17b-115">[Usuwanie wszystkich danych z urządzenia z systemem macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="3c17b-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>