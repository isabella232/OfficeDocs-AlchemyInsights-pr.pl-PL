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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="76e6c-102">Potwierdzenia SAML (tokeny)</span><span class="sxs-lookup"><span data-stu-id="76e6c-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="76e6c-103">Tokeny SAML (Security Assertions Markup Language) są reprezentacją XML oświadczeń.</span><span class="sxs-lookup"><span data-stu-id="76e6c-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="76e6c-104">Domyślnie wystawione są tokeny w scenariuszach zabezpieczeń federacyjnych korzystające z tokenów SAML (WCF).</span><span class="sxs-lookup"><span data-stu-id="76e6c-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="76e6c-105">Aby uzyskać więcej informacji, zobacz informacje o [tokenach i oświadczeniach protokołu SAML](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="76e6c-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="76e6c-106">Platforma Microsoft Identity platform emituje różne typy tokenów zabezpieczających podczas przetwarzania każdego przepływu uwierzytelniania.</span><span class="sxs-lookup"><span data-stu-id="76e6c-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="76e6c-107">[Informacje dotyczące oświadczeń tokenów SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) zawiera opis formatu, charakterystyki zabezpieczeń i zawartości tokenów SAML 2,0.</span><span class="sxs-lookup"><span data-stu-id="76e6c-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="76e6c-108">Postępuj zgodnie z instrukcjami dotyczącymi [konfigurowalnych okresów ważności tokenów na platformie Microsoft Identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) , aby zrozumieć, jak skonfigurować okresy ważności tokenu.</span><span class="sxs-lookup"><span data-stu-id="76e6c-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="76e6c-109">Postępuj zgodnie z instrukcjami przedstawionymi w [tym artykule](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , aby dowiedzieć się, jak skonfigurować szyfrowanie TOKENów SAML usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="76e6c-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="76e6c-110">W usłudze Azure AD możesz skonfigurować opcje podpisywania certyfikatu i algorytm podpisywania certyfikatu.</span><span class="sxs-lookup"><span data-stu-id="76e6c-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="76e6c-111">Aby uzyskać więcej informacji, zobacz [Zaawansowane opcje podpisywania certyfikatu w aplikacjach w obszarze token SAML dla aplikacji Galeria w usłudze Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="76e6c-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
