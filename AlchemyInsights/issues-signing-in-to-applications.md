---
title: Problemy z logowaniem się do aplikacji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901330"
---
# <a name="issues-signing-in-to-applications"></a>Problemy z logowaniem się do aplikacji

Aby wykryć przyczyny problemów związanych z logowaniem się użytkowników, wykonaj następujące czynności:

1. Uruchom [diagnostykę logowania](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Znajdź zdarzenie, które ma zostać zanalizowane, wprowadzając szczegółowe informacje o użytkowniku, aplikacji, godzinie logowania, identyfikatorze żądania lub identyfikatorze korelacji.
3. Przejrzyj wyniki diagnostyczne przedstawiające szczegóły dotyczące tego, co się stało, oraz jakie działania możesz podjąć w celu wprowadzenia zmian, jeśli konieczne są zmiany.

Poniżej przedstawiono kilka typowych problemów, które mogą wystąpić podczas logowania się do aplikacji:

1. Użytkownik lub użytkownik **zakończył logowanie się do usługi Azure AD, ale widzi nieoczekiwany monit** — Zobacz artykuł nieoczekiwana [zgoda podczas logowania się do aplikacji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) i [nieoczekiwany błąd podczas wykonywania zgody na aplikację](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Użytkownik lub użytkownik zalogował się **do aplikacji bezpośrednio, ale nie może zalogować się do niego z głębokiego łącza w portalu niestandardowym lub panelu programu Access**: zobacz [Rozwiązywanie problemów z logowaniem się do aplikacji z usługi Azure AD moje aplikacje](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Użytkownik lub użytkownik **zakończył logowanie do usługi Azure AD, ale aplikacja wyświetla komunikat o błędzie i nie zezwala użytkownikowi na zakończenie przepływu logowania**: problem polega na tym, że aplikacja nie zaakceptowała odpowiedzi wydanej przez usługę Azure AD. Wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) , aby rozwiązać problem.
4. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji innej niż Galeria skonfigurowanej do logowania** jednokrotnego: Postępuj zgodnie z instrukcjami w [poniższych krokach](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , aby rozwiązać problem.
5. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji Microsoft Azure AD Gallery skonfigurowanej do logowania** jednokrotnego: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , aby rozwiązać problem.
6. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji firmy Microsoft**: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) , aby rozwiązać problem.
7. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji innej niż Galeria skonfigurowanej do federacyjnego logowania** jednokrotnego: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) , aby rozwiązać problem.
8. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji Microsoft Azure AD Gallery skonfigurowanej do federacyjnego logowania** jednokrotnego: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , aby rozwiązać problem.
9. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji rozwiniętej niestandardowo**: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , aby rozwiązać problem.
10. Użytkownik lub użytkownik **nie mogą zalogować się do aplikacji lokalnej przy użyciu serwera proxy aplikacji Azure AD**: wykonaj [poniższe czynności](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) , aby rozwiązać problem.

