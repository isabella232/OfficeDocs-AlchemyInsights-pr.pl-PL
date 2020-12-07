---
title: Ikona kalendarza nie jest wyświetlana w kliencie aplikacji Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583922"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="796d9-102">Ikona kalendarza nie jest wyświetlana w kliencie aplikacji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="796d9-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="796d9-103">Karta **Kalendarz** w aplikacji Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange.</span><span class="sxs-lookup"><span data-stu-id="796d9-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="796d9-104">Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna.</span><span class="sxs-lookup"><span data-stu-id="796d9-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="796d9-105">W przypadku użytkowników w trybie online, którzy nie widzą karty **Kalendarz** , upewnij się, że [są one licencjonowane dla skrzynki pocztowej usługi Exchange Online, a skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="796d9-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="796d9-106">Jeśli użytkownicy mieszkają lokalnie, musisz potwierdzić, że konfiguracja hybrydowa jest zdrowy.</span><span class="sxs-lookup"><span data-stu-id="796d9-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="796d9-107">Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="796d9-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="796d9-108">Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="796d9-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="796d9-109">Aby uzyskać więcej informacji i kroków rozwiązywania problemów, zobacz [Rozwiązywanie problemów ze interakcją Microsoft Teams i Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="796d9-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
