---
title: Dzienniki haseł
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527177"
---
# <a name="password-logs"></a>Dzienniki haseł

**Występują problemy z uzyskiwaniem dostępu do dzienników inspekcji resetowania hasła**

Aby rozwiązać problemy dotyczące dostępu do dzienników inspekcji resetowania hasła, wykonaj następujące czynności:

Upewnij się, że masz uprawnienia do wyświetlania dzienników inspekcji. 

Autoryzowane są tylko następujące role:
 - Administrator globalny
 - Administrator zabezpieczeń
 - Czytelnik zabezpieczeń

**Chcę wyświetlić wszystkie zdarzenia inspekcji resetowania hasła od chwili wstępnego wdrożenia**

W raportach z ostatnich 30 dni jest przechowywanych maksymalnie 120 000 zdarzeń resetowania/rejestracji hasła. Ten maksymalny limit dotyczy interfejsu użytkownika podczas pobierania pliku CSV. Za pośrednictwem programu PowerShell dostępnych jest 1 milion zdarzeń.
Aby uzyskać więcej informacji, zobacz poniższe linki:

- [Zdarzenia samodzielnego resetowania hasła z interfejsu API raportów i zdarzeń usługi Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak szybko pobrać zdarzenia rejestracji resetowania hasła za pomocą programu PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Chcę dowiedzieć się więcej o możliwościach raportowania resetowania haseł**

Sprawdź, kto rejestruje lub resetuje hasła w dziennikach inspekcji resetowania haseł usługi Azure AD w portalu Azure w **obszarze Użytkownicy i grupy.**
Aby uzyskać więcej informacji, zobacz następujące linki:

- [Omówienie raportów dotyczących resetowania hasła](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak wyświetlić raporty resetowania hasła w portalu Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Zdarzenia samodzielnego resetowania hasła z interfejsu API raportów i zdarzeń usługi Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Jak szybko pobrać zdarzenia rejestracji resetowania hasła za pomocą programu PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


