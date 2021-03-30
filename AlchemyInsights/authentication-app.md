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
# <a name="authentication-app"></a><span data-ttu-id="2aea0-102">Aplikacja do uwierzytelniania</span><span class="sxs-lookup"><span data-stu-id="2aea0-102">Authentication app</span></span>

<span data-ttu-id="2aea0-103">Jeśli jesteś administratorem globalnym, możesz szybko dowiedzieć się, co się stało lub zdiagnozować problemy związane z logowaniem użytkownika, korzystając z [diagnostyki logowania.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="2aea0-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="2aea0-104">Uruchom diagnostykę, klikając przycisk "[Uruchom diagnostykę".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="2aea0-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="2aea0-105">Znajdź zdarzenie do przeanalizowania, wprowadzając szczegółowe informacje dotyczące użytkownika, aplikacji, godziny logowania, identyfikatora żądania lub identyfikatora korelacji.</span><span class="sxs-lookup"><span data-stu-id="2aea0-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="2aea0-106">Przejrzyj wyniki diagnostyczne ze szczegółami tego, co się stało, i czynnościami, które można podjąć, aby wprowadzić zmiany, jeśli są potrzebne.</span><span class="sxs-lookup"><span data-stu-id="2aea0-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="2aea0-107">**Sprawdź scenariusz, który ma zastosowanie:**</span><span class="sxs-lookup"><span data-stu-id="2aea0-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="2aea0-108">Jeśli użytkownik nie jest wyświetlany w aplikacji Microsoft Authenticator z powiadomieniem push, sprawdź, czy nie jest on wyświetlany w obszarze zablokowanych użytkowników uwierzytelniania wieloskładnikowego, jak to opisano w tece Blokowanie [i odblokowywanie użytkowników.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="2aea0-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="2aea0-109">Jeśli użytkownik nie zostanie zablokowany na uwierzytelnianie MFA, ale nie otrzyma powiadomienia push, może otworzyć aplikację Microsoft Authenticator, co spowoduje odciągnięcie oczekujących próśb o zatwierdzenie.</span><span class="sxs-lookup"><span data-stu-id="2aea0-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="2aea0-110">Alternatywnym sposobem logowania jest kliknięcie przycisku Zaloguj się w inny sposób i wybranie kodu weryfikacyjnego z mojej aplikacji mobilnej.</span><span class="sxs-lookup"><span data-stu-id="2aea0-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="2aea0-111">Aplikacja Microsoft Authenticator jest jedyną dostępną metodą dla wielu użytkowników.</span><span class="sxs-lookup"><span data-stu-id="2aea0-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="2aea0-112">[Dowiedz się więcej o ustawieniach domyślnych zabezpieczeń](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), zobacz Często zadawane pytania dotyczące aplikacji [Authenticator,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) aby uzyskać odpowiedzi na często zadawane pytania i dowiedzieć się, jak je rozwiązać.</span><span class="sxs-lookup"><span data-stu-id="2aea0-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="2aea0-113">**Polecane klipy wideo**</span><span class="sxs-lookup"><span data-stu-id="2aea0-113">**Recommended Videos**</span></span>

<span data-ttu-id="2aea0-114">[Jak skonfigurować aplikację Authenticator na nowym telefonie (2 min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="2aea0-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
