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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014888"
---
# <a name="conditional-access-issues"></a>Problemy z dostępem warunkowym

**Rozwiązywanie problemów z diagnostyką logowania**

Możesz szybko dowiedzieć się, co się stało lub zdiagnozować o problemach związanych z logowaniem się użytkowników przy użyciu [diagnostyki logowania](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Uruchom diagnostykę logowania.
1. Znajdź zdarzenie, które ma zostać zanalizowane, wprowadzając szczegółowe informacje o użytkowniku, aplikacji, czasie logowania, identyfikatorze żądania lub identyfikatorze korelacji.
1. Przejrzyj wyniki diagnostyczne przedstawiające szczegóły dotyczące tego, co się stało, oraz jakie działania możesz podjąć, aby wprowadzić zmiany (jeśli są potrzebne zmiany).

**Procedura rozwiązywania problemów z logowaniem** 

1. Przejdź do strony logowania usługi Azure AD.
1. Filtruj logowanie według użytkownika, zakresu czasu, aplikacji, statusu, aplikacji klienckiej itd.
1. Wybierz zdarzenie logowania i Wyświetl kartę dostęp warunkowy, aby sprawdzić, które zasady zostały oszacowane.
1. Kliknij wiersz zasady, aby wyświetlić szczegółowe informacje o zasadach i zrozumieć, dlaczego jest ona stosowana.

**Narzędzia do rozwiązywania problemów z zasadami dostępu warunkowego**

- Tryb tylko w raporcie umożliwia ocenę zasad bez wpływu na użytkowników.
- Narzędzie warunkowe umożliwia symulowanie zdarzeń logowania i sprawdzanie, jakie zasady obowiązują.
- W skoroszycie informacji szczegółowych i raportowania jest wyświetlany wpływ poszczególnych zasad na czas w czasie rzeczywistym.

**Zasady ochrony planu bazowego**

Zasady ochrony planu bazowego są przestarzałe. Nie są już wymuszane i wkrótce zostaną usunięte z portalu Azure Portal. Zalecamy włączenie [ustawień domyślnych zabezpieczeń](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Aby uzyskać więcej informacji o dostępie warunkowym, zobacz:

[Najważniejsze wskazówki dotyczące dostępu warunkowego w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Warunki w dostępie](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 warunkowym [Formanty w dostępie](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 warunkowym [Lokalizacje w dostępie warunkowym](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
