---
title: Monitorowanie dostępu warunkowego
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708684"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorowanie dostępu warunkowego dla programu Exchange

Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełniają wymagań dotyczących dostępu do organizacji. Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:

- Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji Portal firmy i sprawdź, czy jest ono widoczne w portalu firmy. Jeśli tak się nie stanie, użytkownik powinien zarejestrować urządzenie.
- W portalu Azure przejdź do usługi Intune > zgodności urządzenia. W obszarze Monitorowanie kliknij pozycję Zgodność urządzenia. Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest zgodne.
- W portalu Azure przejdź do usługi Intune > zgodności urządzenia. W obszarze Zarządzanie kliknij pozycję Zasady. Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli nie przypisano żadnego profilu, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.
- Edytuj przypisanie dostępu warunkowego użytkownika.

1. W portalu Azure przejdź do zasad **dostępu**  >    >  **warunkowego usługi Intune.**
2. Wybierz zasady z listy.
3. Kliknij pozycję Użytkownicy i grupy.
4. Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do listy Uwzględnij. Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do listy Wyklucz.

Przydatne linki:

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów z urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorowanie zgodności urządzenia w usłudze Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Uwaga: te kroki są pomocne tylko podczas rozwiązywania problemów z dostępem warunkowym funkcji usługi Azure Active Directory. Za pomocą zasad programu Exchange można także poddać kwarantannie urządzenie, które blokuje dostęp do poczty e-mail. Więcej informacji na temat zarządzania urządzeniami z programem Exchange można znaleźć [tutaj]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
