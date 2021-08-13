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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975111"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorowanie dostępu warunkowego Exchange

Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełniają wymagań dotyczących dostępu do organizacji. Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:

- Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji usługi Portal firmy i sprawdź, czy jest ono widoczne w Portal firmy. Jeśli tak się nie stanie, użytkownik powinien zarejestrować urządzenie.
- W portalu Azure przejdź do intune > zgodności urządzenia. W obszarze Monitor kliknij pozycję Zgodność urządzenia. Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest zgodne.
- W portalu Azure przejdź do intune > zgodności urządzenia. W obszarze Zarządzanie kliknij pozycję Zasady. Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli żaden profil nie został przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.
- Edytuj przypisanie dostępu warunkowego użytkownika.

1. W portalu Azure przejdź do tematu **Zasady dostępu**  >  **warunkowego usługi**  >  Intune.
2. Wybierz zasady z listy.
3. Kliknij pozycję Użytkownicy i grupy.
4. Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do listy Uwzględnij. Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do listy Wyklucz.

Przydatne linki:

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów z urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorowanie zgodności urządzenia w usłudze Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Uwaga: te kroki są pomocne tylko podczas rozwiązywania problemów z Azure Active Directory dostęp warunkowy. Istnieje również możliwość kwarantanny urządzenia blokującego dostęp do poczty e-mail za pomocą Exchange poczty e-mail. Więcej informacji na Exchange zarządzania urządzeniami można znaleźć [tutaj]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
