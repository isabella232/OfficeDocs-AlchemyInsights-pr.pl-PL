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
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendarza nie jest wyświetlana w kliencie aplikacji Microsoft Teams

Karta **Kalendarz** w aplikacji Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange. Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna. W przypadku użytkowników w trybie online, którzy nie widzą karty **Kalendarz** , upewnij się, że [są one licencjonowane dla skrzynki pocztowej usługi Exchange Online, a skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Jeśli użytkownicy mieszkają lokalnie, musisz potwierdzić, że konfiguracja hybrydowa jest zdrowy. Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Aby uzyskać więcej informacji i kroków rozwiązywania problemów, zobacz [Rozwiązywanie problemów ze interakcją Microsoft Teams i Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
