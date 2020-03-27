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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977448"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="12366-102">DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="12366-102">DLP not working as expected</span></span>

<span data-ttu-id="12366-103">**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="12366-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="12366-104">**Konfigurowanie DLP**</span><span class="sxs-lookup"><span data-stu-id="12366-104">**Setting up DLP**</span></span>

<span data-ttu-id="12366-105">Czy masz problemy z **zapobieganiem utracie danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="12366-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="12366-106">Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawiera to, czego szukają **zasady DLP** podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="12366-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="12366-107">Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji.</span><span class="sxs-lookup"><span data-stu-id="12366-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="12366-108">Aby skonfigurować zasady DLP, użyj tych informacji [w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="12366-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="12366-109">**Czego szukają zasady DLP**</span><span class="sxs-lookup"><span data-stu-id="12366-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="12366-110">Podczas korzystania z **wbudowanych typów poufnych informacji** w Centrum zabezpieczeń i zgodności usługi Office 365 zasady DLP wyszukują określone wzorce i elementy podczas wykrywania tych typów poufnych.</span><span class="sxs-lookup"><span data-stu-id="12366-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="12366-111">**Wbudowane typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="12366-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="12366-112">Aby uzyskać informacje na temat wbudowanych typów poufnych i tego, czego szukają zasady DLP podczas wykrywania typu poufnego, zobacz: [Czego szukają typy poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="12366-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="12366-113">**Niestandardowe typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="12366-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="12366-114">Jeśli próbujesz utworzyć niestandardowe typy poufnych informacji, użyj następującego artykułu, aby uzyskać informacje dotyczące tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="12366-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="12366-115">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="12366-115">**Test a DLP policy**</span></span>

<span data-ttu-id="12366-116">Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu poufnych informacji, użyj opcji **Typ testu** w obszarze **Typy** > **informacji poufne**klasyfikacji .</span><span class="sxs-lookup"><span data-stu-id="12366-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="12366-117">Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="12366-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="12366-118">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="12366-118">**Reports**</span></span>
  
- <span data-ttu-id="12366-119">Uzyskaj szczegółowe informacje o poufnych danych dzięki [raportom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="12366-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="12366-120">Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="12366-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
