---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820188"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="5baa5-102">Blokowanie starszego uwierzytelniania</span><span class="sxs-lookup"><span data-stu-id="5baa5-102">Blocking legacy authentication</span></span>

<span data-ttu-id="5baa5-103">Starsze uwierzytelnianie to termin, który odwołuje się do żądania uwierzytelnienia dokonanego przez:</span><span class="sxs-lookup"><span data-stu-id="5baa5-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="5baa5-104">Starsi klienci pakietu Office, którzy nie używają nowoczesnego uwierzytelniania (na przykład klienta pakietu Office 2010).</span><span class="sxs-lookup"><span data-stu-id="5baa5-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="5baa5-105">Każdy klient, który korzysta ze starszych protokołów poczty, takich jak IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="5baa5-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="5baa5-106">Aby uzyskać więcej informacji na temat blokowania starszego uwierzytelniania i włączania nowoczesnego uwierzytelniania, zobacz Blokowanie [starszego uwierzytelniania.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="5baa5-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="5baa5-107">Domyślne ustawienia zabezpieczeń w usłudze Azure Active Directory (Azure AD) ułatwiają zabezpieczanie i ochronę organizacji.</span><span class="sxs-lookup"><span data-stu-id="5baa5-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="5baa5-108">Wartości domyślne zabezpieczeń zawierają wstępnie skonfigurowane ustawienia zabezpieczeń dla typowych ataków.</span><span class="sxs-lookup"><span data-stu-id="5baa5-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="5baa5-109">Aby uzyskać więcej informacji o ustawieniach domyślnych zabezpieczeń, zobacz Co [to są ustawienia domyślne zabezpieczeń?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="5baa5-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="5baa5-110">**Uwaga:** Jeśli dzierżawa została utworzona 22 października 2019 r. lub później, możliwe, że w Twojej dzierżawie włączono nowe zachowanie bezpieczne i domyślne ustawienia domyślne zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="5baa5-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="5baa5-111">W celu ochrony wszystkich naszych użytkowników są publikowane domyślne ustawienia zabezpieczeń we wszystkich nowo tworzonach dzierżawach.</span><span class="sxs-lookup"><span data-stu-id="5baa5-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
