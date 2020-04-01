---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079270"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="caad3-102">Blokowanie uwierzytelniania starszego</span><span class="sxs-lookup"><span data-stu-id="caad3-102">Blocking legacy authentication</span></span>

<span data-ttu-id="caad3-103">Uwierzytelnianie starsze to termin, który odnosi się do żądania uwierzytelnienia złożonego przez:</span><span class="sxs-lookup"><span data-stu-id="caad3-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="caad3-104">Starsi klienci pakietu Office, którzy nie korzystają z nowoczesnego uwierzytelniania (na przykład klient pakietu Office 2010).</span><span class="sxs-lookup"><span data-stu-id="caad3-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="caad3-105">Każdy klient, który używa starszych protokołów poczty, takich jak IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="caad3-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="caad3-106">Aby uzyskać więcej informacji na temat blokowania uwierzytelniania starszego i włączania nowoczesnego uwierzytelniania, zobacz [Blokowanie uwierzytelniania starszego](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="caad3-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="caad3-107">Domyślne zabezpieczenia w usłudze Azure Active Directory (Azure AD) ułatwiają bezpieczeństwo i pomagają chronić organizację.</span><span class="sxs-lookup"><span data-stu-id="caad3-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="caad3-108">Domyślne zabezpieczenia zawierają wstępnie skonfigurowane ustawienia zabezpieczeń dla typowych ataków.</span><span class="sxs-lookup"><span data-stu-id="caad3-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="caad3-109">Aby uzyskać więcej informacji na temat wartości domyślnych zabezpieczeń, zobacz [Co to są domyślne zabezpieczenia?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="caad3-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="caad3-110">**Uwaga:** Jeśli dzierżawa została utworzona w dniu lub po 22 października 2019 r., możliwe, że występują nowe zachowanie domyślne zabezpieczeń i już mają włączone ustawienia domyślne zabezpieczeń w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="caad3-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="caad3-111">Aby chronić wszystkich naszych użytkowników, domyślne zabezpieczenia są wdrażane dla wszystkich nowych utworzonych dzierżaw.</span><span class="sxs-lookup"><span data-stu-id="caad3-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
