---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679451"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="919c9-102">Problemy dotyczące DLP z numerami kart kredytowych</span><span class="sxs-lookup"><span data-stu-id="919c9-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="919c9-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="919c9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="919c9-104">**Problemy dotyczące DLP z numerami kart kredytowych**</span><span class="sxs-lookup"><span data-stu-id="919c9-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="919c9-105">Czy problemy związane z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer karty kredytowej** przy użyciu informacji poufnych dla DLP w usłudze Office 365?</span><span class="sxs-lookup"><span data-stu-id="919c9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="919c9-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje, aby wyzwolić zasady DLP podczas jej szacowania.</span><span class="sxs-lookup"><span data-stu-id="919c9-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="919c9-107">Na przykład w przypadku **zasad dotyczących karty kredytowej** skonfigurowanych z poziomem ufności 85% obliczane są następujące wartości, które muszą zostać wykryte, aby reguła była wyzwalana:</span><span class="sxs-lookup"><span data-stu-id="919c9-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="919c9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cyfr, które mogą być formatowane lub niesformatowane (dddddddddddddddd) i muszą przebiegać test LUHN.</span><span class="sxs-lookup"><span data-stu-id="919c9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="919c9-109">**[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Bardzo skomplikowany i niezawodny deseń wykrywający karty ze wszystkich głównych marek na całym świecie, w tym karty Visa, MasterCard, Discover Card, JCB, American Express, karty upominkowe i karty Diner.</span><span class="sxs-lookup"><span data-stu-id="919c9-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="919c9-110">**[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Tak, suma kontrolna LUHN</span><span class="sxs-lookup"><span data-stu-id="919c9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="919c9-111">**[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zasady DLP to 85% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="919c9-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="919c9-112">Funkcja Func_credit_card umożliwia Znajdowanie zawartości zgodnej ze wzorcem.</span><span class="sxs-lookup"><span data-stu-id="919c9-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="919c9-113">Jest spełniony co najmniej jedna z następujących warunków:</span><span class="sxs-lookup"><span data-stu-id="919c9-113">One of the following is true:</span></span>

  - <span data-ttu-id="919c9-114">Znaleziono słowo kluczowe from Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="919c9-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="919c9-115">Znaleziono słowo kluczowe z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="919c9-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="919c9-116">Funkcja Func_expiration_date umożliwia znalezienie daty w prawidłowym formacie daty.</span><span class="sxs-lookup"><span data-stu-id="919c9-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="919c9-117">Przekazanie sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="919c9-117">The checksum passes</span></span>

    <span data-ttu-id="919c9-118">Na przykład w przypadku numeru karty kredytowej DLP jest wyzwalana następująca przykład:</span><span class="sxs-lookup"><span data-stu-id="919c9-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="919c9-119">Wiza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="919c9-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="919c9-120">Wygasa: 2/2009</span><span class="sxs-lookup"><span data-stu-id="919c9-120">Expires: 2/2009</span></span>

<span data-ttu-id="919c9-121">Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia **numeru karty kredytowej** dla zawartości, zobacz poniższą sekcję w tym artykule: co to są [typy informacji wrażliwych na typ karty kredytowej #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="919c9-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="919c9-122">Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .</span><span class="sxs-lookup"><span data-stu-id="919c9-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  