---
title: Instalator DKIM w usłudze Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765297"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="71ffc-102">Instalator DKIM w usłudze Office 365</span><span class="sxs-lookup"><span data-stu-id="71ffc-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="71ffc-103">Kompletne instrukcje dotyczące konfigurowania DKIM dla domen niestandardowych w usłudze Office 365 są [tutaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="71ffc-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="71ffc-104">Dla **każdej** domeny niestandardowe należy utworzyć **dwa** rekordy DKIM CNAME w usłudze hostingowej DNS domeny (zazwyczaj rejestratora domen).</span><span class="sxs-lookup"><span data-stu-id="71ffc-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="71ffc-105">Na przykład contoso.com i fourthcoffee.com wymagają cztery rekordy DKIM CNAME: dwa dla domeny contoso.com i dwa dla fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="71ffc-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="71ffc-106">Rekordy DKIM CNAME dla **każdej** domeny niestandardowe użyć następujących formatów:</span><span class="sxs-lookup"><span data-stu-id="71ffc-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="71ffc-107">**Nazwa hosta**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="71ffc-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="71ffc-108">**Wskazuje adres lub wartość**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="71ffc-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="71ffc-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="71ffc-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="71ffc-110">**Nazwa hosta**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="71ffc-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="71ffc-111">**Wskazuje adres lub wartość**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="71ffc-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="71ffc-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="71ffc-112">**TTL**: 3600</span></span>

   <span data-ttu-id="71ffc-113">\<DomainGUID\> tekst z lewej strony jest `.mail.protection.outlook.com` w dostosowanych rekord MX dla domeny niestandardowej (na przykład `contoso-com` dla domeny contoso.com).</span><span class="sxs-lookup"><span data-stu-id="71ffc-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="71ffc-114">\<InitialDomain\> jest domena używana podczas rejestrowania się w usłudze Office 365 (na przykład contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="71ffc-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="71ffc-115">Po utworzeniu rekordy CNAME dla domen niestandardowych, należy wykonać następujące instrukcje:</span><span class="sxs-lookup"><span data-stu-id="71ffc-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="71ffc-116">.</span><span class="sxs-lookup"><span data-stu-id="71ffc-116">a.</span></span> <span data-ttu-id="71ffc-117">[Zaloguj się do usługi Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) , potrzebne do tego będzie Twoje konto służbowe.</span><span class="sxs-lookup"><span data-stu-id="71ffc-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="71ffc-118">b.</span><span class="sxs-lookup"><span data-stu-id="71ffc-118">b.</span></span> <span data-ttu-id="71ffc-119">Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="71ffc-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="71ffc-120">c.</span><span class="sxs-lookup"><span data-stu-id="71ffc-120">c.</span></span> <span data-ttu-id="71ffc-121">W lewym dolnym nawigacji rozwiń **Admin** i wybierz **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="71ffc-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="71ffc-122">d.</span><span class="sxs-lookup"><span data-stu-id="71ffc-122">d.</span></span> <span data-ttu-id="71ffc-123">Przejdź do **ochrony** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="71ffc-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="71ffc-124">e.</span><span class="sxs-lookup"><span data-stu-id="71ffc-124">e.</span></span> <span data-ttu-id="71ffc-125">Wybierz domenę, a następnie wybierz polecenie **Włącz** **znak**wiadomości dla tej domeny z podpisami DKIM.</span><span class="sxs-lookup"><span data-stu-id="71ffc-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="71ffc-126">Powtórz ten krok dla każdej domeny niestandardowej.</span><span class="sxs-lookup"><span data-stu-id="71ffc-126">Repeat this step for each custom domain.</span></span>
