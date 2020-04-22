---
title: Dostęp warunkowy z usłudze Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706031"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="144cf-102">Dostęp warunkowy z usłudze Intune</span><span class="sxs-lookup"><span data-stu-id="144cf-102">Conditional Access with Intune</span></span>

<span data-ttu-id="144cf-103">Korzystanie z **dostępu warunkowego** z usłudze Intune wymaga 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="144cf-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="144cf-104">Utwórz **zasady dostępu warunkowego,** który określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="144cf-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="144cf-105">Na przykład urządzenie musi być zgodne przed dostępem do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="144cf-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="144cf-106">Utwórz **zasady zgodności,** aby zdefiniować ustawienia, które muszą być spełnione, zanim urządzenie zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="144cf-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="144cf-107">Na przykład urządzenie musi mieć pin co najmniej 6 cyfr, zanim zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="144cf-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="144cf-108">Zapewnienie zarówno **zasad zgodności,** jak i **zasad dostępu warunkowego** są kierowane do pożądanych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="144cf-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="144cf-109">Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="144cf-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="144cf-110">Czytaj więcej:</span><span class="sxs-lookup"><span data-stu-id="144cf-110">Read more:</span></span>
  
- [<span data-ttu-id="144cf-111">Najważniejsze wskazówki dotyczące dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="144cf-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="144cf-112">Wprowadzenie do dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="144cf-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

