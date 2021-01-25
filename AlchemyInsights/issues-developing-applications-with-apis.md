---
title: Problemy z tworzeniem aplikacji przy użyciu interfejsów API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975013"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="0a1f6-102">Problemy z tworzeniem aplikacji przy użyciu interfejsów API</span><span class="sxs-lookup"><span data-stu-id="0a1f6-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="0a1f6-103">Aby rozpocząć korzystanie z interfejsu API Graph w usłudze Azure Active Directory, zobacz [Przewodnik Szybki Start dla interfejsu API Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) lub wyświetlanie [dokumentacji referencyjnej interfejsu API programu Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="0a1f6-104">**Koniec obsługi biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API Azure AD Graph (usługa AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="0a1f6-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="0a1f6-105">**Od 30 czerwca 2020** r. nie będziemy już dodawać żadnych nowych funkcji do wykresu ADAL i Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="0a1f6-106">Będziemy nadal dostarczać pomoc techniczną i aktualizacje zabezpieczeń, ale nie będą już udostępniać aktualizacji funkcji.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="0a1f6-107">**Począwszy od 30 czerwca 2022** r., zostanie zakończona pomoc techniczna dla wykresu ADAL i Azure AD i nie będzie już udzielana pomoc techniczna ani aktualizacje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="0a1f6-108">Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymywać pomocy technicznej ani aktualizacji zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="0a1f6-109">Aplikacje korzystające z programu Azure AD Graph już po upływie tego czasu nie możesz już odbierać odpowiedzi z punktu końcowego wykresu usługi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="0a1f6-110">**Migracja biblioteki ADAL**</span><span class="sxs-lookup"><span data-stu-id="0a1f6-110">**ADAL Migration**</span></span>

<span data-ttu-id="0a1f6-111">Zalecamy aktualizację do [biblioteki uwierzytelniania firmy Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), która ma najnowsze funkcje i aktualizacje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="0a1f6-112">Jeśli korzystasz z aplikacji firmy Microsoft, sprawdź, czy firma Microsoft jest w trakcie migrowania swoich aplikacji do MSAL przez ostateczny nieprzekraczalny termin, dzięki którym będą mogli korzystać z MSAL bieżących zabezpieczeń i funkcji.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="0a1f6-113">[Przeczytaj często zadawane pytania dotyczące biblioteki ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="0a1f6-114">[Dowiedz się, jak przeprowadzić migrację aplikacji na poszczególnych platformach](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="0a1f6-115">Jeśli potrzebujesz pomocy dotyczącej korzystania z aplikacji ADAL, zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i w razie potrzeby skontaktowanie się z dostawcami ISV lub aplikacjami.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0a1f6-116">Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich aplikacji innych niż Microsoft ADAL w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="0a1f6-117">**Migracja wykresu w usłudze AAD**</span><span class="sxs-lookup"><span data-stu-id="0a1f6-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="0a1f6-118">W przypadku aplikacji korzystających z usługi Azure AD Graph postępuj zgodnie z naszymi wskazówkami, aby przeprowadzić migrację [aplikacji Azure AD Graph do programu Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="0a1f6-119">[Lista kontrolna migracji zawiera punkt wprowadzenia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="0a1f6-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="0a1f6-120">Portal rejestracji aplikacji platformy Azure pokazuje, które aplikacje używają wykresu w usłudze AAD.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="0a1f6-121">Zalecamy przejrzenie wszystkich kodów źródłowych aplikacji, a w razie potrzeby skontaktowanie się z dostawcami ISV lub aplikacjami.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="0a1f6-122">Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich zastosowań wykresów w usłudze AAD w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="0a1f6-123">Aby aplikacja miała dostęp do danych w programie Microsoft Graph, użytkownik lub administrator musi udzielić mu odpowiednich uprawnień za pośrednictwem procesu wyrażania zgody.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="0a1f6-124">Informacje o uprawnieniach [programu Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) zawiera listę uprawnień skojarzonych z poszczególnymi zestawami interfejsów API programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="0a1f6-125">Zawiera również wskazówki dotyczące korzystania z tych uprawnień.</span><span class="sxs-lookup"><span data-stu-id="0a1f6-125">It also provides guidance about how to use the permissions.</span></span>
