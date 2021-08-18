---
title: Ikona kalendarza nie jest wyświetlana w Microsoft Teams klienta
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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120014"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendarza nie jest wyświetlana w Microsoft Teams klienta

Karta **Kalendarz** w programie Teams wymaga dostępu do skrzynki Exchange pocztowej za pośrednictwem Exchange sieci Web. Skrzynka Exchange może być lokalna lub online. W przypadku użytkowników w  trybie online, którzy nie widzą karty Kalendarz, upewnij się, że mają oni licencje na skrzynkę pocztową usługi Exchange Online i [że skrzynka pocztowa jest włączona.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Jeśli Twoi użytkownicy znajdują się w środowisku lokalnym, musisz potwierdzić, że Konfiguracja hybrydowa jest w dobrej kondycji. Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Aby uzyskać więcej informacji i procedurę rozwiązywania problemów, zobacz [Rozwiązywanie Microsoft Teams i Exchange Server dotyczących interakcji.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
