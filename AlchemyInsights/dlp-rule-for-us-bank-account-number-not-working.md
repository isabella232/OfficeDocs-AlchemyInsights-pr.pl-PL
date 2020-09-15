---
title: Reguła DLP dla numeru konta bankowego nie działa w Stanach Zjednoczonych
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679306"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="613c0-102">Problemy dotyczące DLP w numerach kont bankowych Stanów Zjednoczonych</span><span class="sxs-lookup"><span data-stu-id="613c0-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="613c0-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="613c0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="613c0-104">**Problemy dotyczące DLP w numerach kont bankowych Stanów Zjednoczonych**</span><span class="sxs-lookup"><span data-stu-id="613c0-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="613c0-105">Czy problemy związane z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer konta bankowego w Stanach Zjednoczonych** w przypadku korzystania z informacji poufnych dotyczących DLP w usłudze Office 365?</span><span class="sxs-lookup"><span data-stu-id="613c0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="613c0-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, co mają zasady DLP podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="613c0-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="613c0-107">Na przykład w przypadku zasad **numeru konta bankowego Stanów Zjednoczonych** skonfigurowanych z poziomem ufności równą 85% zostaną obliczone następujące obliczenia i trzeba je wykryć, aby reguła była wyzwalana:</span><span class="sxs-lookup"><span data-stu-id="613c0-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="613c0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cyfr</span><span class="sxs-lookup"><span data-stu-id="613c0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="613c0-109">**[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 kolejnych cyfr.</span><span class="sxs-lookup"><span data-stu-id="613c0-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="613c0-110">**[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="613c0-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="613c0-111">**[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zasady DLP to 75% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="613c0-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="613c0-112">Wyrażenie regularne Regex_usa_bank_account_number umożliwia Znajdowanie zawartości zgodnej ze wzorcem</span><span class="sxs-lookup"><span data-stu-id="613c0-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="613c0-113">Znaleziono słowo kluczowe from Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="613c0-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="613c0-114">Na przykład Poniższa przykładowa zasada **numeru konta bankowego Stanów Zjednoczonych** : sprawdzanie konta 78344011</span><span class="sxs-lookup"><span data-stu-id="613c0-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="613c0-115">Aby uzyskać więcej informacji na temat tego, co jest wymagane, aby **numer konta bankowego w Stanach Zjednoczonych** był wykrywany dla zawartości, zapoznaj się z poniższą sekcją w tym artykule: co to są [typy informacji wrażliwych na numer konta bankowego](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .</span><span class="sxs-lookup"><span data-stu-id="613c0-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="613c0-116">Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .</span><span class="sxs-lookup"><span data-stu-id="613c0-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  