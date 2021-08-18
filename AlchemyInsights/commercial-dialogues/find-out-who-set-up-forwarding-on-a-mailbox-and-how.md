---
title: Dowiedz się, kto s skonfigurować przesyłanie dalej w skrzynce pocztowej i jak to zrobić
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317818"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Dowiedz się, kto s skonfigurować przesyłanie dalej w skrzynce pocztowej i jak to zrobić

Jeśli dla skrzynki pocztowej ustawiono przesyłanie dalej zewnętrzne, działanie jest przekazywane w ramach polecenia cmdlet **Set-Mailbox.** Aby znaleźć działanie w dzienniku inspekcji:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

   **Uwaga:** Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, przejdź dalej i włącz ją teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.

2. Na stronie **Inspekcja** sprawdź, czy jest **zaznaczona** karta Wyszukiwanie, a następnie skonfiguruj następujące ustawienia:
   - Zaznacz zakres dat i godzin w **polach Rozpoczęcie** **i** Koniec.
   - Sprawdź, **czy pole Działania** zawiera pole Pokaż wyniki dla wszystkich **działań.**

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. W wynikach kliknij **kolumnę** Działanie, aby posortować wyniki, a następnie odszukaj pozycje **Set-Mailbox.**

5. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły. Aby ustalić, czy dane działanie jest związane z przesyłaniem dalej poczty e-mail, należy przyjrzeć się szczegółom każdego rekordu inspekcji:
   - **ObjectId:** wartość aliasu zmodyfikowanej skrzynki pocztowej.
   - **Parametry:** _ForwardingSmtpAddress_ wskazuje docelowy adres e-mail.
   - **UserId**: Użytkownik, który skonfigurował przesyłanie dalej poczty e-mail w skrzynce pocztowej w polu **ObjectId.**

Aby uzyskać więcej informacji, zobacz Określanie, kto s skonfigurować [przesyłanie dalej poczty e-mail dla skrzynki pocztowej.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
