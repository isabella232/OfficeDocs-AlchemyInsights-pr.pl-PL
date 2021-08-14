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
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989601"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams

Karta kalendarz w usłudze Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange. Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna. W przypadku użytkowników online, którzy nie widzą karty Kalendarz, upewnij się, że [mają oni licencję dla skrzynek pocztowych usługi Exchange Online i że skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jeśli użytkownik ma prawidłową skrzynkę pocztową w usłudze Exchange Online, ale nadal nie widzi karty Kalendarz, być może wystąpił problem z siecią. Użyj programu [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) i uruchom **testy łączności usług Microsoft Exchange Web Services** dla użytkownika, którego to dotyczy.

Na koniec sprawdź [aplikacje usługi Teams — zasady konfiguracji aplikacji](https://admin.teams.microsoft.com/policies/app-setup), aby upewnić się, że aplikacja kalendarza nie została usunięta z zasad stosowanych dla użytkownika (najprawdopodobniej **Globalne (domyślne dla całej organizacji)**.

Jeśli użytkownicy są objęci usługą lokalną, musisz potwierdzić, że konfiguracja środowiska hybrydowego jest w dobrej kondycji. Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
