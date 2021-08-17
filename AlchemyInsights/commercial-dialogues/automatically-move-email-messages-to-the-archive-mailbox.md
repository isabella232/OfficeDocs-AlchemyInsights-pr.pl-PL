---
title: Automatyczne przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 57dbfd116bbae227f2288ce23edeaaa833fadf54ca3b10b95c49512758542e32
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059236"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automatyczne przenoszenie wiadomości e-mail do archiwaowej skrzynki pocztowej

Oto jak skonfigurować zasady automatycznego przenoszenia starych wiadomości e-mail użytkownika do archiwaowej skrzynki pocztowej:

1. Przejdź do [**tematu & zarządzania**](https://go.microsoft.com/fwlink/p/?linkid=2077143)danymi zgodności, aby sprawdzić, czy dla użytkownika włączono archiwacyjną  >    >   skrzynkę pocztową. Jeśli tak nie jest, kliknij pozycję **Włącz,** a **następnie tak w** polu ostrzeżenia.
2. Przejdź do [**Exchange administracyjnego i > zarządzania zgodnością > tagami przechowywania**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Wybierz ikonę +, a następnie **wybierz pozycję automatycznie zastosuj do całej skrzynki pocztowej.**
4. Przypisz nazwę do tagu przechowywania i wybierz pozycję **Przenieś do archiwum.** W okresie przechowywania wprowadź czas, na przykład 90 dni. Kliknij **Zapisz**.
5. Teraz utwórz zasady przechowywania: wybierz **zasady przechowywania**, wybierz ikonę, aby dodać nowe zasady.
6. Przypisz nazwę do zasad przechowywania, a następnie kliknij i przewiń listę, aby znaleźć i dodać właśnie utworzony tag przechowywania. Kliknij **Zapisz**.
7. Na koniec zastosuj zasady przechowywania do skrzynki pocztowej użytkownika: nadal w centrum administracyjnym Exchange przejdź do **skrzynek** pocztowych  >  **adresatów.** Wybierz wszystkich użytkowników, do których chcesz zastosować zasady, a następnie wybierz pozycję **Edytuj** (ikona ołówka).
8. W oknie dialogowym kliknij pozycję **funkcje skrzynki pocztowej**. W **obszarze Zasady** przechowywania zastosuj zasady, które właśnie zostały > **Zapisz.**
9. Aby uzyskać instrukcje dotyczące stosowania zasad do wszystkich użytkowników, zobacz Stosowanie zasad przechowywania [do skrzynek pocztowych.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
