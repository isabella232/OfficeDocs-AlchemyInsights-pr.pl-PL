---
title: Aplikacja do uwierzytelniania
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405068"
---
# <a name="authentication-app"></a>Aplikacja do uwierzytelniania

Jeśli jesteś administratorem globalnym, możesz szybko dowiedzieć się, co się stało lub zdiagnozować problemy związane z logowaniem użytkownika, korzystając z [diagnostyki logowania.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Uruchom diagnostykę, klikając przycisk "[Uruchom diagnostykę".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Znajdź zdarzenie do przeanalizowania, wprowadzając szczegółowe informacje dotyczące użytkownika, aplikacji, godziny logowania, identyfikatora żądania lub identyfikatora korelacji.
1. Przejrzyj wyniki diagnostyczne ze szczegółami tego, co się stało, i czynnościami, które można podjąć, aby wprowadzić zmiany, jeśli są potrzebne.

**Sprawdź scenariusz, który ma zastosowanie:**

1. Jeśli użytkownik nie jest wyświetlany w aplikacji Microsoft Authenticator z powiadomieniem push, sprawdź, czy nie jest on wyświetlany w obszarze zablokowanych użytkowników uwierzytelniania wieloskładnikowego, jak to opisano w tece Blokowanie [i odblokowywanie użytkowników.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Jeśli użytkownik nie zostanie zablokowany na uwierzytelnianie MFA, ale nie otrzyma powiadomienia push, może otworzyć aplikację Microsoft Authenticator, co spowoduje odciągnięcie oczekujących próśb o zatwierdzenie.
1. Alternatywnym sposobem logowania jest kliknięcie przycisku Zaloguj się w inny sposób i wybranie kodu weryfikacyjnego z mojej aplikacji mobilnej.
1. Aplikacja Microsoft Authenticator jest jedyną dostępną metodą dla wielu użytkowników. [Dowiedz się więcej o ustawieniach domyślnych zabezpieczeń](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), zobacz Często zadawane pytania dotyczące aplikacji [Authenticator,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) aby uzyskać odpowiedzi na często zadawane pytania i dowiedzieć się, jak je rozwiązać.
 
**Polecane klipy wideo**

[Jak skonfigurować aplikację Authenticator na nowym telefonie (2 min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
