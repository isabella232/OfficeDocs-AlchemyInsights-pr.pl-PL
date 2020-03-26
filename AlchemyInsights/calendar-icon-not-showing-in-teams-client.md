---
title: Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932199"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="62534-102">Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams</span><span class="sxs-lookup"><span data-stu-id="62534-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="62534-103">Karta kalendarz w usłudze Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="62534-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="62534-104">Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna.</span><span class="sxs-lookup"><span data-stu-id="62534-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="62534-105">W przypadku użytkowników online, którzy nie widzą karty Kalendarz, upewnij się, że [mają oni licencję dla skrzynek pocztowych usługi Exchange Online i że skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="62534-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="62534-106">Jeśli użytkownik ma prawidłową skrzynkę pocztową w usłudze Exchange Online, ale nadal nie widzi karty Kalendarz, być może wystąpił problem z siecią.</span><span class="sxs-lookup"><span data-stu-id="62534-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="62534-107">Użyj programu [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) i uruchom **testy łączności usług Microsoft Exchange Web Services** dla użytkownika, którego to dotyczy.</span><span class="sxs-lookup"><span data-stu-id="62534-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="62534-108">Na koniec sprawdź [aplikacje usługi Teams — zasady konfiguracji aplikacji](https://admin.teams.microsoft.com/policies/app-setup), aby upewnić się, że aplikacja kalendarza nie została usunięta z zasad stosowanych dla użytkownika (najprawdopodobniej **Globalne (domyślne dla całej organizacji)**.</span><span class="sxs-lookup"><span data-stu-id="62534-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="62534-109">Jeśli użytkownicy są objęci usługą lokalną, musisz potwierdzić, że konfiguracja środowiska hybrydowego jest w dobrej kondycji.</span><span class="sxs-lookup"><span data-stu-id="62534-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="62534-110">Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="62534-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="62534-111">Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="62534-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
