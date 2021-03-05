---
title: Inicjowanie obsługi administracyjnej użytkowników
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481884"
---
# <a name="user-provisioning"></a>Inicjowanie obsługi administracyjnej użytkowników

- Użyj funkcji [inicjowania obsługi na](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) żądanie, aby aprowizować użytkownika i uzyskać szczegółową diagnostykę kroków.
- Aby rozwiązać problemy napotykane podczas inicjowania obsługi administracyjnej użytkowników i grup, zobacz przewodnik po rozwiązywaniu problemów, w którym nie jest [zapewniana inicjowanie obsługi użytkowników.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Jeśli zauważysz, że użytkownicy nie są aprowni adresaci, zobacz dzienniki inicjowania obsługi [administracyjnej (wersja Preview)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) w usłudze Azure Active Directory (AD). Wyszukaj wpisy dziennika dotyczące określonego użytkownika.
- Okresowo ponownie uruchamiaj inicjowanie obsługi administracyjnej, aby wychwycić wszystkich użytkowników, których pominięto w poprzednim cyklu inicjowania obsługi.
- Być może obsługi administracyjnej użytkownika/grupy nie było, ponieważ usługa nie miała jeszcze możliwości oceny użytkownika. Zapoznaj się ze wskazówkami, jak długo trwa inicjowanie obsługi administracyjnej, a także z paska postępu na stronie konfiguracji inicjowania obsługi. Jeśli stan określony w sekcji dodatkowych szczegółów jest stały przed datą utworzenia/zaktualizowania/usunięcia użytkownika, oznacza to, że nie został jeszcze ocenić użytkownika. W tym scenariuszu najlepiej jest zaczekać na ukończenie obsługi administracyjnej. Jeśli stan jest stały, zalecamy wykonanie ponownego uruchomienia z interfejsu użytkownika w portalu Azure Portal.
  - Pamiętaj, że usługa ma świadomość zmian wprowadzonych tylko do użytkownika/grupy w systemie źródłowym (Azure Active Directory). Jeśli użytkownik/grupa zostanie usunięta bezpośrednio z aplikacji (na przykład ServiceNow), nie wiemy o tych zmianach i nie cofniemy ich na podstawie stanu użytkownika w systemie źródłowym. W tym scenariuszu najlepszym rozwiązaniem jest wycofywanie zmiany bezpośrednio w aplikacji docelowej.
- Nasza usługa oszacowała użytkownika/grupę i ustaliła, że nie należy jej zapewniać obsługi administracyjnej:
  - Jeśli zakres został ustawiony na przypisanych użytkowników i grupy, sprawdź, czy do aplikacji przypisano użytkownika lub grupę.
  - Jeśli do aplikacji przypisano użytkownika/grupę, upewnij się, że nie jest on przypisany do domyślnej roli dostępu. Tej roli nie można używać do inicjowania obsługi administracyjnej.
  - Jeśli ustawiono filtr zakresu oparty na atrybutach, upewnij się, że użytkownik spełnia określone kryteria.
  - Jeśli użytkownicy już istnieją w systemie docelowym i stanie użytkownika w dopasowaniu źródłowym i docelowym, nie podejmiemy dalszych działań.
- Usługa próbowała aprowizować użytkownika i nie powiodło się. Aby zapoznać się z tymi scenariuszami, zapoznaj się z kartą rozwiązywania problemów i zaleceń dzienników inicjowania obsługi:
  - W usłudze Azure Active Directory może brakować wymaganego atrybutu użytkownika lub format wymagany przez aplikację innej firmy. Na przykład atrybut Country na użytkowniku może mieć wartość Stany Zjednoczone, gdy powinien to być Stan Zjednoczone.
  - Ten atrybut jest atrybutem referential, który jeszcze nie istnieje w aplikacji docelowej. Atrybut referential to atrybut, który wskazuje inny obiekt, na przykład użytkownika, który jest członkiem grupy. Identyfikator użytkownika będzie miał atrybut członka grupy, ale może być przetwarzany tylko wtedy, gdy obiekt użytkownika, na który wskazuje, już istnieje.
