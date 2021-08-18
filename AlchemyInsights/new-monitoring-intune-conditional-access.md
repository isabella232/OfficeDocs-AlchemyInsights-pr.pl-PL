---
title: Monitorowanie dostępu warunkowego w usłudze Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327567"
---
# <a name="monitor-intune-conditional-access"></a>Monitorowanie dostępu warunkowego w usłudze Intune

Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełnią wymagań dotyczących dostępu do organizacji. Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:

1. Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji usługi Portal firmy i sprawdź, czy jest ono widoczne w Portal firmy. Jeśli tak się nie stanie, użytkownik musi zarejestrować urządzenie.
1. W portalu Azure przejdź do tematu **Zgodność urządzenia**  >  **Intune**. 
1. Aby wyświetlić raport zgodności urządzenia w celu potwierdzenia, że urządzenie użytkownika jest zgodne, w obszarze **Monitorowanie** kliknij pozycję **Zgodność urządzenia**.
1. W portalu Azure przejdź do tematu **Zgodność urządzenia**  >  **Intune**. W **obszarze Zarządzanie kliknij** pozycję **Zasady**. Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli żaden profil nie został przypisany, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.
1. Edytuj przypisanie dostępu warunkowego użytkownika.
1. W portalu Azure przejdź do strony **Intune** Zasady dostępu  >  **warunkowego,** wybierz zasady z  >  listy, a następnie kliknij pozycję Użytkownicy **i grupy.**
1. Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do **listy Uwzględnij.** Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do **listy Wyklucz.**

**Przydatne linki:**

- [Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Rozwiązywanie problemów z urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Zasady rozwiązywania problemów](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorowanie zgodności urządzenia w usłudze Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Uwaga:** te kroki są pomocne tylko podczas rozwiązywania problemów z Azure Active Directory dostęp warunkowy. Można także poddać kwarantannie urządzenie, które blokuje dostęp do poczty e-mail za pomocą Exchange poczty e-mail. Więcej informacji na Exchange zarządzania urządzeniami można znaleźć [**tutaj.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
