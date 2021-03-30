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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404781"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Problemy z kluczem tajnym klienta rejestracji aplikacji lub certyfikatem

Klucz tajny klienta aplikacji wygasa?

Niezależnie od sposobu utworzenia zarejestrowanej aplikacji, czy to w ramach standardowego procesu rejestracji w portalu rejestracji aplikacji, czy też podmiot zabezpieczeń usługi został utworzony w dzierżawie przy użyciu zgody aplikacji, przed wygaśnięciem bieżącej aplikacji musi zostać utworzony nowy klucz tajny klienta i zaktualizowany w powiązanym kodzie aplikacji. Maksymalny okres ważności to 2 lata. Warto pamiętać, że wartość tajna musi być rejestrowana, ponieważ nie będzie już widoczna po opuszczeniu strony rejestracji aplikacji w portalu. Aby uzyskać więcej informacji, zobacz [Szybki start: rejestrowanie](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplikacji na platformie tożsamości Firmy Microsoft i [Najlepsze rozwiązania dotyczące platformy tożsamości firmy Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Aby dowiedzieć się więcej, [zobacz Tworzenie aplikacji Usługi Azure AD & podmiotu](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)zabezpieczeń usługi w portalu — platforma tożsamości firmy Microsoft.
