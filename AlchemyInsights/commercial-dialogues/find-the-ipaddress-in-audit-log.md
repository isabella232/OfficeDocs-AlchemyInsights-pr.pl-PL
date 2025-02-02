---
title: Znajdowanie adresu IP w dzienniku inspekcji
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902270"
---
# <a name="find-the-ip-address-in-audit-log"></a>Znajdowanie adresu IP w dzienniku inspekcji

Adres IP odpowiadający działaniu wykonanemu przez użytkownika lub administratora jest wyświetlany w dziennikach inspekcji. Rejestrowane są również informacje o kliencie. Oto jak zidentyfikować adres IP:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja**. Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz włączyć ją teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.

2. Na stronie **Inspekcja** sprawdź, czy jest **zaznaczona** karta Wyszukiwanie, a następnie skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Jeśli interesuje Cię określone działanie, wybierz je z listy. w przeciwnym razie zostanie zwrócona wartość domyślna **Pokaż** wyniki dla wszystkich działań. Należy zauważyć, że niektóre działania mogą być niedostępne do wyboru. jednak te elementy inspekcji zostaną zwrócone, jeśli zaznaczono opcję Pokaż wyniki **dla wszystkich** działań.
   - **Użytkownicy:** zaakceptuj pustą wartość domyślną, aby zwrócić wyniki wszystkim użytkownikom, lub wprowadź co najmniej jednego użytkownika.

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. W wynikach kliknij pozycję **Filtruj wyniki** i wpisz **Set-Mailbox** w polu filtru aktywności.

5. Wybierz rekord inspekcji w wynikach, aby otworzyć **wysuwną pozycję** Szczegóły.

Aby uzyskać więcej informacji, zobacz [Przeszukiwanie dziennika inspekcji w celu zbadania typowych problemów z obsługą.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
