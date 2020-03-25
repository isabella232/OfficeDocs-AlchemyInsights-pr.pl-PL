---
title: Reguła DLP dla SSN nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932545"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="c6696-102">Problemy Z DLP z numerami ubezpieczenia społecznego</span><span class="sxs-lookup"><span data-stu-id="c6696-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="c6696-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="c6696-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c6696-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="c6696-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c6696-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="c6696-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c6696-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="c6696-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c6696-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="c6696-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c6696-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="c6696-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c6696-109">**Problemy z DLP z sieciami SSN**</span><span class="sxs-lookup"><span data-stu-id="c6696-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="c6696-110">Czy występują problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer ubezpieczenia społecznego (SSN)** podczas korzystania z typu poufnych informacji w usłudze Office 365?</span><span class="sxs-lookup"><span data-stu-id="c6696-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="c6696-111">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP.</span><span class="sxs-lookup"><span data-stu-id="c6696-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="c6696-112">Na przykład dla zasad SSN skonfigurowanych z poziomem ufności 85%, następujące są oceniane i muszą zostać wykryte, aby reguła wyzwoliła:</span><span class="sxs-lookup"><span data-stu-id="c6696-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c6696-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cyfr, które mogą znajdować się w sformatowanym lub niesformatowanym wzorze</span><span class="sxs-lookup"><span data-stu-id="c6696-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="c6696-114">**[Wzór:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje wyszukuje sieci SSN w czterech różnych wzorcach:</span><span class="sxs-lookup"><span data-stu-id="c6696-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="c6696-115">Func_ssn wyszukuje sieci SSN z silnym formatowaniem sprzed 2011 r., sformatowanym z myślnikami lub spacjami (ddd-dddd LUB ddd dd ddd dddd)</span><span class="sxs-lookup"><span data-stu-id="c6696-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c6696-116">Func_unformatted_ssn wyszukuje sieci SSN z silnym formatowaniem sprzed 2011 r., które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c6696-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="c6696-117">Func_randomized_formatted_ssn znajdzie sieci SSN po 2011 r., które są sformatowane myślnikami lub spacjami (ddd-ddd-ddd ddd ddddd)</span><span class="sxs-lookup"><span data-stu-id="c6696-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c6696-118">Func_randomized_unformatted_ssn znajduje sieci SSN po 2011 r., które są niesformatowane jako dziewięć kolejnych cyfr (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c6696-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="c6696-119">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie ma sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="c6696-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="c6696-120">**[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Zasady DLP są w 85% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="c6696-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c6696-121">[Funkcja Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) znajduje zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="c6696-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c6696-122">Zostanie znalezione słowo kluczowe z [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="c6696-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="c6696-123">Przykłady słów kluczowych obejmują: *Social Security, Social Security#, Soc Sec , SSN* .</span><span class="sxs-lookup"><span data-stu-id="c6696-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="c6696-124">Na przykład następujący przykład może wyzwolić dla zasad DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="c6696-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="c6696-125">Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrywania sieci SSN dla zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają w sieci SSNS](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="c6696-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="c6696-126">Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c6696-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  