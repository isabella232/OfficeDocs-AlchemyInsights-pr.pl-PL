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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082952"
---
# <a name="authentication-app"></a>Aplikacja do uwierzytelniania

Jeśli jesteś administratorem globalnym, możesz szybko dowiedzieć się, co się stało lub zdiagnozować problemy związane z logowaniem użytkownika, korzystając z [diagnostyki logowania.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Uruchom diagnostykę, klikając przycisk "[Uruchom diagnostykę".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Znajdź zdarzenie do przeanalizowania, wprowadzając szczegółowe informacje dotyczące użytkownika, aplikacji, godziny logowania, identyfikatora żądania lub identyfikatora korelacji.
1. Przejrzyj wyniki diagnostyczne ze szczegółami tego, co się stało, i czynnościami, które można podjąć, aby wprowadzić zmiany, jeśli są potrzebne.

**Sprawdź scenariusz, który ma zastosowanie:**

1. Jeśli użytkownik nie jest wyświetlany w aplikacji usługi Microsoft Authenticator, sprawdź, czy nie jest on wyświetlany w obszarze zablokowanych użytkowników uwierzytelniania MFA zgodnie z opisem w tece Blokowanie [i odblokowywanie użytkowników.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Jeśli użytkownik nie zostanie zablokowany na uwierzytelniania MFA, ale nie otrzyma powiadomienia push, może otworzyć aplikację usługi Microsoft Authenticator, co spowoduje pociągnięcie oczekujących wniosków o zatwierdzenie.
1. Alternatywnym sposobem logowania jest kliknięcie przycisku Zaloguj się w inny sposób i wybranie kodu weryfikacyjnego z mojej aplikacji mobilnej.
1. Aplikacja Microsoft Authenticator jest jedyną dostępną metodą dla wielu użytkowników. [Dowiedz się więcej o ustawieniach domyślnych zabezpieczeń](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), sprawdź [Authenticator często](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) zadawanych pytań dotyczących aplikacji oraz sposobu ich rozwiązywania.
 
**Polecane klipy wideo**

[Jak skonfigurować aplikację Authenticator na nowym telefonie (2 min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
