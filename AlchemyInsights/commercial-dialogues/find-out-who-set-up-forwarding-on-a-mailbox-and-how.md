---
title: Dowiedz się, kto s skonfigurować przesyłanie dalej w skrzynce pocztowej, i jak to zrobić
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988216"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Dowiedz się, kto s skonfigurować przesyłanie dalej w skrzynce pocztowej, i jak to zrobić

Jeśli dla skrzynki pocztowej ustawiono zewnętrzne przesyłanie dalej, to działanie jest podlega inspekcji w ramach polecenia cmdlet Set-Mailbox cmdlet. Aby znaleźć działanie w dzienniku inspekcji:

1. Przejdź do centrum [Office 365 zabezpieczeń & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Wybierz **pozycję** >  **Przeszukiwanie dziennika inspekcji wyszukiwania**.
    > [!NOTE]
    > Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz włączyć ją teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.
1. Upewnij się, **że pole Działania** ma ustawioną wartość Pokaż wyniki dla wszystkich **działań** (ustawienie domyślne). Określ zakres dat. Nie musisz określać nazwy użytkownika.
1. Wybierz **pozycję Wyszukaj**. Działania zostaną wyświetlone w obszarze **Wyniki**.
1. Wybierz **pozycję Filtruj** wyniki , a następnie **wprowadź set-mailbox** w polu **filtru** Działanie. Zwraca wszystkie działania **set-mailbox.**
1. Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz **pozycję Więcej informacji.** W **obszarze** Parametry możesz zobaczyć adres e-mail przesyłania dalej ustawiony w skrzynce pocztowej. Identyfikator **użytkownika to** użytkownik, który schowyzda zewnętrzną usługę przesyłania dalej w skrzynce pocztowej.
Aby dowiedzieć się więcej, zobacz [Przeszukiwanie dziennika Office 365 w celu rozwiązania typowych scenariuszy.](https://go.microsoft.com/fwlink/?linkid=2103944)