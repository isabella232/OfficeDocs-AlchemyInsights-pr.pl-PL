---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304144"
---
<span data-ttu-id="fa54a-p101">Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer karty kredytowej** , używając typu informacji poufnych DLP w O365? Jeśli tak, upewnij się, treści zawiera informacje potrzebne do wyzwalania zasad DLP podczas szacowania. Na przykład dla **zasad karty kredytowej** skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:</span><span class="sxs-lookup"><span data-stu-id="fa54a-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="fa54a-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowany (dddddddddddddddd) i musi pomyślnie przejść test Luhna.</span><span class="sxs-lookup"><span data-stu-id="fa54a-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="fa54a-106">**[Wzór:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Wzór bardzo złożone i niezawodne, który wykrywa kart z wszystkich głównych marek na świecie, w tym Visa, Mastercard, Discover Card, JCB, American Express, kart upominkowych i karty diner.</span><span class="sxs-lookup"><span data-stu-id="fa54a-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="fa54a-107">**[Suma kontrolna:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna</span><span class="sxs-lookup"><span data-stu-id="fa54a-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="fa54a-108">**[Definicji:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="fa54a-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="fa54a-109">Funkcja Func_credit_card znajduje się zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="fa54a-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="fa54a-110">Spełniony jest jeden z następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="fa54a-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="fa54a-111">Znajduje słowa kluczowego z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="fa54a-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="fa54a-112">Znalezione słowa kluczowego z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="fa54a-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="fa54a-113">Funkcja Func_expiration_date znajdzie datę w formacie daty prawo.</span><span class="sxs-lookup"><span data-stu-id="fa54a-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="fa54a-114">Przekazuje sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="fa54a-114">The checksum passes</span></span>
    
    <span data-ttu-id="fa54a-115">Na przykład poniższy przykładowy wywołałoby zasad DLP numer karty kredytowej:</span><span class="sxs-lookup"><span data-stu-id="fa54a-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="fa54a-116">Wizy: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="fa54a-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="fa54a-117">Wygasa: 2/2009</span><span class="sxs-lookup"><span data-stu-id="fa54a-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="fa54a-118">Aby uzyskać więcej informacji na to, co jest wymagany **Numer karty kredytowej** wykryć dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy Poszukaj karty kredytowej #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="fa54a-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="fa54a-119">Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fa54a-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

