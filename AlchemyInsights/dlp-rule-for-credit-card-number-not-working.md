---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389587"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="54622-102">Problemy dotyczące DLP numery kart kredytowych</span><span class="sxs-lookup"><span data-stu-id="54622-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="54622-103">Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer karty kredytowej** , używając typu informacji poufnych DLP w O365?</span><span class="sxs-lookup"><span data-stu-id="54622-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="54622-104">Jeśli tak, upewnij się, treści zawiera informacje potrzebne do wyzwalania zasad DLP podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="54622-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="54622-105">Na przykład dla **zasad karty kredytowej** skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:</span><span class="sxs-lookup"><span data-stu-id="54622-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="54622-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowany (dddddddddddddddd) i musi pomyślnie przejść test Luhna.</span><span class="sxs-lookup"><span data-stu-id="54622-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="54622-107">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Wzór bardzo złożone i niezawodne, który wykrywa kart z wszystkich głównych marek na świecie, w tym Visa, MasterCard, Discover Card, JCB, American Express, kart upominkowych i karty diner.</span><span class="sxs-lookup"><span data-stu-id="54622-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="54622-108">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna</span><span class="sxs-lookup"><span data-stu-id="54622-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="54622-109">**[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="54622-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="54622-110">Funkcja Func_credit_card znajduje się zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="54622-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="54622-111">Spełniony jest jeden z następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="54622-111">One of the following is true:</span></span>

  - <span data-ttu-id="54622-112">Znajduje słowa kluczowego z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="54622-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="54622-113">Znalezione słowa kluczowego z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="54622-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="54622-114">Funkcja Func_expiration_date znajdzie datę w formacie daty prawo.</span><span class="sxs-lookup"><span data-stu-id="54622-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="54622-115">Przekazuje sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="54622-115">The checksum passes</span></span>

    <span data-ttu-id="54622-116">Na przykład poniższy przykładowy wywołałoby zasad DLP numer karty kredytowej:</span><span class="sxs-lookup"><span data-stu-id="54622-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="54622-117">Wizy: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="54622-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="54622-118">Wygasa: 2/2009</span><span class="sxs-lookup"><span data-stu-id="54622-118">Expires: 2/2009</span></span>

<span data-ttu-id="54622-119">Aby uzyskać więcej informacji na to, co jest wymagany **Numer karty kredytowej** wykryć dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy Poszukaj karty kredytowej #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="54622-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="54622-120">Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="54622-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  