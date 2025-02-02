---
title: Identyfikowanie działań reguł skrzynki odbiorczej w dziennikach inspekcji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331133"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identyfikowanie działań reguł skrzynki odbiorczej w dziennikach inspekcji

Zdarzenia reguł skrzynki odbiorczej (tworzenie, modyfikowanie i usuwanie reguł skrzynki odbiorczej) można Centrum zgodności platformy Microsoft 365 za pomocą przeszukiwania dziennika inspekcji.

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

2. Na karcie **Wyszukiwanie** na stronie **Inspekcja** skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Wybierz co najmniej jedną z następujących wartości:
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Aktualizowanie reguł skrzynki odbiorczej z Outlook klienta**

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji.

4. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły. Informacje o ustawieniach reguły skrzynki odbiorczej są wyświetlane w polu **Parametry.**

Aby uzyskać więcej informacji, zobacz [Ustalanie, czy użytkownik utworzył regułę skrzynki odbiorczej.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
