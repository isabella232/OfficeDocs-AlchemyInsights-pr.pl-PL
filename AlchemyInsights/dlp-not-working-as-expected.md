---
title: DLP nie działa zgodnie z oczekiwaniami
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704423"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="6dcbd-102">DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="6dcbd-102">DLP not working as expected</span></span>

<span data-ttu-id="6dcbd-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="6dcbd-104">**Konfigurowanie DLP**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-104">**Setting up DLP**</span></span>

<span data-ttu-id="6dcbd-105">Czy masz problemy z **zapobieganiem utracie danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="6dcbd-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="6dcbd-106">Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawiera to, czego szukają **zasady DLP** podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="6dcbd-107">Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="6dcbd-108">Aby skonfigurować zasady DLP, użyj tych informacji [w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="6dcbd-109">**Czego szukają zasady DLP**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="6dcbd-110">Podczas korzystania z **wbudowanych typów informacji poufnych** w centrach zabezpieczeń i zgodności zasady DLP wyszukują określone wzorce i elementy podczas wykrywania tych typów poufnych.</span><span class="sxs-lookup"><span data-stu-id="6dcbd-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="6dcbd-111">**Wbudowane typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="6dcbd-112">Aby uzyskać informacje na temat wbudowanych typów poufnych i tego, czego szukają zasady DLP podczas wykrywania typu poufnego, zobacz: [Czego szukają typy poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="6dcbd-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="6dcbd-113">**Niestandardowe typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="6dcbd-114">Jeśli próbujesz utworzyć niestandardowe typy poufnych informacji, użyj następującego artykułu, aby uzyskać informacje dotyczące tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="6dcbd-115">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-115">**Test a DLP policy**</span></span>

<span data-ttu-id="6dcbd-116">Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu poufnych informacji, użyj opcji **Typ testu** w obszarze **Typy** > **informacji poufne**klasyfikacji .</span><span class="sxs-lookup"><span data-stu-id="6dcbd-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="6dcbd-117">Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="6dcbd-118">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="6dcbd-118">**Reports**</span></span>
  
- <span data-ttu-id="6dcbd-119">Uzyskaj szczegółowe informacje o poufnych danych dzięki [raportom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="6dcbd-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="6dcbd-120">Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="6dcbd-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
