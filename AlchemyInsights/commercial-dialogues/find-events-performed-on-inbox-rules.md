---
title: Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482602"
---
# <a name="find-events-performed-on-inbox-rules"></a>Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej

Podczas tworzenia, zmieniania lub usuwania reguł skrzynki odbiorczej zdarzenia są rejestrowane w dzienniku inspekcji. Oto jak je przejrzeć:

1. Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wybierz pozycję Wyszukiwanie > przeszukiwanie dziennika inspekcji.

    > [!NOTE]
    > Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz ją włączyć już teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.
1. Wybierz pole Działania i znajdź działania skrzynki pocztowej programu Exchange, a następnie wybierz pozycję New-InboxRule Utwórz regułę skrzynki odbiorczej w aplikacji Outlook Web App. Gdy to zrobisz, kliknij poza okienkiem, aby zminimalizować okienko Działania.
1. Określ zakres dat, a następnie w polu Użytkownicy wybierz nazwę użytkownika, którego chcesz zbadać. Możesz wybrać więcej niż jednego użytkownika na raz.
1. Wybierz pozycję Wyszukaj. Działania zostaną wyświetlone w obszarze Wyniki.
1. Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz pozycję Więcej informacji. W sekcji Parametry możesz zobaczyć nazwę reguły, zestaw warunków i akcje, które będą podejmowane przez regułę.

Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi Office 365 w celu rozwiązania typowych scenariuszy.