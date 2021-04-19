---
title: W portalu brakuje urządzeń programu Configuration Manager
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817254"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="fe532-102">W portalu brakuje urządzeń programu Configuration Manager</span><span class="sxs-lookup"><span data-stu-id="fe532-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="fe532-103">Aby mogła działać synchronizacja urządzeń, na serwerze lokalnym, który obsługuje rolę punktu połączenia usługi, muszą być dostępne [wymagane internetowe punkty końcowe](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints).</span><span class="sxs-lookup"><span data-stu-id="fe532-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="fe532-104">Aby rozwiązać problem z synchronizacją urządzeń, przejrzyj plik **CMGatewaySyncUploadWorker.log** znajdujący się w punkcie połączenia usługi.</span><span class="sxs-lookup"><span data-stu-id="fe532-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="fe532-105">Dowiedz się więcej o [dołączaniu dzierżawy w programie Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="fe532-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
