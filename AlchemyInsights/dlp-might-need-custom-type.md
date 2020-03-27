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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977280"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="2d358-102">DLP może wymagać typu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="2d358-102">DLP might need a custom type</span></span>

<span data-ttu-id="2d358-103">**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="2d358-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2d358-104">**DLP może wymagać niestandardowego typu informacji**</span><span class="sxs-lookup"><span data-stu-id="2d358-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="2d358-105">Za pomocą zasad zapobiegania utracie danych (DLP) można identyfikować i chronić poufne dane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="2d358-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="2d358-106">W niektórych scenariuszach może być konieczne utworzenie własnego **niestandardowego** typu poufnych informacji w celu ochrony danych organizacji.</span><span class="sxs-lookup"><span data-stu-id="2d358-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="2d358-107">Na przykład organizacja może wymagać identyfikowania i ochrony identyfikatorów pracowników lub innych danych w formacie specyficznym dla organizacji. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="2d358-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="2d358-108">**Dostosowywanie wbudowanego typu poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="2d358-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="2d358-109">Jeśli wbudowany typ poufnych informacji odpowiadałby Twoim potrzebom za pomocą zaledwie kilku poprawek, możesz [dostosować wbudowany typ poufnych informacji.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="2d358-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="2d358-110">Możesz na przykład dodać lub usunąć słowa kluczowe lub dodać lub usunąć dowody potwierdzające, takie jak data lub adres.</span><span class="sxs-lookup"><span data-stu-id="2d358-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="2d358-111">**Tworzenie niestandardowego typu poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="2d358-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="2d358-112">Jeśli jednak musisz zidentyfikować i chronić zupełnie inny typ poufnych informacji, możesz [utworzyć niestandardowy typ poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika Centrum zgodności & zabezpieczeń.</span><span class="sxs-lookup"><span data-stu-id="2d358-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="2d358-113">**Tworzenie niestandardowego typu poufnych informacji w programie PowerShell centrum zabezpieczeń & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="2d358-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="2d358-114">Jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, można [utworzyć niestandardowy typ poufnych informacji w programie Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="2d358-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="2d358-115">Zaczynając od pliku XML, można użyć każdej dostępnej opcji.</span><span class="sxs-lookup"><span data-stu-id="2d358-115">By starting with an XML file, you can use every option available.</span></span>
