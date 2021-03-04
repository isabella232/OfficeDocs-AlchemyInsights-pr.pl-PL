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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430202"
---
# <a name="problem-with-single-user"></a>Problem z jednym użytkownikiem

- Być może użytkownikowi nie zapewniano obsługi administracyjnej, ponieważ usługa nie miała jeszcze możliwości oceny użytkownika. Zapoznaj się ze wskazówkami, jak długo trwa inicjowanie obsługi administracyjnej, a także z paska postępu na stronie konfiguracji inicjowania obsługi. Jeśli stan określony w sekcji dodatkowych szczegółów jest stały przed datą utworzenia/aktualizacji/usunięcia użytkownika, oznacza to, że ten użytkownik nie został jeszcze ocenić. W tym scenariuszu najlepiej jest zaczekać na ukończenie obsługi administracyjnej.

  - Pamiętaj, że usługa ma świadomość zmian wprowadzonych tylko do użytkownika w systemie źródłowym (Cloud HR). Aby wykryć zmianę i przepływać ją do usługi Active Directory, w systemie źródłowym usługi Azure AD musi być prawidłowa zmiana.
- Usługa inicjowania obsługi administracyjnej oszacowała użytkownika i ustaliła, że nie powinna być zapewniana obsługa aprowizowana:
  - Jeśli ustawiono filtr zakresu oparty na atrybutach, upewnij się, że użytkownik spełnia określone kryteria.
  - Jeśli użytkownicy już istnieją w systemie docelowym i stanie użytkownika w dopasowaniu źródłowym i docelowym, nie podejmiemy dalszych działań.
- Usługa inicjowania obsługi administracyjnej próbowała aprowizować użytkownika i nie powiodła się. Aby zapoznać się z tymi scenariuszami, zapoznaj się z kartą rozwiązywania problemów i zaleceń dzienników inicjowania obsługi:
  - W lokalnej usłudze Active Directory lub usłudze Azure AD może brakować wymaganego atrybutu użytkownika. Na przykład reguły generowania userPrincipalName lub sAMAccountName nie generują odpowiedniej wartości.
  - Zgodny atrybut (zwykle identyfikator pracownika) nie jest rozpoznawny dla unikatowego użytkownika w lokalnej usłudze Active Directory lub usłudze Azure AD. Na przykład dwóch użytkowników ma ten sam identyfikator pracownika w usłudze AD, a usługa zwraca kod błędu wskazujący zduplikowane wpisy docelowe dla tego samego wpisu źródłowego.

Aby przejrzeć dzienniki dla jednego użytkownika i grup, zobacz Przeglądanie dzienników inicjowania obsługi [dla problemu z określonym użytkownikiem.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
