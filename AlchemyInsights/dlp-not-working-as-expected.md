---
title: DLP nie działa zgodnie z oczekiwaniami
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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707820"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e9126-102">DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="e9126-102">DLP not working as expected</span></span>

<span data-ttu-id="e9126-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e9126-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e9126-104">**Konfigurowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="e9126-104">**Setting up DLP**</span></span>

<span data-ttu-id="e9126-105">Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention) w** usłudze Office 365 nie działa zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="e9126-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e9126-106">Jeśli tak, upewnij się, że zasady **DLP** zostały poprawnie skonfigurowane i że dane zawierają szukane zasady **DLP** podczas ich oceny.</span><span class="sxs-lookup"><span data-stu-id="e9126-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e9126-107">Zasady DLP umożliwiają identyfikowanie i ochronę informacji poufnych w organizacji.</span><span class="sxs-lookup"><span data-stu-id="e9126-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e9126-108">Aby skonfigurować zasady DLP, skorzystaj z informacji w tym [miejscu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)</span><span class="sxs-lookup"><span data-stu-id="e9126-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="e9126-109">**Jakie zasady ochrony przed zasadami ochrony przed zasadami DLP należy szukać**</span><span class="sxs-lookup"><span data-stu-id="e9126-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e9126-110">Podczas korzystania **z** wbudowanych typów informacji poufnych w centrach zabezpieczeń i zgodności zasady DLP szukają określonych wzorców i elementów podczas wykrywania tych typów poufnych.</span><span class="sxs-lookup"><span data-stu-id="e9126-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e9126-111">**Wbudowane typy informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="e9126-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e9126-112">Aby uzyskać informacje o wbudowanych typach poufnych oraz o tym, co wyszukuje zasady DLP podczas wykrywania typu poufnego, zobacz: Czego szukają typy [informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="e9126-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e9126-113">**Niestandardowe typy informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="e9126-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e9126-114">Jeśli próbujesz utworzyć niestandardowe typy informacji poufnych, skorzystaj z następującego artykułu, aby uzyskać informacje na temat tworzenia niestandardowego typu poufnego: Tworzenie niestandardowego typu informacji [poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="e9126-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e9126-115">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="e9126-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e9126-116">Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu informacji poufnych, użyj opcji **Typ** testu w obszarze **Klasyfikacje** typów informacji  >  **poufnych.**</span><span class="sxs-lookup"><span data-stu-id="e9126-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e9126-117">Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów informacji poufnych.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="e9126-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e9126-118">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="e9126-118">**Reports**</span></span>
  
- <span data-ttu-id="e9126-119">Uzyskiwanie szczegółowych informacji o danych poufnych za pomocą [raportów DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e9126-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e9126-120">Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="e9126-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
