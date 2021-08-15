---
title: Problem z jednym użytkownikiem
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
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960161"
---
# <a name="problem-with-single-user"></a>Problem z jednym użytkownikiem

- Być może użytkownik nie ma obsługi administracyjnej, ponieważ usługa nie ma jeszcze możliwości oceny użytkownika. Przejrzyj wskazówki dotyczące czasu inicjowania obsługi oraz paska postępu na stronie konfiguracji inicjowania obsługi. Jeśli stan stały określony w sekcji dodatkowych szczegółów jest przed datą utworzenia/zaktualizowania/usunięcia użytkownika, oznacza to, że nie ocenić jeszcze użytkownika. W tym scenariuszu najlepiej jest zaczekać na ukończenie usługi inicjowania obsługi administracyjnej.

  - Pamiętaj, że usługa ma świadomość zmian wprowadzonych tylko do użytkownika w systemie źródłowym (Cloud HR). Aby wykryć zmianę i przepływać ją do usługi Active Directory, w systemie źródłowym usługi Azure AD musi być prawidłowa zmiana.
- Usługa inicjowania obsługi administracyjnej oceń użytkownika i ustaliła, że nie powinna być zapewniana obsługa administracyjne:
  - Jeśli ustawiono filtr zakresu określony na podstawie atrybutów, upewnij się, że użytkownik spełnia określone kryteria.
  - Jeśli użytkownicy już istnieją w systemie docelowym oraz w stanie dopasowania źródłowego i docelowego użytkownika, nie podejmiemy dalszych działań.
- Usługa inicjowania obsługi administracyjnej próbowała aprowizować użytkownika i nie powiodła się. Aby zapoznać się z tymi scenariuszami, zapoznaj się z kartą rozwiązywania problemów i zaleceń dzienników inicjowania obsługi:
  - W lokalnej usłudze Active Directory lub Azure AD może brakować wymaganego atrybutu użytkownika. Na przykład reguły generowania userPrincipalName lub sAMAccountName nie generują odpowiedniej wartości.
  - Zgodny atrybut (zwykle identyfikator pracownika) nie jest rozpoznawny dla unikatowego użytkownika w lokalnej usłudze Active Directory lub Azure AD. Na przykład dwóch użytkowników z tym samym identyfikatorem pracownika w usłudze AD i usługa zwraca kod błędu wskazujący zduplikowane pozycje docelowe dla tego samego wpisu źródłowego.

Aby przejrzeć dzienniki dla pojedynczych użytkowników i grup, zobacz Przeglądanie dzienników inicjowania obsługi w celu sprawdzenia, czy nie występuje [problem z określonym użytkownikiem.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
