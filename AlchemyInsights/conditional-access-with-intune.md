---
title: Warunkowy dostęp z Windows Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505004"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e0409-102">Warunkowy dostęp z Windows Intune</span><span class="sxs-lookup"><span data-stu-id="e0409-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e0409-103">Przy użyciu **Dostępu warunkowego** w usłudze Intune wymaga 3 kroki:</span><span class="sxs-lookup"><span data-stu-id="e0409-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e0409-104">Utwórz **Zasadę warunkową dostępu** , który definiuje, jakie zasoby są chronione, a co warunki muszą być spełnione, aby uzyskać dostęp do tych zasobów.</span><span class="sxs-lookup"><span data-stu-id="e0409-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e0409-105">Na przykład urządzenie musi być zgodny, przed uzyskaniem dostępu do firmowych wiadomości e-mail.</span><span class="sxs-lookup"><span data-stu-id="e0409-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e0409-106">Tworzy **Zasady zgodności** do definiowania ustawień, które muszą być spełnione, zanim urządzenie zostanie uznana za zgodną.</span><span class="sxs-lookup"><span data-stu-id="e0409-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e0409-107">Na przykład urządzenie musi mieć co najmniej 6 cyfr numeru pin zostanie uznany za zgodny z.</span><span class="sxs-lookup"><span data-stu-id="e0409-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e0409-108">Zapewnienie zarówno **Zasady dostępu warunkowego** , jak i **Zasady zgodności** są kierowane do żądanej grupy użytkowników.</span><span class="sxs-lookup"><span data-stu-id="e0409-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e0409-109">To może być konieczne utworzenie określonych grup użytkowników w usłudze Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="e0409-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e0409-110">Dowiedz się więcej:</span><span class="sxs-lookup"><span data-stu-id="e0409-110">Read more:</span></span>
  
- [<span data-ttu-id="e0409-111">Warunkowy dostęp do najlepszych praktyk</span><span class="sxs-lookup"><span data-stu-id="e0409-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e0409-112">Wprowadzenie do dostępu warunkowego</span><span class="sxs-lookup"><span data-stu-id="e0409-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

