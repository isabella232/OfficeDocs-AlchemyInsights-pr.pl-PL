---
title: Dowiedz się, kto i jak skonfigurować przesyłanie dalej w skrzynce pocztowej
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429990"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Dowiedz się, kto i jak skonfigurować przesyłanie dalej w skrzynce pocztowej

Jeśli w skrzynce pocztowej ustawiono zewnętrzne przesyłanie dalej, to działanie jest raportowane w Set-Mailbox cmdlet. Poniżej opisano, jak można znaleźć działanie w dzienniku inspekcji:

1. Przejdź do Centrum [zabezpieczeń usługi Office 365 & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wybierz **pozycję** >  **Przeszukiwanie dziennika inspekcji.**
    > [!NOTE]
    > Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz ją włączyć już teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły wyciągać danych z poprzednich dat.
1. Upewnij się, **że pole Działania** ma ustawioną wartość Pokaż wyniki dla wszystkich **działań** (ustawienie domyślne). Określ zakres dat. Nie musisz określać nazwy użytkownika.
1. Wybierz **pozycję Wyszukaj.** Działania zostaną wyświetlone w obszarze **Wyniki.**
1. Wybierz **pozycję Filtruj** wyniki, a następnie **wprowadź pole Ustaw skrzynkę** pocztową w **polu** Filtr aktywności. W ten sposób są **zwracane wszystkie działania typu Set-Mailbox.**
1. Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz **pozycję Więcej informacji.** W **obszarze** Parametry możesz zobaczyć adres e-mail przesyłania dalej ustawiony w skrzynce pocztowej. Identyfikator **użytkownika reprezentuje** użytkownika, który schowa zewnętrzne przesyłanie dalej w skrzynce pocztowej.
Aby dowiedzieć się więcej, zobacz Przeszukiwanie dziennika inspekcji usługi [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)w celu rozwiązania typowych scenariuszy.