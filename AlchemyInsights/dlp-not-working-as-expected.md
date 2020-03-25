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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932632"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="95182-102">DLP nie działa zgodnie z oczekiwaniami</span><span class="sxs-lookup"><span data-stu-id="95182-102">DLP not working as expected</span></span>

<span data-ttu-id="95182-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="95182-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="95182-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="95182-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="95182-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="95182-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="95182-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="95182-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="95182-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="95182-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="95182-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="95182-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="95182-109">**Konfigurowanie DLP**</span><span class="sxs-lookup"><span data-stu-id="95182-109">**Setting up DLP**</span></span>

<span data-ttu-id="95182-110">Czy masz problemy z **zapobieganiem utracie danych (DLP)** w usłudze Office 365, nie działa zgodnie z oczekiwaniami?</span><span class="sxs-lookup"><span data-stu-id="95182-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="95182-111">Jeśli tak, upewnij się, że **zasady DLP** jest poprawnie skonfigurowany i że dane zawiera to, czego szukają **zasady DLP** podczas oceny.</span><span class="sxs-lookup"><span data-stu-id="95182-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="95182-112">Zasady DLP umożliwiają identyfikowanie i ochronę poufnych informacji w organizacji.</span><span class="sxs-lookup"><span data-stu-id="95182-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="95182-113">Aby skonfigurować zasady DLP, użyj tych informacji [w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="95182-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="95182-114">**Czego szukają zasady DLP**</span><span class="sxs-lookup"><span data-stu-id="95182-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="95182-115">Podczas korzystania z **wbudowanych typów poufnych informacji** w Centrum zabezpieczeń i zgodności usługi Office 365 zasady DLP wyszukują określone wzorce i elementy podczas wykrywania tych typów poufnych.</span><span class="sxs-lookup"><span data-stu-id="95182-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="95182-116">**Wbudowane typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="95182-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="95182-117">Aby uzyskać informacje na temat wbudowanych typów poufnych i tego, czego szukają zasady DLP podczas wykrywania typu poufnego, zobacz: [Czego szukają typy poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="95182-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="95182-118">**Niestandardowe typy poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="95182-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="95182-119">Jeśli próbujesz utworzyć niestandardowe typy poufnych informacji, użyj następującego artykułu, aby uzyskać informacje dotyczące tworzenia niestandardowego typu poufnego: [Tworzenie niestandardowego typu poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="95182-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="95182-120">**Testowanie zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="95182-120">**Test a DLP policy**</span></span>

<span data-ttu-id="95182-121">Aby przetestować dane przy użyciu wbudowanego lub niestandardowego typu poufnych informacji, użyj opcji **Typ testu** w obszarze **Typy** > **informacji poufne**klasyfikacji .</span><span class="sxs-lookup"><span data-stu-id="95182-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="95182-122">Aby uzyskać więcej informacji, zobacz [Testowanie niestandardowych typów poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="95182-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="95182-123">**Raporty**</span><span class="sxs-lookup"><span data-stu-id="95182-123">**Reports**</span></span>
  
- <span data-ttu-id="95182-124">Uzyskaj szczegółowe informacje o poufnych danych dzięki [raportom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="95182-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="95182-125">Zobacz szczegółowe informacje o zdarzeniu za pomocą [raportu o zdarzeniu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="95182-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
