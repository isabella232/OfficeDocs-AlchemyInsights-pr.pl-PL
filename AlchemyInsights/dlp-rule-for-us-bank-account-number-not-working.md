---
title: Reguła DLP dla numeru konta bankowego w USA nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507344"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="129df-102">Problemy z DLP z numerami amerykańskich kont bankowych</span><span class="sxs-lookup"><span data-stu-id="129df-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="129df-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="129df-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="129df-104">**Problemy z DLP z numerami amerykańskich kont bankowych**</span><span class="sxs-lookup"><span data-stu-id="129df-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="129df-105">Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer konta bankowego w USA** podczas korzystania z typu poufnych informacji DLP w UO365?</span><span class="sxs-lookup"><span data-stu-id="129df-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="129df-106">Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="129df-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="129df-107">Na przykład dla zasad **numeru konta bankowego w USA** skonfigurowanych z poziomem zaufania równym 85%, aby reguła wyzwoliła, są oceniane następujące zasady:</span><span class="sxs-lookup"><span data-stu-id="129df-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="129df-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cyfr</span><span class="sxs-lookup"><span data-stu-id="129df-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="129df-109">**[Wzór:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 kolejnych cyfr.</span><span class="sxs-lookup"><span data-stu-id="129df-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="129df-110">**[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma sumy kontrolnej</span><span class="sxs-lookup"><span data-stu-id="129df-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="129df-111">**[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:</span><span class="sxs-lookup"><span data-stu-id="129df-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="129df-112">Wyrażenie regularne Regex_usa_bank_account_number znajduje zawartość odpowiadającą wzorcowi</span><span class="sxs-lookup"><span data-stu-id="129df-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="129df-113">Zostanie znalezione słowo kluczowe z Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="129df-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="129df-114">Na przykład następujący przykład może wyzwolić zasady **numeru konta bankowego w USA:** Sprawdzanie konta 78344011</span><span class="sxs-lookup"><span data-stu-id="129df-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="129df-115">Aby uzyskać więcej informacji na temat tego, co jest wymagane do **wykrycia numeru konta bankowego w USA** dla zawartości, zobacz następującą sekcję w tym artykule: Jakie [typy poufnych informacji szukają numeru konta bankowego w USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="129df-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="129df-116">Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="129df-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  