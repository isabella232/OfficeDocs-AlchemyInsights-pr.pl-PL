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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366438"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitorowanie dostępu warunkowego dla programu Exchange

Użytkownicy ukierunkowany na dostęp warunkowy otrzymają powiadomienie pocztą e-mail, jeśli nie spełnią wymagań organizacji dotyczących dostępu. W celu rozwiązania problemu zalecamy co najmniej jedno z następujących rozwiązań:

- Jeśli urządzenie jest uważane za zarejestrowane, zaleca się, aby użytkownik przeszedł do aplikacji Portal firmy i upewnić się, że jest wyświetlany w portalu firmy. Jeśli nie, użytkownik powinien zarejestrować urządzenie.
- W portalu Azure przejdź do usługi Intune > Device. W obszarze Monitor kliknij pozycję Zgodność urządzenia. Wyświetl raport zgodności urządzenia, aby sprawdzić, czy urządzenie użytkownika jest oznaczone jako zgodne.
- W portalu Azure przejdź do usługi Intune > Device. W obszarze Zarządzanie kliknij pozycję zasady. Na liście zasad zgodności Sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli żaden profil nie jest przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.
- Edytowanie przydziału dostępu warunkowego użytkownika.

1. W portalu Azure Portal przejdź do **Intune**  >  **zasad dostępu warunkowego**usługi Intune  >  **Policies**.
2. Wybierz zasadę z listy.
3. Kliknij pozycję Użytkownicy i grupy.
4. Aby określić zasady jako docelowe dla określonej osoby, Dodaj je do listy dołączania. Aby upewnić się, że dana osoba zostanie pominięta w zasadach, Dodaj je do listy wykluczania.

Pomocne linki:

[Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rozwiązywanie problemów dotyczących urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Zasady rozwiązywania problemów](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Monitorowanie zgodności urządzenia usługi Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Uwaga: te czynności są pomocne tylko w rozwiązywaniu problemów z funkcją dostęp warunkowy usługi Azure Active Directory. Możliwe jest również poddawanie kwarantannie urządzenia blokującego dostęp do poczty e-mail za pomocą zasad programu Exchange. Więcej informacji na temat zarządzania urządzeniami programu Exchange można znaleźć [tutaj](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).
