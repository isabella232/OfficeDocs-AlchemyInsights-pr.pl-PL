---
title: Porady dotyczące zasad DLP nie działają
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932596"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="1a3ec-102">Problemy z poradami dotyczącymi zasad DLP</span><span class="sxs-lookup"><span data-stu-id="1a3ec-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="1a3ec-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1a3ec-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1a3ec-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1a3ec-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1a3ec-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1a3ec-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1a3ec-109">**Wskazówki dotyczące zasad DLP**</span><span class="sxs-lookup"><span data-stu-id="1a3ec-109">**DLP policy tips**</span></span>

<span data-ttu-id="1a3ec-110">Podczas korzystania z **zasad DLP**użytkownicy mogą otrzymywać powiadomienia o naruszeniu zasad za pomocą **wskazówek dotyczących zasad.**</span><span class="sxs-lookup"><span data-stu-id="1a3ec-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="1a3ec-111">Administratorzy mogą skonfigurować wskazówki dotyczące zasad do wyświetlania podczas testowania zasad DLP lub gdy zasady są w trybie pełnego wymuszania.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="1a3ec-112">Aby skonfigurować wskazówki dotyczące zasad dotyczących zasad DLP w Centrum zabezpieczeń i zgodności w trybie pełnego wymuszania, wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="1a3ec-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="1a3ec-113">Upewnij się, że wskazówki dotyczące zasad zostały **włączone** w regule DLP, wykonując kroki [opisane w tym miejscu](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="1a3ec-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="1a3ec-114">Upewnij się, że **zawartość jest zgodna** z tym, co jest **wymagane** do wyzwolenia reguły opisanej w tym artykule [tutaj](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="1a3ec-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="1a3ec-115">Porady dotyczące zasad są wyświetlane zarówno w programie OWA, jak i w programie Outlook.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="1a3ec-116">Jednak w przypadku korzystania z **programu Outlook 2013 lub nowszego**porady dotyczące zasad są wyświetlane tylko pod pewnymi warunkami.</span><span class="sxs-lookup"><span data-stu-id="1a3ec-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="1a3ec-117">Te warunki są wymienione w tym miejscu: [Obsługiwane warunki dla programu Outlook 2013 lub nowszego dotyczące wyświetlania porad dotyczących zasad](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="1a3ec-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="1a3ec-118">Aby uzyskać dodatkowe informacje na temat wskazówek dotyczących zasad DLP, zobacz: [Pokaż wskazówki dotyczące zasad dla zasad DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="1a3ec-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  