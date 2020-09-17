---
title: Konfiguracja DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808717"
---
# <a name="setup-dkim"></a><span data-ttu-id="c0a79-102">Konfiguracja DKIM</span><span class="sxs-lookup"><span data-stu-id="c0a79-102">Setup DKIM</span></span>

<span data-ttu-id="c0a79-103">Pełne instrukcje dotyczące konfigurowania DKIM dla domen niestandardowych w programie Microsoft [365 są dostępne](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="c0a79-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="c0a79-104">W przypadku **każdej** domeny niestandardowej trzeba utworzyć **dwa** DKIM rekordy CNAME w usłudze hostingu DNS domeny (zazwyczaj rejestrator domen).</span><span class="sxs-lookup"><span data-stu-id="c0a79-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="c0a79-105">Na przykład contoso.com i fourthcoffee.com wymaga czterech DKIM rekordów CNAME: dwóch dla contoso.com i dwóch dla fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="c0a79-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="c0a79-106">W rekordach CNAME DKIM dla **każdej** domeny niestandardowej zastosowano następujące formaty:</span><span class="sxs-lookup"><span data-stu-id="c0a79-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="c0a79-107">**Nazwa hosta**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c0a79-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c0a79-108">**Wskazuje adres lub wartość**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c0a79-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c0a79-109">**Czas wygaśnięcia**: 3600</span><span class="sxs-lookup"><span data-stu-id="c0a79-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="c0a79-110">**Nazwa hosta**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="c0a79-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="c0a79-111">**Wskazuje adres lub wartość**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="c0a79-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="c0a79-112">**Czas wygaśnięcia**: 3600</span><span class="sxs-lookup"><span data-stu-id="c0a79-112">**TTL**: 3600</span></span>

   <span data-ttu-id="c0a79-113">\<DomainGUID\> jest tekstem po lewej stronie `.mail.protection.outlook.com` dostosowanego rekordu MX dla domeny niestandardowej (na przykład `contoso-com` dla contoso.com domeny).</span><span class="sxs-lookup"><span data-stu-id="c0a79-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="c0a79-114">\<InitialDomain\> jest domeną używaną podczas tworzenia konta w usłudze Microsoft 365 (na przykład contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="c0a79-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="c0a79-115">Po utworzeniu rekordów CNAME dla domen niestandardowych wykonaj następujące instrukcje:</span><span class="sxs-lookup"><span data-stu-id="c0a79-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="c0a79-116">a.</span><span class="sxs-lookup"><span data-stu-id="c0a79-116">a.</span></span> <span data-ttu-id="c0a79-117">[Zaloguj się do usługi Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) za pomocą konta służbowego lub szkolnego.</span><span class="sxs-lookup"><span data-stu-id="c0a79-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="c0a79-118">b.</span><span class="sxs-lookup"><span data-stu-id="c0a79-118">b.</span></span> <span data-ttu-id="c0a79-119">Wybierz ikonę Uruchamianie aplikacji w lewym górnym rogu i wybierz pozycję **Administrator**.</span><span class="sxs-lookup"><span data-stu-id="c0a79-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="c0a79-120">c.</span><span class="sxs-lookup"><span data-stu-id="c0a79-120">c.</span></span> <span data-ttu-id="c0a79-121">W lewym dolnym okienku nawigacji rozwiń pozycję **administrator** i wybierz pozycję **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c0a79-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="c0a79-122">d.</span><span class="sxs-lookup"><span data-stu-id="c0a79-122">d.</span></span> <span data-ttu-id="c0a79-123">Przejdź na stronę **Ochrona**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="c0a79-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="c0a79-124">e.</span><span class="sxs-lookup"><span data-stu-id="c0a79-124">e.</span></span> <span data-ttu-id="c0a79-125">Wybierz domenę, a następnie wybierz pozycję **Włącz** dla **podpisywania wiadomości dla tej domeny z podpisami DKIM**.</span><span class="sxs-lookup"><span data-stu-id="c0a79-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="c0a79-126">Powtórz ten krok dla każdej domeny niestandardowej.</span><span class="sxs-lookup"><span data-stu-id="c0a79-126">Repeat this step for each custom domain.</span></span>
