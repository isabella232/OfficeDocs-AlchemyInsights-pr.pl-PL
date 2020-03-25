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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931272"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="5a6a3-102">Problemy z DLP - numery paszportów USA/Wielkiej Brytanii</span><span class="sxs-lookup"><span data-stu-id="5a6a3-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="5a6a3-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5a6a3-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5a6a3-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5a6a3-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5a6a3-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5a6a3-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5a6a3-109">**Problemy z DLP z numerami paszportów USA/Wielkiej Brytanii**</span><span class="sxs-lookup"><span data-stu-id="5a6a3-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="5a6a3-110">Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla treści zawierających **numer paszportu USA / Wielkiej Brytanii** podczas korzystania z DLP typu poufnych informacji w O365?</span><span class="sxs-lookup"><span data-stu-id="5a6a3-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5a6a3-111">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="5a6a3-112">Na przykład w przypadku zasad **dotyczących numerów paszportów w STANACH Zjednoczonych/Wielkiej Brytanii** skonfigurowanych z poziomem ufności równym 75%, następujące zasady są oceniane i muszą zostać wykryte, aby reguła</span><span class="sxs-lookup"><span data-stu-id="5a6a3-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="5a6a3-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dziewięć cyfr</span><span class="sxs-lookup"><span data-stu-id="5a6a3-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="5a6a3-114">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Dziewięć kolejnych cyfr</span><span class="sxs-lookup"><span data-stu-id="5a6a3-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="5a6a3-115">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="5a6a3-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="5a6a3-116">**[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="5a6a3-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5a6a3-117">Funkcja Func_usa_uk_passport znajduje zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5a6a3-118">Zostanie znalezione słowo kluczowe z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="5a6a3-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="5a6a3-119">Na przykład następująca próbka spowoduje uruchomienie dla zasad **dotyczących numerów paszportów USA/Wielkiej Brytanii:** numer paszportu USA 123456789</span><span class="sxs-lookup"><span data-stu-id="5a6a3-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="5a6a3-120">Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia numeru paszportu USA/WIELKIEJ BRYTANII dla twojej zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają numeru paszportu USA/Wielkiej Brytanii](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="5a6a3-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="5a6a3-121">Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5a6a3-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  