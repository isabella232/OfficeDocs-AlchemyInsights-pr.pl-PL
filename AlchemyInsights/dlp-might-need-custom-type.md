---
title: DLP może potrzebować typu niestandardowego
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052911"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8c81b-102">DLP może potrzebować typu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="8c81b-102">DLP might need a custom type</span></span>

<span data-ttu-id="8c81b-103">Dzięki zasadzie ochrony przed utratą danych (DLP) można identyfikować i chronić poufne dane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="8c81b-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8c81b-104">W niektórych scenariuszach może być konieczne utworzenie własnego **niestandardowego** typu informacji poufnych, aby chronić dane organizacji.</span><span class="sxs-lookup"><span data-stu-id="8c81b-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8c81b-105">Na przykład Twoja organizacja może potrzebować zidentyfikować i ochronić identyfikatory pracowników lub inne dane w jakimś formacie specyficznej dla Twojej organizacji. Jeśli tak, zobacz następujące artykuły, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="8c81b-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8c81b-106">**Dostosowywanie wbudowanego typu informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="8c81b-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8c81b-107">Jeśli wbudowany typ informacji poufnych spełni Twoje potrzeby z zaledwie kilkoma Wariacje, można [dostosować typ informacji poufnych wbudowanych](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8c81b-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8c81b-108">Na przykład można dodawać lub usuwać słowa kluczowe lub dodawać lub usuwać dowody potwierdzające, takie jak data lub adres.</span><span class="sxs-lookup"><span data-stu-id="8c81b-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8c81b-109">**Tworzenie niestandardowego typu informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="8c81b-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8c81b-110">Ale jeśli trzeba zidentyfikować i ochrony innego typu poufnych informacji całkowicie, można [utworzyć niestandardowy typ informacji poufnych](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="8c81b-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8c81b-111">**Utwórz niestandardowy typ informacji poufnych w programie Security & Centrum zgodności środowiska PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8c81b-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8c81b-112">Na koniec Jeśli interfejs użytkownika nie dostarcza wszystkich potrzebnych opcji, można [utworzyć niestandardowy typ informacji poufnych w programie Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="8c81b-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8c81b-113">Rozpoczynając od pliku XML, można użyć każdej dostępnej opcji.</span><span class="sxs-lookup"><span data-stu-id="8c81b-113">By starting with an XML file, you can use every option available.</span></span>
