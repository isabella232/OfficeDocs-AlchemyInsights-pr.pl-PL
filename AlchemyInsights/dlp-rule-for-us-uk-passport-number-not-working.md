---
title: Reguła DLP dla numeru paszportu USA/Wielkiej Brytanii nie działa
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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977116"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="41357-102">Problemy z DLP - numery paszportów USA/Wielkiej Brytanii</span><span class="sxs-lookup"><span data-stu-id="41357-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="41357-103">**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="41357-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="41357-104">**Problemy z DLP z numerami paszportów USA/Wielkiej Brytanii**</span><span class="sxs-lookup"><span data-stu-id="41357-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="41357-105">Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla treści zawierających **numer paszportu USA / Wielkiej Brytanii** podczas korzystania z DLP typu poufnych informacji w O365?</span><span class="sxs-lookup"><span data-stu-id="41357-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="41357-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="41357-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="41357-107">Na przykład w przypadku zasad **dotyczących numerów paszportów w STANACH Zjednoczonych/Wielkiej Brytanii** skonfigurowanych z poziomem ufności równym 75%, następujące zasady są oceniane i muszą zostać wykryte, aby reguła</span><span class="sxs-lookup"><span data-stu-id="41357-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="41357-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dziewięć cyfr</span><span class="sxs-lookup"><span data-stu-id="41357-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="41357-109">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Dziewięć kolejnych cyfr</span><span class="sxs-lookup"><span data-stu-id="41357-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="41357-110">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="41357-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="41357-111">**[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="41357-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="41357-112">Funkcja Func_usa_uk_passport znajduje zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="41357-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="41357-113">Zostanie znalezione słowo kluczowe z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="41357-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="41357-114">Na przykład następująca próbka spowoduje uruchomienie dla zasad **dotyczących numerów paszportów USA/Wielkiej Brytanii:** numer paszportu USA 123456789</span><span class="sxs-lookup"><span data-stu-id="41357-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="41357-115">Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia numeru paszportu USA/WIELKIEJ BRYTANII dla twojej zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają numeru paszportu USA/Wielkiej Brytanii](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="41357-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="41357-116">Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="41357-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  