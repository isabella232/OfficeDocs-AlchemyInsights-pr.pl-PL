---
title: Blokowanie podpisów e-mail wykonanych przez użytkownika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243630"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="6b160-102">Blokowanie podpisów e-mail wykonanych przez użytkownika</span><span class="sxs-lookup"><span data-stu-id="6b160-102">Block user-made email signatures</span></span>

<span data-ttu-id="6b160-103">Poniższe rozwiązanie dotyczy tylko podpisów e-mail utworzonych w aplikacji Outlook w sieci Web.</span><span class="sxs-lookup"><span data-stu-id="6b160-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="6b160-104">Podpisy można blokować tylko w aplikacji Outlook, jeśli masz aplikację lokalną Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="6b160-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="6b160-105">W centrum administracyjnym wybierz pozycję **Centra administracyjne programu**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="6b160-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="6b160-106">Kliknij **uprawnienia zasady** aplikacji Outlook Web  >  **App.**</span><span class="sxs-lookup"><span data-stu-id="6b160-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="6b160-107">Wybierz zasady, a następnie kliknij ikonę ołówka, aby je edytować.</span><span class="sxs-lookup"><span data-stu-id="6b160-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="6b160-108">Kliknij **pozycję Więcej**  >  **opcji.**</span><span class="sxs-lookup"><span data-stu-id="6b160-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="6b160-109">W **obszarze Środowisko użytkownika** wyczyść pole wyboru Podpis e-mail, a następnie kliknij przycisk **Zapisz.** </span><span class="sxs-lookup"><span data-stu-id="6b160-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="6b160-110">**Ważne:** Jeśli przed wyczyszczeniem tego pola wyboru dodano podpis, użytkownik nadal będzie mógł go używać.</span><span class="sxs-lookup"><span data-stu-id="6b160-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="6b160-111">Poproś ją o jej usunięcie.</span><span class="sxs-lookup"><span data-stu-id="6b160-111">Ask them to remove it.</span></span>
