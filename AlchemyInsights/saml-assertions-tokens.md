---
title: Potwierdzenia SAML (tokeny)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885671"
---
# <a name="saml-assertions-tokens"></a>Potwierdzenia SAML (tokeny)

1. Tokeny SAML (Security Assertions Markup Language) są reprezentacją XML oświadczeń. Domyślnie wystawione są tokeny w scenariuszach zabezpieczeń federacyjnych korzystające z tokenów SAML (WCF). Aby uzyskać więcej informacji, zobacz informacje o [tokenach i oświadczeniach protokołu SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Platforma Microsoft Identity platform emituje różne typy tokenów zabezpieczających podczas przetwarzania każdego przepływu uwierzytelniania. [Informacje dotyczące oświadczeń tokenów SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) zawiera opis formatu, charakterystyki zabezpieczeń i zawartości tokenów SAML 2,0.
3. Postępuj zgodnie z instrukcjami dotyczącymi [konfigurowalnych okresów ważności tokenów na platformie Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , aby zrozumieć, jak skonfigurować okresy ważności tokenu.
4. Postępuj zgodnie z instrukcjami przedstawionymi w [tym artykule](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , aby dowiedzieć się, jak skonfigurować szyfrowanie TOKENów SAML usługi Azure AD.
5. W usłudze Azure AD możesz skonfigurować opcje podpisywania certyfikatu i algorytm podpisywania certyfikatu. Aby uzyskać więcej informacji, zobacz [Zaawansowane opcje podpisywania certyfikatu w aplikacjach w obszarze token SAML dla aplikacji Galeria w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
