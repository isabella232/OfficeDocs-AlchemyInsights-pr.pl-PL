---
title: DLP nie działa zgodnie z oczekiwaniami
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 1ea457bd69e7d545cf761a0be849695738b19d8b
ms.sourcegitcommit: d6ea6f4456a582559f27b34c0b9455a86a8e61f1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/31/2019
ms.locfileid: "35941078"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="da97c-102">DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="da97c-102">DLP not working as expected</span></span>

<span data-ttu-id="da97c-103">Czy masz problemy z **Zapobiegania utraty danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="da97c-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="da97c-104">Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawierają jakie **zasady DLP** poszukuje podczas jest oceniana.</span><span class="sxs-lookup"><span data-stu-id="da97c-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="da97c-105">**Definiowanie DLP**</span><span class="sxs-lookup"><span data-stu-id="da97c-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="da97c-106">Zasady DLP pozwala zidentyfikować i ochrony poufnych informacji w danej organizacji.</span><span class="sxs-lookup"><span data-stu-id="da97c-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="da97c-107">Konfiguracja zasad DLP, należy użyć informacji [w tym polu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="da97c-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="da97c-108">**Jakie zasady DLP szukać**</span><span class="sxs-lookup"><span data-stu-id="da97c-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="da97c-109">Korzystając z **typów wbudowanych poufnych informacji** w Centrum Office 365 bezpieczeństwa i zgodności, zasad DLP szukać określonych wzorców i elementów podczas wykrywania tego typu wrażliwe.</span><span class="sxs-lookup"><span data-stu-id="da97c-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="da97c-110">**Typy wbudowane poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="da97c-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="da97c-111">Szczegółowe informacje o wbudowanych typów wrażliwych i co zasad DLP szuka podczas wykrywania typu wrażliwe,: [poszukaj jakie typy informacji poufnych](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="da97c-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="da97c-112">**Typy niestandardowe informacje poufne**</span><span class="sxs-lookup"><span data-stu-id="da97c-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="da97c-113">Jeśli próbujesz utworzyć typy niestandardowe informacje poufne, użyj następującego artykułu informacji na temat tworzenia niestandardowego typu poufne: [Utwórz typ niestandardowy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="da97c-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="da97c-114">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="da97c-114">**Test a DLP policy**</span></span>

<span data-ttu-id="da97c-115">Aby przetestować danych o typie wbudowane lub niestandardowe poufne informacje, należy użyć opcji **Typ testu** w obszarze **Klasyfikacje** > **typów poufnych informacji**.</span><span class="sxs-lookup"><span data-stu-id="da97c-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="da97c-116">Aby uzyskać więcej informacji zobacz [Typy niestandardowe informacje poufne testu](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="da97c-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="da97c-117">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="da97c-117">**Reports**</span></span>
  
- <span data-ttu-id="da97c-118">Wyszukaj informacje poufne dane z [DLP raportów.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="da97c-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="da97c-119">Zobacz szczegółowe informacje dotyczące zdarzeń [Incydentu raport](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)z.</span><span class="sxs-lookup"><span data-stu-id="da97c-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
