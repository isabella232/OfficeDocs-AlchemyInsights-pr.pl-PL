---
title: Układ DLP nie działa zgodnie z oczekiwaniami
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679703"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="56de2-102">Układ DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="56de2-102">DLP not working as expected</span></span>

<span data-ttu-id="56de2-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="56de2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="56de2-104">**Konfigurowanie DLP**</span><span class="sxs-lookup"><span data-stu-id="56de2-104">**Setting up DLP**</span></span>

<span data-ttu-id="56de2-105">Czy problemy z **Zapobieganie utracie danych (DLP)** w pakiecie Office 365 nie działają zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="56de2-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="56de2-106">Jeśli tak, upewnij się, że **zasady DLP** są poprawnie skonfigurowane i że dane zawierają **zasady DLP** , które są używane podczas szacowania.</span><span class="sxs-lookup"><span data-stu-id="56de2-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="56de2-107">Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji.</span><span class="sxs-lookup"><span data-stu-id="56de2-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="56de2-108">Aby skonfigurować zasady DLP, Skorzystaj z informacji w [tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="56de2-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="56de2-109">**Jakie zasady DLP wyglądają**</span><span class="sxs-lookup"><span data-stu-id="56de2-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="56de2-110">Gdy korzystasz z **wbudowanych typów informacji poufnych** w centrach zabezpieczeń i zgodności, zasady DLP szukają określonych wzorców i elementów podczas wykrywania tych wrażliwych typów.</span><span class="sxs-lookup"><span data-stu-id="56de2-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="56de2-111">**Wbudowane typy informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="56de2-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="56de2-112">Aby uzyskać informacje na temat wbudowanych typów poufnych oraz zasad DLP, które wyszukują podczas wykrywania typu poufnego, zobacz: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="56de2-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="56de2-113">**Niestandardowe typy informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="56de2-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="56de2-114">Jeśli próbujesz utworzyć niestandardowe typy informacji poufnych, Skorzystaj z następującego artykułu, aby uzyskać informacje na temat tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="56de2-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="56de2-115">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="56de2-115">**Test a DLP policy**</span></span>

<span data-ttu-id="56de2-116">Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu informacji poufnych, użyj opcji **typ testu** w obszarze **klasyfikacje**  >  **informacje wrażliwe**.</span><span class="sxs-lookup"><span data-stu-id="56de2-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="56de2-117">Aby uzyskać więcej informacji, zobacz [testowanie typów niestandardowych informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="56de2-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="56de2-118">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="56de2-118">**Reports**</span></span>
  
- <span data-ttu-id="56de2-119">Uzyskiwanie ważnych danych w celu uwzględnienia [raportów DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="56de2-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="56de2-120">Szczegółowe informacje o zdarzeniu można znaleźć w [raporcie dotyczącym incydentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="56de2-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
