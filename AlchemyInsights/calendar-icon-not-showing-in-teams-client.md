---
title: Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819963"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="0b94d-102">Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams</span><span class="sxs-lookup"><span data-stu-id="0b94d-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="0b94d-103">Karta kalendarz w usłudze Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b94d-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="0b94d-104">Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna.</span><span class="sxs-lookup"><span data-stu-id="0b94d-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="0b94d-105">W przypadku użytkowników online, którzy nie widzą karty Kalendarz, upewnij się, że [mają oni licencję dla skrzynek pocztowych usługi Exchange Online i że skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="0b94d-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="0b94d-106">Jeśli użytkownik ma prawidłową skrzynkę pocztową w usłudze Exchange Online, ale nadal nie widzi karty Kalendarz, być może wystąpił problem z siecią.</span><span class="sxs-lookup"><span data-stu-id="0b94d-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="0b94d-107">Użyj programu [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) i uruchom **testy łączności usług Microsoft Exchange Web Services** dla użytkownika, którego to dotyczy.</span><span class="sxs-lookup"><span data-stu-id="0b94d-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="0b94d-108">Na koniec sprawdź [aplikacje usługi Teams — zasady konfiguracji aplikacji](https://admin.teams.microsoft.com/policies/app-setup), aby upewnić się, że aplikacja kalendarza nie została usunięta z zasad stosowanych dla użytkownika (najprawdopodobniej **Globalne (domyślne dla całej organizacji)**.</span><span class="sxs-lookup"><span data-stu-id="0b94d-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="0b94d-109">Jeśli użytkownicy są objęci usługą lokalną, musisz potwierdzić, że konfiguracja środowiska hybrydowego jest w dobrej kondycji.</span><span class="sxs-lookup"><span data-stu-id="0b94d-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="0b94d-110">Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="0b94d-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="0b94d-111">Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="0b94d-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
