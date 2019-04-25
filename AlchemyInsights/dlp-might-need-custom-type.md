---
title: DLP może być konieczne typu niestandardowego
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: cd5bac5efe3a16d32f9b695c8cb452a1eaa3a796
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399117"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="a0ad9-102">DLP może być konieczne typu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="a0ad9-102">DLP might need a custom type</span></span>

<span data-ttu-id="a0ad9-103">Z zasady zapobiegania (DLP) utraty danych można zidentyfikować i ochrony poufnych danych w organizacji.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="a0ad9-104">W niektórych scenariuszach może być konieczne utworzyć swój własny **Niestandardowy** typ informacji poufnych do ochrony danych w organizacji.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="a0ad9-105">Na przykład organizacja może być konieczne dla ustalenia i ochrony identyfikatory pracowników lub innych danych w określonym formacie specyficzne dla Twojego org. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span> 
  
 <span data-ttu-id="a0ad9-106">**Dostosować typ wbudowany poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="a0ad9-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="a0ad9-107">Jeśli typ wbudowany poufnych informacji, by spełnić Twoje potrzeby z kilka poprawek, można [dostosować typ wbudowany poufnych informacji](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="a0ad9-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="a0ad9-108">Na przykład możesz można dodać lub usunąć słowa kluczowe, lub dodać lub usunąć dowody, takie jak data lub adres.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="a0ad9-109">**Tworzenie typu niestandardowego poufnych informacji**</span><span class="sxs-lookup"><span data-stu-id="a0ad9-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="a0ad9-110">Ale jeśli zachodzi konieczność ustalenia i ochrony zupełnie innego typu informacji poufnych, możesz [utworzyć typ niestandardowy poufne informacje](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika & zabezpieczeń Centrum zgodności.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span> 
  
<span data-ttu-id="a0ad9-111">**Tworzenie typu niestandardowe informacje poufne w & zabezpieczeń środowiska PowerShell Centrum zgodności**</span><span class="sxs-lookup"><span data-stu-id="a0ad9-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="a0ad9-112">Wreszcie Jeśli interfejs użytkownika nie udostępnia wszystkie opcje, które są potrzebne, można [utworzyć typ niestandardowy poufnych informacji w & zabezpieczeń środowiska PowerShell Centrum zgodności](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="a0ad9-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="a0ad9-113">Zaczynając od pliku XML, można użyć wszystkie dostępne opcje.</span><span class="sxs-lookup"><span data-stu-id="a0ad9-113">By starting with an XML file, you can use every option available.</span></span>

    
