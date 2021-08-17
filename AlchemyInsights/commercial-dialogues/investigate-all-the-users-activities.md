---
title: Badanie działań wszystkich użytkowników
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898806"
---
# <a name="investigate-all-the-users-activities"></a>Badanie działań wszystkich użytkowników

Poniżej opisano, jak to zrobić:

1. Wykonaj jedną z następujących czynności:
   - Na stronie Centrum zgodności platformy Microsoft 365 <https://compliance.microsoft.com> przejdź do **tematu Inspekcja** \> **rozwiązań.** Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://compliance.microsoft.com/auditlogsearch> .
   - W portalu Microsoft 365 Defender w <https://security.microsoft.com> witrynie przejdź do tematu **Inspekcja**. Aby przejść bezpośrednio do strony **Inspekcja,** użyj <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Jeśli zauważysz, że musisz włączyć tę funkcję, możesz ją włączyć już teraz. Jeśli funkcja nie jest włączona, wyniki wyszukiwania nie będą mogły ściągać danych z poprzednich dat.

2. Na karcie **Wyszukiwanie** na stronie **Inspekcja** skonfiguruj następujące ustawienia:
   - **Zakres dat i godzin:** Zaznacz zakres dat i godzin w polach **Rozpoczęcie** **i** Zakończenie.
   - **Działania:** Jeśli interesuje Cię określone działanie, wybierz je z listy. w przeciwnym razie wartość domyślna **Pokaż wyniki dla wszystkich działań** zwraca wszystkie działania.
   - **Użytkownicy:** zaakceptuj pustą wartość domyślną, aby zwrócić wyniki wszystkim użytkownikom, lub wprowadź co najmniej jednego użytkownika.

3. Po zakończeniu kliknij pozycję **Wyszukaj**. Działania zostaną wyświetlone na nowej **stronie Przeszukiwanie** inspekcji. Zostanie wyświetlony adres **IP**, **nazwa** użytkownika i **działania.**

4. Aby pobrać wyniki, wybierz pozycję **Eksportuj** \> **pobierz wszystkie wyniki.**

5. Wybierz działanie w wynikach, aby otworzyć wysuwne szczegóły.

Aby dowiedzieć się więcej, zobacz [Przeszukiwanie dziennika inspekcji w celu zbadania typowych problemów z obsługą.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
