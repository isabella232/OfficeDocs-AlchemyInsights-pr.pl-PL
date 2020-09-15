---
title: Funkcja DLP może wymagać typu niestandardowego
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712194"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="b8dab-102">Funkcja DLP może wymagać typu niestandardowego</span><span class="sxs-lookup"><span data-stu-id="b8dab-102">DLP might need a custom type</span></span>

<span data-ttu-id="b8dab-103">**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b8dab-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b8dab-104">**Funkcja DLP może wymagać niestandardowego typu informacji**</span><span class="sxs-lookup"><span data-stu-id="b8dab-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="b8dab-105">Dzięki zasadom ochrony przed utratą danych (DLP) można identyfikować i chronić poufne dane w organizacji.</span><span class="sxs-lookup"><span data-stu-id="b8dab-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="b8dab-106">W przypadku kilku scenariuszy może być konieczne **utworzenie własnych typów informacji poufnych,** aby chronić dane organizacji.</span><span class="sxs-lookup"><span data-stu-id="b8dab-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="b8dab-107">Na przykład organizacja może potrzebować identyfikacji i ochrony identyfikatorów pracowników lub innych danych w pewnym formacie specyficznym dla organizacji. Jeśli tak, zobacz poniższe artykuły, aby uzyskać więcej informacji.</span><span class="sxs-lookup"><span data-stu-id="b8dab-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="b8dab-108">**Dostosowywanie wbudowanego typu informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="b8dab-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="b8dab-109">Jeśli wbudowany typ informacji poufnych spełnia Twoje potrzeby, wystarczy kilka ulepszeń, aby [dostosować wbudowany typ informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="b8dab-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="b8dab-110">Możesz na przykład dodawać lub usuwać słowa kluczowe albo dodawać lub usuwać dowody dodatkowe, takie jak data lub adres.</span><span class="sxs-lookup"><span data-stu-id="b8dab-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="b8dab-111">**Tworzenie niestandardowego typu informacji poufnych**</span><span class="sxs-lookup"><span data-stu-id="b8dab-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="b8dab-112">Jeśli jednak konieczne jest całkowite zidentyfikowanie i chronienie różnych typów poufnych informacji, można [utworzyć niestandardowe typy informacji poufnych](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) w interfejsie użytkownika centrum zabezpieczeń & zgodności.</span><span class="sxs-lookup"><span data-stu-id="b8dab-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="b8dab-113">**Tworzenie niestandardowego typu informacji poufnych w centrum zabezpieczeń & zgodności programu PowerShell**</span><span class="sxs-lookup"><span data-stu-id="b8dab-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="b8dab-114">Na koniec, jeśli interfejs użytkownika nie udostępnia wszystkich potrzebnych opcji, możesz [utworzyć niestandardowy typ informacji poufnych w centrum zabezpieczeń & zgodności programu PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b8dab-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="b8dab-115">Rozpoczynając od pliku XML, możesz korzystać z każdej dostępnej opcji.</span><span class="sxs-lookup"><span data-stu-id="b8dab-115">By starting with an XML file, you can use every option available.</span></span>
