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
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427925"
---
# <a name="monitor-intune-conditional-access"></a>Monitorowanie dostępu warunkowego w usłudze Intune

Użytkownicy z dostępem warunkowym otrzymają powiadomienie e-mail, jeśli nie spełniają wymagań dotyczących dostępu do organizacji. Aby rozwiązać problem, zalecamy co najmniej jedno z następujących rozwiązań:

1. Jeśli urządzenie powinno zostać zarejestrowane, zasuń użytkownika do aplikacji Portal firmy i sprawdź, czy jest ono widoczne w portalu firmy. Jeśli tak się nie stanie, użytkownik musi zarejestrować urządzenie.
1. W portalu Azure przejdź do tematu **zgodność**  >  **urządzenia Intune.** 
1. Aby wyświetlić raport zgodności urządzenia w celu sprawdzenia, czy urządzenie użytkownika jest zgodne, w obszarze **Monitorowanie** kliknij pozycję **Zgodność urządzenia.**
1. W portalu Azure przejdź do tematu **zgodność**  >  **urządzenia Intune.** W **obszarze Zarządzanie kliknij** pozycję **Zasady.** Na liście zasad zgodności sprawdź, czy profil jest przypisany do urządzenia użytkownika. Jeśli nie przypisano żadnego profilu, usługa Intune nie będzie mogła potwierdzić stanu zgodności urządzenia.
1. Edytuj przypisanie dostępu warunkowego użytkownika.
1. W portalu Azure przejdź do zasad dostępu warunkowego usługi **Intune,** wybierz zasady z listy, a następnie kliknij pozycję  >    >  Użytkownicy **i grupy.**
1. Aby zasady dotyczące określonej osoby dotyczyły określonej osoby, dodaj ją do **listy Dołącz.** Aby mieć pewność, że dana osoba zostanie pominięta w zasadach, dodaj ją do **listy Wyklucz.**

**Przydatne linki:**

- [Omówienie zgodności urządzeń](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Rozwiązywanie problemów z urzędu certyfikacji](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Zasady rozwiązywania problemów](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Monitorowanie zgodności urządzenia w usłudze Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Te kroki są pomocne tylko podczas rozwiązywania problemów z dostępem warunkowym funkcji usługi Azure Active Directory. Za pomocą zasad programu Exchange można także poddać kwarantannie urządzenie, które blokuje dostęp do poczty e-mail. Więcej informacji na temat zarządzania urządzeniami z programem Exchange można znaleźć [**tutaj.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
