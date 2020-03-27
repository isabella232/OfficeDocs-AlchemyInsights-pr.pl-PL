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
ms.openlocfilehash: 40a4a1668039b70455e09ee662359c05235645e8
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977208"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="0c4d0-102">Problemy z DLP z numerami kart kredytowych</span><span class="sxs-lookup"><span data-stu-id="0c4d0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="0c4d0-103">**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0c4d0-104">**Problemy z DLP z numerami kart kredytowych**</span><span class="sxs-lookup"><span data-stu-id="0c4d0-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="0c4d0-105">Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer karty kredytowej** podczas korzystania z typu poufnych informacji DLP w UO365?</span><span class="sxs-lookup"><span data-stu-id="0c4d0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0c4d0-106">Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne do wyzwolenia zasad DLP, gdy jest oceniana.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="0c4d0-107">Na przykład dla **zasad kart kredytowych** skonfigurowanych z poziomem zaufania równym 85%, aby reguła wyzwoliła, należy wykryć następujące zasady:</span><span class="sxs-lookup"><span data-stu-id="0c4d0-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="0c4d0-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowane (ddddddddddddddd) i muszą przejść test Luhna.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="0c4d0-109">**[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Bardzo złożony i solidny wzór, który wykrywa karty wszystkich głównych marek na całym świecie, w tym Visa, MasterCard, Discover Card, JCB, American Express, karty upominkowe i karty do kolacji.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="0c4d0-110">**[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna</span><span class="sxs-lookup"><span data-stu-id="0c4d0-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="0c4d0-111">**[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP są w 85% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="0c4d0-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0c4d0-112">Funkcja Func_credit_card znajduje zawartość, która pasuje do wzorca.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0c4d0-113">Jedna z następujących elementów jest prawdziwa:</span><span class="sxs-lookup"><span data-stu-id="0c4d0-113">One of the following is true:</span></span>

  - <span data-ttu-id="0c4d0-114">Zostanie znalezione słowo kluczowe z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="0c4d0-115">Znaleziono słowo kluczowe z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="0c4d0-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="0c4d0-116">Funkcja Func_expiration_date znajduje datę w odpowiednim formacie daty.</span><span class="sxs-lookup"><span data-stu-id="0c4d0-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="0c4d0-117">Suma kontrolna przechodzi</span><span class="sxs-lookup"><span data-stu-id="0c4d0-117">The checksum passes</span></span>

    <span data-ttu-id="0c4d0-118">Na przykład następujący przykład może wyzwolić zasady numeru karty kredytowej DLP:</span><span class="sxs-lookup"><span data-stu-id="0c4d0-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="0c4d0-119">Wiza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="0c4d0-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="0c4d0-120">Wygasa: 2/2009</span><span class="sxs-lookup"><span data-stu-id="0c4d0-120">Expires: 2/2009</span></span>

<span data-ttu-id="0c4d0-121">Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia **numeru karty kredytowej** dla twojej zawartości, zobacz następującą sekcję w tym artykule: Jakie [typy poufnych informacji szukają dla karty kredytowej#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="0c4d0-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="0c4d0-122">Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="0c4d0-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  