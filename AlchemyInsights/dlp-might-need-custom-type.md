---
title: DLP może wymagać typu niestandardowego
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932668"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="bab8e-102">DLP może wymagać typu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="bab8e-102">DLP might need a custom type</span></span>

<span data-ttu-id="bab8e-103">**Ważne:** Wielu klientów korzystających z usługi SharePoint Online i OneDrive uruchamia aplikacje o znaczeniu krytycznym dla firmy w stosunku do usługi działającej w tle.</span><span class="sxs-lookup"><span data-stu-id="bab8e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="bab8e-104">Należą do nich migracja zawartości, zapobieganie utracie danych (DLP) i rozwiązania do tworzenia kopii zapasowych.</span><span class="sxs-lookup"><span data-stu-id="bab8e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="bab8e-105">W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostają wysoce dostępne i niezawodne dla użytkowników, którzy są bardziej niż kiedykolwiek zależni od usługi w scenariuszach pracy zdalnej.</span><span class="sxs-lookup"><span data-stu-id="bab8e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="bab8e-106">W celu wsparcia tego celu wprowadziliśmy ściślejsze limity ograniczania przepustowości w aplikacjach w tle (migracja, DLP i rozwiązania do tworzenia kopii zapasowych) w dni powszednie w ciągu dnia.</span><span class="sxs-lookup"><span data-stu-id="bab8e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="bab8e-107">Należy się spodziewać, że te aplikacje osiągną bardzo ograniczoną przepływność w tych czasach.</span><span class="sxs-lookup"><span data-stu-id="bab8e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="bab8e-108">Jednak w godzinach wieczornych i weekendowych dla regionu usługa będzie gotowa do przetwarzania znacznie większej liczby żądań z aplikacji w tle.</span><span class="sxs-lookup"><span data-stu-id="bab8e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="bab8e-109">**DLP może wymagać niestandardowego typu informacji**</span><span class="sxs-lookup"><span data-stu-id="bab8e-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="bab8e-110">Za pomocą zasad zapobiegania utracie danych (DLP) można identyfikować i chronić poufne dane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="bab8e-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="bab8e-111">W niektórych scenariuszach może być konieczne utworzenie własnego **niestandardowego** typu poufnych informacji w celu ochrony danych organizacji.</span><span class="sxs-lookup"><span data-stu-id="bab8e-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="bab8e-112">Na przykład organizacja może wymagać identyfikowania i ochrony identyfikatorów pracowników lub innych danych w formacie specyficznym dla organizacji. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="bab8e-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="bab8e-113">**Dostosowywanie wbudowanego typu poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="bab8e-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="bab8e-114">Jeśli wbudowany typ poufnych informacji odpowiadałby Twoim potrzebom za pomocą zaledwie kilku poprawek, możesz [dostosować wbudowany typ poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="bab8e-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="bab8e-115">Możesz na przykład dodać lub usunąć słowa kluczowe lub dodać lub usunąć dowody potwierdzające, takie jak data lub adres.</span><span class="sxs-lookup"><span data-stu-id="bab8e-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="bab8e-116">**Tworzenie niestandardowego typu poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="bab8e-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="bab8e-117">Jeśli jednak musisz zidentyfikować i chronić zupełnie inny typ poufnych informacji, możesz [utworzyć niestandardowy typ poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika Centrum zgodności & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="bab8e-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="bab8e-118">**Tworzenie niestandardowego typu poufnych informacji w programie PowerShell centrum zabezpieczeń & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="bab8e-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="bab8e-119">Jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, można [utworzyć niestandardowy typ poufnych informacji w programie Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="bab8e-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="bab8e-120">Zaczynając od pliku XML, można użyć każdej dostępnej opcji.</span><span class="sxs-lookup"><span data-stu-id="bab8e-120">By starting with an XML file, you can use every option available.</span></span>
