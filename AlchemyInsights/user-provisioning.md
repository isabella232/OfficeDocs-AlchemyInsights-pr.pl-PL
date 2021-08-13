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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971349"
---
# <a name="user-provisioning"></a>Inicjowanie obsługi administracyjnej użytkowników

- Korzystaj z [funkcji inicjowania obsługi na](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) żądanie, aby aprowizować użytkownika i uzyskać szczegółową diagnostykę kroków.
- Aby rozwiązać problemy napotykane podczas inicjowania obsługi użytkowników i grup, zobacz przewodnik po rozwiązywaniu problemów Brak [obsługi administracyjnej użytkowników.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Jeśli obserwujesz, że użytkownicy nie są inicjowania obsługi administracyjnej, zobacz Dzienniki inicjowania obsługi [administracyjnej (wersja zapoznawcza)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) w programie Azure Active Directory (AD). Wyszukaj wpisy dziennika dotyczące określonego użytkownika.
- Okresowo ponownie uruchom inicjowanie obsługi administracyjnej, aby wychwycić wszystkich użytkowników, których nie ominięto w poprzednim cyklu inicjowania obsługi.
- Być może obsługi administracyjnej użytkownika/grupy nie było, ponieważ usługa nie miała jeszcze możliwości oceny użytkownika. Przejrzyj wskazówki dotyczące czasu inicjowania obsługi oraz paska postępu na stronie konfiguracji inicjowania obsługi. Jeśli stan stały określony w sekcji dodatkowych szczegółów jest przed datą utworzenia/zaktualizowania/usunięcia użytkownika, oznacza to, że nie ocenić jeszcze użytkownika. W tym scenariuszu najlepiej jest zaczekać na ukończenie usługi inicjowania obsługi administracyjnej. Jeśli osiągnięto stały stan, zalecamy wykonanie ponownego uruchomienia z interfejsu użytkownika w portalu Azure Portal.
  - Pamiętaj, że nasza usługa wie tylko o zmianach użytkownika/grupy w systemie źródłowym (Azure Active Directory). Jeśli użytkownik/grupa zostanie usunięta bezpośrednio w aplikacji (na przykład ServiceNow), nie wiemy o tych zmianach i nie wycofamy ich w zależności od stanu użytkownika w systemie źródłowym. W tym scenariuszu najlepiej jest wycofać zmianę bezpośrednio w aplikacji docelowej.
- Nasza usługa ocenić użytkownika/grupę i ustaliła, że nie powinna być zapewniana obsługa administracyjne:
  - Jeśli został ustawiony zakres przypisany do użytkowników i grup, sprawdź, czy użytkownik/grupa nie jest przypisana do aplikacji.
  - Jeśli do aplikacji przypisano użytkownika/grupę, upewnij się, że nie jest on przypisany do domyślnej roli dostępu. Tej roli nie można używać do inicjowania obsługi administracyjnej.
  - Jeśli ustawiono filtr zakresu określony na podstawie atrybutów, upewnij się, że użytkownik spełnia określone kryteria.
  - Jeśli użytkownicy już istnieją w systemie docelowym oraz w stanie dopasowania źródłowego i docelowego użytkownika, nie podejmiemy dalszych działań.
- Nasz usługa próbowała aprowizować użytkownika i nie powiodło się. Aby zapoznać się z tymi scenariuszami, zapoznaj się z kartą rozwiązywania problemów i zaleceń dzienników inicjowania obsługi:
  - Wymagany atrybut dla użytkownika może brakować w Azure Active Directory lub nie jest w formacie wymaganym przez aplikację innej firmy. Na przykład atrybut Country użytkownika może mieć ustawioną wartość Stany Zjednoczone, jeśli ma wartość Stany Zjednoczone.
  - Ten atrybut jest atrybutem referential, który jeszcze nie istnieje w aplikacji docelowej. Atrybut referential to atrybut, który wskazuje inny obiekt, na przykład użytkownika, który jest członkiem grupy. Identyfikator użytkownika znajduje się w atrybutym członka grupy, ale może być przetwarzany tylko wtedy, gdy obiekt użytkownika, na który wskazuje, już istnieje.
