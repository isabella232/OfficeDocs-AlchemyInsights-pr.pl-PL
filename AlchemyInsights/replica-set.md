---
title: Zestaw replik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714253"
---
# <a name="replica-set"></a><span data-ttu-id="1017f-102">Zestaw replik</span><span class="sxs-lookup"><span data-stu-id="1017f-102">Replica set</span></span>

<span data-ttu-id="1017f-103">Identyfikator AADDS jest również nazywany domeną zarządzaną.</span><span class="sxs-lookup"><span data-stu-id="1017f-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="1017f-104">W rzeczywistości są to dwa kontrolery domeny uruchamiane i utrzymywane przez zaplecza.</span><span class="sxs-lookup"><span data-stu-id="1017f-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="1017f-105">Oba te kontrolery obejmują jeden główny kontroler dc i jeden kontroler dc replikacji.</span><span class="sxs-lookup"><span data-stu-id="1017f-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="1017f-106">Kopie zapasowe w domenie zarządzanej AADDS to zautomatyzowany proces zarządzany przez platformę Azure.</span><span class="sxs-lookup"><span data-stu-id="1017f-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="1017f-107">W przypadku problemu z domeną zarządzaną pomoc techniczna platformy Azure może pomóc w przywracaniu z kopii zapasowej.</span><span class="sxs-lookup"><span data-stu-id="1017f-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="1017f-108">Każdy zestaw replik tworzy się w sieci wirtualnej.</span><span class="sxs-lookup"><span data-stu-id="1017f-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="1017f-109">Każda sieć wirtualna musi być równorzędna z co drugą siecią wirtualną hostową repliki domeny zarządzanej.</span><span class="sxs-lookup"><span data-stu-id="1017f-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="1017f-110">Ta konfiguracja tworzy topologię sieci siatki, która obsługuje replikację katalogów.</span><span class="sxs-lookup"><span data-stu-id="1017f-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="1017f-111">Sieć wirtualna może obsługiwać wiele replik zestawów, pod warunkiem że każdy zestaw replik znajduje się w innej wirtualnej podsieci.</span><span class="sxs-lookup"><span data-stu-id="1017f-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="1017f-112">Aby uzyskać więcej szczegółowych informacji na temat zestawu replik, zobacz [zestawy replik pojęć.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="1017f-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
