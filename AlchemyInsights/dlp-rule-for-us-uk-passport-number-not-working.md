---
title: Reguła DLP dla USA / numer paszportu UK nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529929"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="611c3-102">Problemy z DLP - USA / numeru paszportu Wielka Brytania</span><span class="sxs-lookup"><span data-stu-id="611c3-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="611c3-103">Czy masz problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **USA / Wielka Brytania numer paszportu** podczas używania typu informacji poufnych DLP w O365?</span><span class="sxs-lookup"><span data-stu-id="611c3-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="611c3-104">Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne co zasad DLP szuka podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="611c3-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="611c3-105">Na przykład, dla **USA / UK numer paszportu** zasada skonfigurowana z 75% poziomu ufności, następujące są oceniane i musi zostać wykryty dla reguły do uruchomienia</span><span class="sxs-lookup"><span data-stu-id="611c3-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="611c3-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dziewięciu cyfr</span><span class="sxs-lookup"><span data-stu-id="611c3-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="611c3-107">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Dziewięciu następujących po sobie cyfr</span><span class="sxs-lookup"><span data-stu-id="611c3-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="611c3-108">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma żadnych suma kontrolna</span><span class="sxs-lookup"><span data-stu-id="611c3-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="611c3-109">**[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Zasady DLP wynosi 75% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="611c3-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="611c3-110">Funkcja Func_usa_uk_passport znajduje się zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="611c3-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="611c3-111">Znajduje słowa kluczowego z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="611c3-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="611c3-112">Na przykład poniższy przykładowy pociągałaby za **USA / Wielka Brytania numer paszportu** zasad: numer paszportu USA 123456789</span><span class="sxs-lookup"><span data-stu-id="611c3-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="611c3-113">Aby uzyskać więcej informacji, co jest wymagane do USA / numer paszportu UK wykrycie dla zawartości, zobacz następującą sekcję w tym artykule: [co poufnych informacji typy wyglądu dla Stanów Zjednoczonych / numer paszportu UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="611c3-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="611c3-114">Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="611c3-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  