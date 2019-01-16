---
title: Warunkowy dostęp z Windows Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303957"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="6e427-102">Warunkowy dostęp z Windows Intune</span><span class="sxs-lookup"><span data-stu-id="6e427-102">Conditional Access with Intune</span></span>

<span data-ttu-id="6e427-103">Przy użyciu **Dostępu warunkowego** w usłudze Intune wymaga 3 kroki:</span><span class="sxs-lookup"><span data-stu-id="6e427-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="6e427-p101">Utwórz **Zasadę warunkową dostępu** , który definiuje, jakie zasoby są chronione, a co warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów. Na przykład urządzenie musi być zgodny, przed uzyskaniem dostępu do firmowych wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="6e427-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="6e427-p102">Tworzy **Zasady zgodności** do definiowania ustawień, które muszą być spełnione, zanim urządzenie zostanie uznana za zgodną. Na przykład urządzenie musi mieć co najmniej 6 cyfr numeru pin zostanie uznany za zgodny z.</span><span class="sxs-lookup"><span data-stu-id="6e427-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="6e427-p103">Zapewnienie zarówno **Zasady dostępu warunkowego** , jak i **Zasady zgodności** są kierowane do żądanej grupy użytkowników. To może być konieczne utworzenie określonych grup użytkowników w usłudze Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="6e427-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="6e427-110">Dowiedz się więcej:</span><span class="sxs-lookup"><span data-stu-id="6e427-110">Read more:</span></span>
  
- [<span data-ttu-id="6e427-111">Warunkowy dostęp do najlepszych praktyk</span><span class="sxs-lookup"><span data-stu-id="6e427-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="6e427-112">Wprowadzenie do dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="6e427-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

