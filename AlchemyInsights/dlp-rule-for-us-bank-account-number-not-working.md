---
title: Reguła DLP dla nas numer konta bankowego nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529887"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="6b4f6-102">DLP problemów z NAMI numerów kont bankowych</span><span class="sxs-lookup"><span data-stu-id="6b4f6-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="6b4f6-103">Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer konta bankowego w Stanach Zjednoczonych** , używając typu informacji poufnych DLP w O365?</span><span class="sxs-lookup"><span data-stu-id="6b4f6-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6b4f6-104">Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne co zasad DLP szuka podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="6b4f6-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="6b4f6-105">Na przykład dla zasady **Numer konta bankowego w Stanach Zjednoczonych** , skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:</span><span class="sxs-lookup"><span data-stu-id="6b4f6-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6b4f6-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cyfr</span><span class="sxs-lookup"><span data-stu-id="6b4f6-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="6b4f6-107">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cyfr.</span><span class="sxs-lookup"><span data-stu-id="6b4f6-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="6b4f6-108">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma żadnych suma kontrolna</span><span class="sxs-lookup"><span data-stu-id="6b4f6-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="6b4f6-109">**[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Zasady DLP wynosi 75% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="6b4f6-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6b4f6-110">Wyrażenie regularne Regex_usa_bank_account_number znajduje się zawartość, która pasuje do wzorca</span><span class="sxs-lookup"><span data-stu-id="6b4f6-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="6b4f6-111">Znajduje słowa kluczowego z Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="6b4f6-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="6b4f6-112">Na przykład poniższy przykładowy wywołałoby zasady **Numer konta bankowego w Stanach Zjednoczonych** : 78344011 konto bankowe</span><span class="sxs-lookup"><span data-stu-id="6b4f6-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="6b4f6-113">Aby uzyskać więcej informacji na co jest wymagane dla **USA numer konta bankowego** do wykrycia dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy wyszukać numer konta bankowego w Stanach Zjednoczonych](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="6b4f6-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="6b4f6-114">Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6b4f6-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  