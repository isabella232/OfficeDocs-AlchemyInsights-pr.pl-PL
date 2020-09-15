---
title: Reguła DLP dla numeru paszportu my/UK nie działa
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679234"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="748ec-102">Problemy z numerami paszportów DLP-USA/UK</span><span class="sxs-lookup"><span data-stu-id="748ec-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="748ec-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="748ec-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="748ec-104">**Problemy ze współdziałaniem z numerami Passport w USA/Wielkiej Brytanii**</span><span class="sxs-lookup"><span data-stu-id="748ec-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="748ec-105">Czy występują problemy z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer paszportu USA/Wielkiej Brytanii** w przypadku korzystania z typu informacji poufnych dla DLP w usłudze O365?</span><span class="sxs-lookup"><span data-stu-id="748ec-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="748ec-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, co mają zasady DLP podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="748ec-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="748ec-107">Na przykład w przypadku zasad **numeru paszportów amerykańskich/brytyjskich** skonfigurowanych z poziomem ufności równą 75% zostaną obliczone następujące obliczenia i trzeba je wykryć, aby reguła była wyzwalana.</span><span class="sxs-lookup"><span data-stu-id="748ec-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="748ec-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dziewięć cyfr</span><span class="sxs-lookup"><span data-stu-id="748ec-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="748ec-109">**[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Dziewięć kolejnych cyfr</span><span class="sxs-lookup"><span data-stu-id="748ec-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="748ec-110">**[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="748ec-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="748ec-111">**[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zasady DLP to 75% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="748ec-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="748ec-112">Funkcja Func_usa_uk_passport umożliwia Znajdowanie zawartości zgodnej ze wzorcem.</span><span class="sxs-lookup"><span data-stu-id="748ec-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="748ec-113">Znaleziono słowo kluczowe from Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="748ec-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="748ec-114">Na przykład Poniższa przykładowa zasada **numeru paszportu US/UK** jest wyzwalana: numer paszportu amerykańskiego 123456789</span><span class="sxs-lookup"><span data-stu-id="748ec-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="748ec-115">Aby uzyskać więcej informacji na temat tego, co jest wymagane w przypadku wykrycia dla zawartości numeru paszportu USA/Wielkiej Brytanii, zobacz poniższą sekcję w tym artykule: [co to są typy informacji wrażliwych na numer paszportu my/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .</span><span class="sxs-lookup"><span data-stu-id="748ec-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="748ec-116">Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .</span><span class="sxs-lookup"><span data-stu-id="748ec-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  