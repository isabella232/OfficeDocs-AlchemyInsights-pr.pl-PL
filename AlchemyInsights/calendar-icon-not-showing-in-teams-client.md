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
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendarza nie jest wyświetlana w kliencie usługi Teams

Karta kalendarz w usłudze Teams wymaga dostępu do skrzynki pocztowej programu Exchange za pośrednictwem usług sieci Web programu Exchange. Skrzynka pocztowa programu Exchange może być w trybie online lub lokalna. W przypadku użytkowników online, którzy nie widzą karty Kalendarz, upewnij się, że [mają oni licencję dla skrzynek pocztowych usługi Exchange Online i że skrzynka pocztowa jest włączona](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Jeśli użytkownik ma prawidłową skrzynkę pocztową w usłudze Exchange Online, ale nadal nie widzi karty Kalendarz, być może wystąpił problem z siecią. Użyj programu [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) i uruchom **testy łączności usług Microsoft Exchange Web Services** dla użytkownika, którego to dotyczy.

Na koniec sprawdź [aplikacje usługi Teams — zasady konfiguracji aplikacji](https://admin.teams.microsoft.com/policies/app-setup), aby upewnić się, że aplikacja kalendarza nie została usunięta z zasad stosowanych dla użytkownika (najprawdopodobniej **Globalne (domyślne dla całej organizacji)**.

Jeśli użytkownicy są objęci usługą lokalną, musisz potwierdzić, że konfiguracja środowiska hybrydowego jest w dobrej kondycji. Do rozwiązywania problemów użyj [Kreatora konfiguracji hybrydowej](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Zwróć uwagę, że [usługa Teams wymaga programu Exchange 2016 CU3 lub nowszego](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
