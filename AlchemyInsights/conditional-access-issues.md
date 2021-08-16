---
title: Problemy z dostępem warunkowym
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069974"
---
# <a name="conditional-access-issues"></a>Problemy z dostępem warunkowym

**Rozwiązywanie problemów z diagnostyką logowania**

Aby szybko dowiedzieć się, co się stało lub zdiagnozować problemy związane z logowaniem użytkownika, możesz użyć narzędzia [diagnostycznego logowania:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Uruchom narzędzie Diagnostyczne logowanie.
1. Znajdź zdarzenie do przeanalizowania, wprowadzając szczegółowe informacje dotyczące użytkownika, aplikacji, godziny logowania, identyfikatora żądania lub identyfikatora korelacji.
1. Przejrzyj wyniki diagnostyczne pokazujące szczegóły tego, co się stało, i czynności, które możesz wykonać, aby wprowadzić zmiany (jeśli są potrzebne jakieś zmiany).

**Procedura rozwiązywania problemów z logowaniem** 

1. Przejdź do strony logowania w usłudze Azure AD.
1. Filtruj logowania według użytkownika, zakresu czasu, aplikacji, stanu, aplikacji klienckiej i tak dalej.
1. Wybierz zdarzenie logowania i wyświetl kartę Dostęp warunkowy, aby sprawdzić, które zasady zostały ocenione.
1. Kliknij wiersz zasad, aby wyświetlić szczegóły zasad i dowiedzieć się, dlaczego je zastosowano.

**Narzędzia do rozwiązywania problemów z zasadami dostępu warunkowego**

- Tryb tylko do raportu umożliwia ocenę zasad bez wpływu na użytkowników.
- Narzędzie symulacji pozwala symulować zdarzenia logowania i zobaczyć, które zasady mają zastosowanie.
- Szczegółowe informacje i raportowania są wyświetlane wpływ poszczególnych zasad na czas rzeczywisty.

**Zasady ochrony według planu bazowego**

Zasady ochrony według planu bazowego zostały wycofane. Nie są one już wymuszane i wkrótce zostaną usunięte z portalu Azure Portal. Zalecamy włączenie [ustawień domyślnych zabezpieczeń.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Aby uzyskać więcej informacji na temat dostępu warunkowego, zobacz:

[Najlepsze rozwiązania dotyczące dostępu warunkowego w programie Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Warunki w dostępie warunkowym](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrolki w dostępie warunkowym](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokalizacje w dostępie warunkowym](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
