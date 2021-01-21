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
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurowanie i rozszerzanie okresów ważności tokenów

Możesz określić okres istnienia tokenu dostępu, SAML lub identyfikatora wystawionego przez platformę Microsoft Identity. Możesz ustawić okresy ważności tokenów dla wszystkich aplikacji w organizacji, dla aplikacji z wieloma dzierżawami (wielu organizacji) lub dla określonego podmiotu zabezpieczeń usługi w organizacji. Aby uzyskać więcej informacji, zobacz [konfigurowalne okresy ważności tokenu](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Przykłady można znaleźć w artykule [Przykłady sposobu konfigurowania okresów ważności tokenu](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Aby dowiedzieć się, jak skonfigurować okres istnienia i zgodność tokenów w usłudze Azure Active Directory B2C (Azure AD B2C), zobacz [Konfigurowanie tokenów w usłudze Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Artykuł [Konfigurowanie zachowania sesji w usłudze Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) zawiera opis metod logowania jednokrotnego (SSO) używanych w usłudze Azure AD B2C i pomaga w wyborze najbardziej odpowiedniej metody rejestracji jednokrotnej podczas konfigurowania zasad.

**Jak długo mają być tokeny? Jak długo są ważne?**

Okres ważności tokenu to 1 godzina, a okres istnienia sesji to 24 godziny. Oznacza to, że jeśli nie przeprowadzono żadnych żądań w ciągu 24 godzin, musisz zalogować się ponownie przed żądaniem nowego tokenu.

> [!NOTE]
> Po 30 maja 2020, żadna Nowa dzierżawa nie będzie mogła korzystać z zasad konfiguracji okresu istnienia konfiguracji w celu konfigurowania tokenów sesji i odświeżania. Rezygnacja będzie obowiązywać w ciągu kilku miesięcy, co oznacza, że będziemy przetrzymywać przestrzeganie istniejących zasad dotyczących tokenów sesji i odświeżania. Możesz nadal konfigurować okresy ważności tokenów dostępu po zaniechaniu.






