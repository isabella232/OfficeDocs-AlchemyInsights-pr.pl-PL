---
title: Konfiguracja wirtualna z usługami domenowymi w usłudze AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885645"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="b474a-102">Konfiguracja wirtualna z usługami domenowymi w usłudze AAD</span><span class="sxs-lookup"><span data-stu-id="b474a-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="b474a-103">Konfiguracja wirtualna z usługami domenowymi w usłudze AAD obejmuje następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="b474a-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="b474a-104">Sprawdzanie kondycji domeny w portalu Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="b474a-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="b474a-105">Sprawdzanie NSG dla reguł, które blokują porty potrzebne do synchronizacji w usługach domenowych w usłudze Azure AD w portalu https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="b474a-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="b474a-106">Sprawdzanie, czy sieć wirtualna jest wdrożona w tym samym regionie platformy Azure, co domena zarządzana przez usługi domenowe w usłudze Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b474a-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="b474a-107">Upewnianie się, że nie masz istniejącej domeny z tą samą nazwą domeny dostępną w sieci wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="b474a-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="b474a-108">Aby uzyskać więcej szczegółowych informacji na temat zagadnień dotyczących projektowania sieci wirtualnej platformy Azure do obsługi usług domenowych w usłudze AAD, zobacz [zagadnienia dotyczące sieci wirtualnej](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="b474a-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

