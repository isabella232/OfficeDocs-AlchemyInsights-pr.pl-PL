---
title: 'Rozwiązywanie problemów poczty głosowej '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679099"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="7951f-102">Rozwiązywanie problemów poczty głosowej</span><span class="sxs-lookup"><span data-stu-id="7951f-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="7951f-103">Upewnij się, że funkcja zajęta w trakcie zajętości jest zamierzona.</span><span class="sxs-lookup"><span data-stu-id="7951f-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="7951f-104">Jeśli ta funkcja nie jest potrzebna dla tego użytkownika:</span><span class="sxs-lookup"><span data-stu-id="7951f-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="7951f-105">Przejdź do [Centrum administracyjnego aplikacji Teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="7951f-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="7951f-106">W obszarze lewy kolejno poruszanie się po kolei zasady  >    >  **zarządzania** zasadami dotyczącymi **połączeń** głosowych.</span><span class="sxs-lookup"><span data-stu-id="7951f-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="7951f-107">Wybierz pozycję **Zarządzaj użytkownikami**.</span><span class="sxs-lookup"><span data-stu-id="7951f-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="7951f-108">Wyszukaj użytkownika i Zmień zasady połączeń na takie, które są **zajęte w czasie zajętym, są dostępne, gdy połączenie jest** **wyłączone**.</span><span class="sxs-lookup"><span data-stu-id="7951f-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="7951f-109">Kliknij przycisk **Zastosuj**.</span><span class="sxs-lookup"><span data-stu-id="7951f-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="7951f-110">Replikowanie zmian zasad może potrwać do 24 godzin.</span><span class="sxs-lookup"><span data-stu-id="7951f-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="7951f-111">Aby uzyskać więcej informacji na temat tej funkcji, zobacz: [zajęty na zajętym czasie jest dostępna podczas rozmowy](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="7951f-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
