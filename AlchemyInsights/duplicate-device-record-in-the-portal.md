---
title: Zduplikowany rekord urządzenia w portalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790167"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="f6444-102">Zduplikowany rekord urządzenia w portalu</span><span class="sxs-lookup"><span data-stu-id="f6444-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="f6444-103">Jeśli urządzenie nie zgłosi prawidłowo stanu współzarządzania witrynie programu Configuration Manager, w portalu mogą być widoczne dwa rekordy dla tego samego urządzenia.</span><span class="sxs-lookup"><span data-stu-id="f6444-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="f6444-104">Stan współzarządzania urządzeniem możesz sprawdzić w kolumnie **Współzarządzane** dla urządzenia w konsoli programu Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f6444-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="f6444-105">Jeśli kolumna jest niewidoczna, możesz ją dodać, klikając prawym przyciskiem myszy dowolne nagłówki kolumn, a następnie wybierając ją z listy.</span><span class="sxs-lookup"><span data-stu-id="f6444-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="f6444-106">Kolumna Współzarządzane musi mieć wartość **Tak**.</span><span class="sxs-lookup"><span data-stu-id="f6444-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="f6444-107">Jeśli wartość to **Nie**, otwórz aplet klienta Configuration Manager na urządzeniu klienckim i sprawdź wartość **Współzarządzanie** na karcie Ogólne.</span><span class="sxs-lookup"><span data-stu-id="f6444-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="f6444-108">Jeśli wartość to **Włączone**, wskazuje to na problemy z komunikacją między klientem a punktem zarządzania.</span><span class="sxs-lookup"><span data-stu-id="f6444-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="f6444-109">Sprawdź plik **CcmMessaging.log** na urządzeniu pod kątem potencjalnych problemów z łącznością.</span><span class="sxs-lookup"><span data-stu-id="f6444-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="f6444-110">Jeśli wartość to **Wyłączone**, a urządzenie jest zarejestrowane w usłudze Intune, sprawdź plik **CoManagementHandler.log** na urządzeniu, aby upewnić się, że urządzenie otrzymało zasady współzarządzania.</span><span class="sxs-lookup"><span data-stu-id="f6444-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
