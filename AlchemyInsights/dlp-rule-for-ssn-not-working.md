---
title: Reguła DLP dla numeru PESEL nie działa
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679379"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="14bc3-102">Problemy dotyczące DLP z numerami PESEL</span><span class="sxs-lookup"><span data-stu-id="14bc3-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="14bc3-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="14bc3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="14bc3-104">**Problemy z aplikacją DLP SSNs**</span><span class="sxs-lookup"><span data-stu-id="14bc3-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="14bc3-105">Czy występują problemy z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer PESEL (SSN)** , gdy jest używany typ informacji wrażliwych w programie Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="14bc3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="14bc3-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące działania zasad DLP.</span><span class="sxs-lookup"><span data-stu-id="14bc3-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="14bc3-107">Na przykład w przypadku zasad SSN skonfigurowanych z poziomem ufności 85% obliczane są następujące wartości, które muszą zostać wykryte, aby reguła była wyzwalana:</span><span class="sxs-lookup"><span data-stu-id="14bc3-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="14bc3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cyfr, które mogą znajdować się w sformatowanym lub niesformatowanym deseniu</span><span class="sxs-lookup"><span data-stu-id="14bc3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="14bc3-109">**[Wzorzec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje Szukaj SSNs w czterech różnych wzorach:</span><span class="sxs-lookup"><span data-stu-id="14bc3-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="14bc3-110">Func_ssn odnajduje SSNs przy użyciu funkcji 2011 wcześniejszego formatowania, które są sformatowane za pomocą kresek lub spacji (DDD-DD-dddd lub DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="14bc3-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="14bc3-111">Func_unformatted_ssn znajduje SSNs o silnym formatowaniu sprzed 2011, które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="14bc3-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="14bc3-112">Func_randomized_formatted_ssn znajduje znaki post-2011 SSNs, które są sformatowane za pomocą kresek lub spacji (DDD-DD-dddd lub DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="14bc3-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="14bc3-113">Func_randomized_unformatted_ssn znajduje znaki post-2011 SSNs, które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="14bc3-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="14bc3-114">**[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, nie ma żadnej sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="14bc3-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="14bc3-115">**[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zasady DLP to 85% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="14bc3-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="14bc3-116">[Funkcja Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) umożliwia Znajdowanie zawartości zgodnej ze wzorcem.</span><span class="sxs-lookup"><span data-stu-id="14bc3-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="14bc3-117">Znaleziono słowo kluczowe from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="14bc3-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="14bc3-118">Przykłady słów kluczowych:  *zabezpieczenia społecznego, ubezpieczenie społeczne, #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="14bc3-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="14bc3-119">Na przykład poniższa przykład wywoła zasady SSN dla DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="14bc3-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="14bc3-120">Aby uzyskać więcej informacji na temat tego, co jest wymagane, aby SSNs został wykryty dla zawartości, zobacz poniższą sekcję w tym artykule: co to są [typy informacji wrażliwych na SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="14bc3-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="14bc3-121">Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .</span><span class="sxs-lookup"><span data-stu-id="14bc3-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  