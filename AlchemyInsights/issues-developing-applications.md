---
title: Problemy z tworzeniem aplikacji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974772"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="e5ac0-102">Problemy z tworzeniem aplikacji</span><span class="sxs-lookup"><span data-stu-id="e5ac0-102">Issues developing applications</span></span>

<span data-ttu-id="e5ac0-103">Aby rozwiązać najczęstsze problemy podczas budowania aplikacji usługi Azure Active Directory (AD), zobacz następujące artykuły:</span><span class="sxs-lookup"><span data-stu-id="e5ac0-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="e5ac0-104">Widzę problemy z logowaniem się do aplikacji tylko za pomocą przeglądarki Chrome</span><span class="sxs-lookup"><span data-stu-id="e5ac0-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="e5ac0-105">Nie wiem, jak zmienić ustawienia domyślne okresu ważności tokenu dla mojej aplikacji</span><span class="sxs-lookup"><span data-stu-id="e5ac0-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="e5ac0-106">Nie wiem, jak działa zgoda na stosowanie aplikacji</span><span class="sxs-lookup"><span data-stu-id="e5ac0-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="e5ac0-107">Nie wiem, jak udzielić uprawnień do mojej aplikacji</span><span class="sxs-lookup"><span data-stu-id="e5ac0-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="e5ac0-108">Nie rozumiem różnicy między uprawnieniami delegowanymi i aplikacjami</span><span class="sxs-lookup"><span data-stu-id="e5ac0-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="e5ac0-109">\***Koniec obsługi biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API Azure AD Graph (usługa AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="e5ac0-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="e5ac0-110">Od 30 czerwca 2020 r. nie będziemy już dodawać żadnych nowych funkcji do biblioteki uwierzytelniania usługi Azure Active Directory (ADAL) i interfejsu API usługi Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="e5ac0-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="e5ac0-111">Będziemy nadal dostarczać pomoc techniczną i aktualizacje zabezpieczeń, ale nie będą już udostępniać aktualizacji funkcji.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="e5ac0-112">Począwszy od 30 czerwca 2022 r., zostanie zakończona pomoc techniczna dla wykresu ADAL i AAD, dzięki czemu nie będzie już udzielana pomoc techniczna ani aktualizacje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="e5ac0-113">W wyniku tego warunku obowiązują następujące implikacje:</span><span class="sxs-lookup"><span data-stu-id="e5ac0-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="e5ac0-114">Aplikacje używające biblioteki ADAL w istniejących wersjach systemu operacyjnego będą nadal działać po tym czasie, ale nie będą otrzymywać pomocy technicznej ani aktualizacji zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="e5ac0-115">Aplikacje korzystające z wykresu AAD po upływie tego czasu mogą przestać otrzymywać odpowiedzi z punktu końcowego wykresu w usłudze AAD</span><span class="sxs-lookup"><span data-stu-id="e5ac0-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="e5ac0-116">*Migracja ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="e5ac0-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="e5ac0-117">Jeśli korzystasz z aplikacji firmy Microsoft, Zalecamy zaktualizowanie biblioteki uwierzytelniania firmy Microsoft (MSAL), która ma najnowsze funkcje i aktualizacje zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="e5ac0-118">To zalecenie jest w kontekście firmy Microsoft inicjującej proces migrowania swoich aplikacji do MSAL przed upływem nieprzekraczalnego terminu na koniec obsługi.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="e5ac0-119">Migracja przez firmę Microsoft jej aplikacji na MSAL zapewnia, że aplikacje korzystają z bieżących udoskonaleń zabezpieczeń i funkcji usługi MSAL.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="e5ac0-120">Przeczytaj sekcję ADAL często zadawane pytania</span><span class="sxs-lookup"><span data-stu-id="e5ac0-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="e5ac0-121">Dowiedz się, jak przeprowadzić migrację aplikacji na poszczególnych platformach</span><span class="sxs-lookup"><span data-stu-id="e5ac0-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="e5ac0-122">Jeśli potrzebujesz pomocy w zrozumieniu, które aplikacje używają biblioteki ADAL, zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i, jeśli to konieczne, dotarcie do wszystkich niezależnych dostawców oprogramowania (ISV) lub dostawców aplikacji.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="e5ac0-123">Pomoc techniczna firmy Microsoft może również udostępnić listę wszystkich aplikacji innych niż Microsoft ADAL w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="e5ac0-124">**Migracja wykresu w usłudze AAD**</span><span class="sxs-lookup"><span data-stu-id="e5ac0-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="e5ac0-125">W przypadku aplikacji korzystających z programu obsługi wykresów w usłudze AAD postępuj zgodnie z naszymi wskazówkami, aby przeprowadzić migrację aplikacji Graph</span><span class="sxs-lookup"><span data-stu-id="e5ac0-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="e5ac0-126">[Lista kontrolna migracji zawiera punkt wprowadzenia](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="e5ac0-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="e5ac0-127">Portal rejestracji aplikacji platformy Azure pokazuje, które aplikacje używają wykresu w usłudze AAD.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="e5ac0-128">Zalecamy przejrzenie wszystkich kodów źródłowych aplikacji i, jeśli to konieczne, do wszystkich niezależnych dostawców oprogramowania (ISV) lub dostawców aplikacji.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="e5ac0-129">Pomoc techniczna firmy Microsoft może także dostarczyć informacji na temat użycia wykresu w usłudze AAD w dzierżawie.</span><span class="sxs-lookup"><span data-stu-id="e5ac0-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







