---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685608"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="45fd8-102">Blokowanie starszego uwierzytelniania</span><span class="sxs-lookup"><span data-stu-id="45fd8-102">Blocking legacy authentication</span></span>

<span data-ttu-id="45fd8-103">Starsze uwierzytelnianie to termin, który odwołuje się do żądania uwierzytelnienia wprowadzonego przez:</span><span class="sxs-lookup"><span data-stu-id="45fd8-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="45fd8-104">Starsi klienci pakietu Office, którzy nie używają nowoczesnego uwierzytelniania (na przykład klient pakietu Office 2010).</span><span class="sxs-lookup"><span data-stu-id="45fd8-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="45fd8-105">Dowolny klient korzystający ze starszych protokołów pocztowych, takich jak IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="45fd8-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="45fd8-106">Aby uzyskać więcej informacji na temat blokowania starszych uwierzytelnień i włączania nowoczesnego uwierzytelniania, zobacz [blokowanie starszych wersji uwierzytelniania](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="45fd8-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="45fd8-107">Domyślne ustawienia zabezpieczeń w usłudze Azure Active Directory (Azure AD) ułatwiają Zabezpieczanie organizacji i pomaganie w niej.</span><span class="sxs-lookup"><span data-stu-id="45fd8-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="45fd8-108">Ustawienia domyślne zabezpieczeń zawierają wstępnie skonfigurowane ustawienia zabezpieczeń do typowych ataków.</span><span class="sxs-lookup"><span data-stu-id="45fd8-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="45fd8-109">Aby uzyskać więcej informacji na temat domyślnych ustawień zabezpieczeń, zobacz [co to są domyślne zabezpieczenia?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="45fd8-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="45fd8-110">**Uwaga**: Jeśli Twoja dzierżawa została utworzona w dniu lub po 22 października 2019, być może używasz nowego zachowania zabezpieczeń domyślnych i masz już włączone domyślne ustawienia zabezpieczeń w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="45fd8-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="45fd8-111">W celu ochrony wszystkich naszych użytkowników domyślne ustawienia zabezpieczeń są uwzględniane we wszystkich nowych dzierżawach, które zostały utworzone.</span><span class="sxs-lookup"><span data-stu-id="45fd8-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
