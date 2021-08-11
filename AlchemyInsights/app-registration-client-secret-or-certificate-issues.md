---
title: Problemy z kluczem tajnym klienta rejestracji aplikacji lub certyfikatem
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951503"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemy z kluczem tajnym klienta rejestracji aplikacji lub certyfikatem

Klucz tajny klienta aplikacji wygasa?

Niezależnie od sposobu utworzenia zarejestrowanej aplikacji, czy to w ramach standardowego procesu rejestracji w portalu rejestracji aplikacji, czy też podmiot zabezpieczeń usługi został utworzony w dzierżawie przy użyciu zgody aplikacji, przed wygaśnięciem bieżącej aplikacji musi zostać utworzony nowy klucz tajny klienta i zaktualizowany w powiązanym kodzie aplikacji. Maksymalny okres ważności to 2 lata. Warto pamiętać, że wartość tajna musi być rejestrowana, ponieważ nie będzie już widoczna po opuszczeniu strony rejestracji aplikacji w portalu. Aby uzyskać więcej informacji, zobacz [Szybki start: rejestrowanie](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplikacji w aplikacji Platforma tożsamości Microsoft i Najlepsze rozwiązania [dotyczące aplikacji dla Platforma tożsamości Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Aby dowiedzieć się więcej, [zobacz Tworzenie aplikacji Usługi Azure AD & podmiotu](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)zabezpieczeń usługi w portalu — Platforma tożsamości Microsoft.
