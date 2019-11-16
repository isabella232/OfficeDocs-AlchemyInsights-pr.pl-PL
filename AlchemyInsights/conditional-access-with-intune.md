---
title: Dostęp warunkowy z usługą Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505004"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="50eb2-102">Dostęp warunkowy z usługą Intune</span><span class="sxs-lookup"><span data-stu-id="50eb2-102">Conditional Access with Intune</span></span>

<span data-ttu-id="50eb2-103">Korzystanie z **dostępu warunkowego** w usłudze Intune wymaga 3 kroków:</span><span class="sxs-lookup"><span data-stu-id="50eb2-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="50eb2-104">Utwórz **zasadę dostępu warunkowego** , która określa, jakie zasoby są chronione i jakie warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="50eb2-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="50eb2-105">Na przykład urządzenie musi być zgodne przed uzyskaniem dostępu do firmowej poczty e-mail.</span><span class="sxs-lookup"><span data-stu-id="50eb2-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="50eb2-106">Utwórz **zasadę zgodności** , aby zdefiniować ustawienia, które muszą zostać spełnione, zanim urządzenie zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="50eb2-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="50eb2-107">Na przykład urządzenie musi mieć PIN co najmniej 6 cyfr, zanim zostanie uznane za zgodne.</span><span class="sxs-lookup"><span data-stu-id="50eb2-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="50eb2-108">Zapewnienie, że zarówno **zasady zgodności** , jak i **zasady dostępu warunkowego** są kierowane do żądanych grup użytkowników.</span><span class="sxs-lookup"><span data-stu-id="50eb2-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="50eb2-109">Może to wymagać utworzenia określonych grup użytkowników w usłudze Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50eb2-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="50eb2-110">Czytaj więcej:</span><span class="sxs-lookup"><span data-stu-id="50eb2-110">Read more:</span></span>
  
- [<span data-ttu-id="50eb2-111">Najważniejsze wskazówki dotyczące dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="50eb2-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="50eb2-112">Rozpoczynanie korzystania z dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="50eb2-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

