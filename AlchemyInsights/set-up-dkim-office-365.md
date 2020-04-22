---
title: Konfiguracja DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645682"
---
# <a name="setup-dkim"></a><span data-ttu-id="27615-102">Konfiguracja DKIM</span><span class="sxs-lookup"><span data-stu-id="27615-102">Setup DKIM</span></span>

<span data-ttu-id="27615-103">Pełne instrukcje konfigurowania DKIM dla domen niestandardowych w usłudze Microsoft 365 znajdują [się tutaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="27615-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="27615-104">Dla **każdej** domeny niestandardowej należy utworzyć **dwa** rekordy CNAME DKIM w usłudze hostingu DNS domeny (zazwyczaj rejestratora domen).</span><span class="sxs-lookup"><span data-stu-id="27615-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="27615-105">Na przykład contoso.com i fourthcoffee.com wymagać czterech rekordów CNAME DKIM: dwóch dla contoso.com i dwóch dla fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="27615-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="27615-106">Rekordy CNAME DKIM dla **każdej** domeny niestandardowej używają następujących formatów:</span><span class="sxs-lookup"><span data-stu-id="27615-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="27615-107">**Nazwa hosta**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="27615-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="27615-108">**Wskazuje na adres lub wartość:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="27615-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="27615-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="27615-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="27615-110">**Nazwa hosta**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="27615-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="27615-111">**Wskazuje na adres lub wartość:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="27615-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="27615-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="27615-112">**TTL**: 3600</span></span>

   <span data-ttu-id="27615-113">\<DomainGUID\> to tekst znajdujący `.mail.protection.outlook.com` się po lewej stronie w dostosowanym rekordzie MX dla domeny niestandardowej (na przykład `contoso-com` dla domeny contoso.com).</span><span class="sxs-lookup"><span data-stu-id="27615-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="27615-114">\<InitialDomain\> to domena używana podczas konfigurowania usługi Microsoft 365 (na przykład contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="27615-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="27615-115">Po utworzeniu rekordów CNAME dla domen niestandardowych wykonaj następujące instrukcje:</span><span class="sxs-lookup"><span data-stu-id="27615-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="27615-116">A.</span><span class="sxs-lookup"><span data-stu-id="27615-116">a.</span></span> <span data-ttu-id="27615-117">[zaloguj się do usługi Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) za pomocą konta służbowego.</span><span class="sxs-lookup"><span data-stu-id="27615-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="27615-118">B.</span><span class="sxs-lookup"><span data-stu-id="27615-118">b.</span></span> <span data-ttu-id="27615-119">Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="27615-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="27615-120">C.</span><span class="sxs-lookup"><span data-stu-id="27615-120">c.</span></span> <span data-ttu-id="27615-121">W lewym dolnym lewym przycisku nawigacji rozwiń pozycję **Administrator** i wybierz pozycję **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="27615-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="27615-122">D.</span><span class="sxs-lookup"><span data-stu-id="27615-122">d.</span></span> <span data-ttu-id="27615-123">Przejdź do **ochrony** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="27615-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="27615-124">E.</span><span class="sxs-lookup"><span data-stu-id="27615-124">e.</span></span> <span data-ttu-id="27615-125">Wybierz domenę, a następnie wybierz pozycję **Włącz** dla **sygnatariuszy wiadomości dla tej domeny z podpisami DKIM**.</span><span class="sxs-lookup"><span data-stu-id="27615-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="27615-126">Powtórz ten krok dla każdej domeny niestandardowej.</span><span class="sxs-lookup"><span data-stu-id="27615-126">Repeat this step for each custom domain.</span></span>
