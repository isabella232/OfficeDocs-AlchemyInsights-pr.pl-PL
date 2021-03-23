---
title: Blokowanie użytkownikom nagrywania spotkań
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035985"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="02d6b-102">Blokowanie użytkownikom nagrywania spotkań</span><span class="sxs-lookup"><span data-stu-id="02d6b-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="02d6b-103">Jeśli chcesz uniemożliwić **określonym** użytkownikom nagrywanie spotkań w aplikacji Teams lub zablokować im możliwość ich nagrywania, możesz to zrobić za pomocą ustawień zasad spotkania w aplikacji Teams.</span><span class="sxs-lookup"><span data-stu-id="02d6b-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="02d6b-104">W centrum administracyjnym usługi Microsoft Teams wyłącz ustawienie Zezwalaj na **nagrywanie** w chmurze w zasadach spotkania przypisanych do tego użytkownika.</span><span class="sxs-lookup"><span data-stu-id="02d6b-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="02d6b-105">Aby dowiedzieć się więcej, zobacz [Zarządzanie zasadami spotkań w aplikacji Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="02d6b-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="02d6b-106">Aby sprawdzić, czy określony użytkownik może nagrywać spotkania w aplikacji Teams, skorzystaj z diagnostyki technicznej.</span><span class="sxs-lookup"><span data-stu-id="02d6b-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="02d6b-107">Uruchom nowe zapytanie pomocy technicznej i wpisz **Diag: Nagrywanie** spotkania — diagnostyka sprawdzi ustawienia zasad dla określonego użytkownika i określi jego ustawienia zasad.</span><span class="sxs-lookup"><span data-stu-id="02d6b-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="02d6b-108">Pamiętaj, że nowe ustawienia zasad mogą zostać wprowadzone po kilku godzinach, więc jeśli zmiany zostały właśnie wprowadzone, poczekaj kilka godzin, zanim ponownie zostanie uruchomione narzędzie diagnostyczne.</span><span class="sxs-lookup"><span data-stu-id="02d6b-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="02d6b-109">Aby uzyskać więcej informacji, zapoznaj się z tematem Włączanie [lub wyłączanie nagrywania w chmurze.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="02d6b-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
