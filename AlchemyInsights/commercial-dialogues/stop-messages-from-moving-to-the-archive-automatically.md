---
title: Automatyczne zatrzymywanie przenoszenia wiadomości do archiwum
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749825"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="4c4aa-102">Automatyczne zatrzymywanie przenoszenia wiadomości do archiwum</span><span class="sxs-lookup"><span data-stu-id="4c4aa-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="4c4aa-103">Jeśli korzystasz z zasad przechowywania, możesz zmienić wiek przechowywania w tych zasadach, aby zatrzymać automatyczne archiwizowanie wiadomości.</span><span class="sxs-lookup"><span data-stu-id="4c4aa-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="4c4aa-104">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="4c4aa-104">Here's how:</span></span>

1. <span data-ttu-id="4c4aa-105">W centrum [administracyjnym programu Exchange](https://go.microsoft.com/fwlink/?linkid=2059104)wybierz tagi przechowywania **zarządzania**  >  **zgodnością**.</span><span class="sxs-lookup"><span data-stu-id="4c4aa-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="4c4aa-106">Znajdź tag przechowywania Przenieś do archiwum.</span><span class="sxs-lookup"><span data-stu-id="4c4aa-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="4c4aa-107">W tagu przechowywania zmień okres przechowywania (okres archiwizacji) na Nigdy, aby zatrzymać automatyczne archiwizowanie elementów przez zasady przechowywania. </span><span class="sxs-lookup"><span data-stu-id="4c4aa-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="4c4aa-108">Spowoduje to zmianę ustawienia archiwizacji dla wszystkich skrzynek pocztowych, do których zastosowano ten tag przechowywania.</span><span class="sxs-lookup"><span data-stu-id="4c4aa-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
