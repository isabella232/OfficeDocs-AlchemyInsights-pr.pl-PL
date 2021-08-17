---
title: Asertycy SAML (tokeny)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109250"
---
# <a name="saml-assertions-tokens"></a>Asertycy SAML (tokeny)

1. Tokeny języka adupcji zabezpieczeń (SAML, Security Assertions Markup Language) to reprezentacji roszczeń XML. Domyślnie tokeny SAML używane przez Windows Communication Foundation (WCF) w federowanych scenariuszach zabezpieczeń są wystawiane tokenami. Aby uzyskać więcej informacji, zobacz [Tokeny SAML i roszczenia.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)
2. Ten Platforma tożsamości Microsoft w przetwarzaniu każdego przepływu uwierzytelniania emituje kilka typów tokenów zabezpieczających. [Odwołanie do roszczeń tokenu SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) opisuje format, cechy zabezpieczeń i zawartość tokenów SAML 2.0.
3. Postępuj zgodnie z [wskazówkami w tece Konfigurowanie okresów istnienia tokenu w programie Platforma tożsamości Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) aby dowiedzieć się, jak skonfigurować okresy istnienia tokenu.
4. Wykonaj czynności opisane w tym [artykule,](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) aby dowiedzieć się, jak skonfigurować szyfrowanie tokenu SAML usługi Azure AD.
5. W usłudze Azure AD możesz skonfigurować opcje podpisywania certyfikatów oraz algorytm podpisywania certyfikatu. Aby uzyskać więcej informacji, zobacz Zaawansowane opcje [podpisywania certyfikatów w tokenie SAML dla aplikacji galerii w programie Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)
