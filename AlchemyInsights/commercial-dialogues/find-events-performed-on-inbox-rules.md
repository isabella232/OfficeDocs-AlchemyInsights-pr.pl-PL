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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882645"
---
# <a name="find-events-performed-on-inbox-rules"></a>Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej

Podczas tworzenia, zmieniania lub usuwania reguł skrzynki odbiorczej zdarzenia są rejestrowane w dzienniku inspekcji. Oto jak je przejrzeć:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja**. Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, możesz włączyć ją teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.

2. Na karcie **Wyszukiwanie** na stronie **Inspekcja** skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Wybierz pozycję **Nowa skrzynka odbiorczaZarządzaj tworzenie reguły skrzynki odbiorczej na Outlook Web App**

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły. W sekcji **Parametry** możesz zobaczyć nazwę reguły, zestawu warunków i akcji, które będą podejmowane przez regułę.

Aby dowiedzieć się więcej, zobacz [Przeszukiwanie dziennika inspekcji w celu zbadania typowych problemów z obsługą.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
