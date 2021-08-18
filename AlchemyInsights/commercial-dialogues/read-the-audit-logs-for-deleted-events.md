---
title: Odczytywanie dzienników inspekcji usuniętych zdarzeń
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324743"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Odczytywanie dzienników inspekcji usuniętych zdarzeń

Poniżej opisano, jak to zrobić:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

    **Uwaga:** Jeśli zobaczysz powiadomienie, że musisz włączyć tę funkcję, możesz ją włączyć już teraz. Jeśli funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.

2. Na karcie **Wyszukiwanie** na stronie **Inspekcja** skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Wprowadź **Exchange skrzynce pocztowej,** a następnie wybierz następujące wartości:
     - **Usunięte wiadomości z folderu Elementy usunięte**
     - **Przeniesiono wiadomości do folderu Elementy usunięte**

       Gdy to zrobisz, kliknij poza okienkiem, aby zminimalizować **okienko** Działania.

   - **Użytkownicy:** zaakceptuj pustą wartość domyślną, aby zwrócić wyniki wszystkim użytkownikom, lub wprowadź co najmniej jednego użytkownika.

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły. W polu **Elementy** objęte problemem są wyświetlane dodatkowe informacje dotyczące usuniętego elementu, takie jak wiersz tematu i lokalizacja usuniętego elementu.

   **Uwaga:** Za pomocą funkcji dziennika inspekcji nie można przywrócić usuniętych elementów. Aby przywrócić usunięte elementy, zobacz [Odzyskiwanie usuniętych wiadomości e-mail w programie Outlook w sieci Web.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Aby uzyskać więcej informacji, zobacz [Przeszukiwanie dziennika inspekcji w celu zbadania typowych problemów z obsługą.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
