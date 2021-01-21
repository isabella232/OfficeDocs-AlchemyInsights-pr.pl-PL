---
title: Konfigurowanie i rozszerzanie okresów ważności tokenów
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917007"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="44661-102">Konfigurowanie i rozszerzanie okresów ważności tokenów</span><span class="sxs-lookup"><span data-stu-id="44661-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="44661-103">Możesz określić okres istnienia tokenu dostępu, SAML lub identyfikatora wystawionego przez platformę Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="44661-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="44661-104">Możesz ustawić okresy ważności tokenów dla wszystkich aplikacji w organizacji, dla aplikacji z wieloma dzierżawami (wielu organizacji) lub dla określonego podmiotu zabezpieczeń usługi w organizacji.</span><span class="sxs-lookup"><span data-stu-id="44661-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="44661-105">Aby uzyskać więcej informacji, zobacz [konfigurowalne okresy ważności tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="44661-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="44661-106">Przykłady można znaleźć w artykule [Przykłady sposobu konfigurowania okresów ważności tokenu](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="44661-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="44661-107">Aby dowiedzieć się, jak skonfigurować okres istnienia i zgodność tokenów w usłudze Azure Active Directory B2C (Azure AD B2C), zobacz [Konfigurowanie tokenów w usłudze Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="44661-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="44661-108">Artykuł [Konfigurowanie zachowania sesji w usłudze Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) zawiera opis metod logowania jednokrotnego (SSO) używanych w usłudze Azure AD B2C i pomaga w wyborze najbardziej odpowiedniej metody rejestracji jednokrotnej podczas konfigurowania zasad.</span><span class="sxs-lookup"><span data-stu-id="44661-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="44661-109">**Jak długo mają być tokeny? Jak długo są ważne?**</span><span class="sxs-lookup"><span data-stu-id="44661-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="44661-110">Okres ważności tokenu to 1 godzina, a okres istnienia sesji to 24 godziny.</span><span class="sxs-lookup"><span data-stu-id="44661-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="44661-111">Oznacza to, że jeśli nie przeprowadzono żadnych żądań w ciągu 24 godzin, musisz zalogować się ponownie przed żądaniem nowego tokenu.</span><span class="sxs-lookup"><span data-stu-id="44661-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="44661-112">Po 30 maja 2020, żadna Nowa dzierżawa nie będzie mogła korzystać z zasad konfiguracji okresu istnienia konfiguracji w celu konfigurowania tokenów sesji i odświeżania.</span><span class="sxs-lookup"><span data-stu-id="44661-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="44661-113">Rezygnacja będzie obowiązywać w ciągu kilku miesięcy, co oznacza, że będziemy przetrzymywać przestrzeganie istniejących zasad dotyczących tokenów sesji i odświeżania.</span><span class="sxs-lookup"><span data-stu-id="44661-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="44661-114">Możesz nadal konfigurować okresy ważności tokenów dostępu po zaniechaniu.</span><span class="sxs-lookup"><span data-stu-id="44661-114">You can still configure access token lifetimes after the deprecation.</span></span>






