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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313509"
---
# <a name="find-events-performed-on-inbox-rules"></a>Znajdowanie zdarzeń wykonanych w zasadach skrzynki odbiorczej

Podczas tworzenia, zmieniania lub usuwania reguł skrzynki odbiorczej zdarzenia są rejestrowane w dzienniku inspekcji. Oto jak je przejrzeć:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

    **Uwaga:** Jeśli zobaczysz powiadomienie, że musisz włączyć inspekcję, przejdź dalej i włącz ją teraz. Jeśli ta funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.
1. Wybierz pole Działania i znajdź Exchange skrzynce pocztowej, a następnie wybierz pozycję New-InboxRule utwórz regułę skrzynki odbiorczej na Outlook Web App. Gdy to zrobisz, kliknij poza okienkiem, aby zminimalizować okienko Działania.
1. Określ zakres dat, a następnie w polu Użytkownicy wybierz nazwę użytkownika, którego chcesz zbadać. Możesz wybrać więcej niż jednego użytkownika na raz.
1. Wybierz pozycję Wyszukaj. Działania zostaną wyświetlone w obszarze Wyniki.
1. Aby wyświetlić szczegóły, wybierz działanie, a następnie wybierz pozycję Więcej informacji. W sekcji Parametry możesz zobaczyć nazwę reguły, zestawu warunków i akcji, które będą podejmowane przez regułę.

2. Na karcie **Wyszukiwanie** na stronie **Inspekcja** skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Wybierz pozycję **Nowa skrzynka odbiorczaZamów utwórz regułę skrzynki odbiorczej na Outlook Web App**

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły. W sekcji **Parametry** możesz zobaczyć nazwę reguły, zestawu warunków i akcji, które będą podejmowane przez regułę.

Aby dowiedzieć się więcej, zobacz [Przeszukiwanie dziennika inspekcji w celu zbadania typowych problemów z obsługą.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
