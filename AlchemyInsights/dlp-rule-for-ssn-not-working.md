---
title: Reguła DLP dla numeru PESEL nie działa
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
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389443"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="6a88a-102">DLP problemów z numery ubezpieczenia społecznego</span><span class="sxs-lookup"><span data-stu-id="6a88a-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="6a88a-103">Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer PESEL (SSN)** podczas używania typu informacji poufnych w usłudze Office 365?</span><span class="sxs-lookup"><span data-stu-id="6a88a-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="6a88a-104">Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne dla czego szuka zasad DLP.</span><span class="sxs-lookup"><span data-stu-id="6a88a-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="6a88a-105">Na przykład polityki SSN skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:</span><span class="sxs-lookup"><span data-stu-id="6a88a-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6a88a-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cyfr, które mogą być we wzorcu sformatowaną lub niesformatowaną</span><span class="sxs-lookup"><span data-stu-id="6a88a-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="6a88a-107">**[Wzór:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje szukać SSNs w czterech różnych wzorów:</span><span class="sxs-lookup"><span data-stu-id="6a88a-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="6a88a-108">Func_ssn znajdzie SSNs z pre-2011 silne formatowania, które są sformatowane za pomocą kresek ani spacji (ddd-dd-dddd lub ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="6a88a-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6a88a-109">Func_unformatted_ssn znajdzie SSNs z pre-2011 silne formatowania, które są formatowane jako dziewięciu następujących po sobie cyfr (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="6a88a-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="6a88a-110">Func_randomized_formatted_ssn znajdzie SSNs post-2011, które są sformatowane za pomocą kresek ani spacji (ddd-dd-dddd lub ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="6a88a-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="6a88a-111">Func_randomized_unformatted_ssn znajdzie SSNs post-2011, które są formatowane jako dziewięciu następujących po sobie cyfr (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="6a88a-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="6a88a-112">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie ma żadnych suma kontrolna</span><span class="sxs-lookup"><span data-stu-id="6a88a-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="6a88a-113">**[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="6a88a-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6a88a-114">[Funkcja Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) znajduje się zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="6a88a-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6a88a-115">Znajduje słowa kluczowego z [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="6a88a-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="6a88a-116">Zawiera przykłady słów kluczowych: *zabezpieczenia społecznego, zabezpieczenia społecznego #, s Soc, numer PESEL* .</span><span class="sxs-lookup"><span data-stu-id="6a88a-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="6a88a-117">Na przykład poniższy przykładowy wywołałoby zasad DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="6a88a-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="6a88a-118">Aby uzyskać więcej informacji na co jest wymagane dla SSNs do wykrycia dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy szukać SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="6a88a-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="6a88a-119">Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6a88a-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  