---
title: Lokalizacja danych
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655292"
---
# <a name="data-location"></a><span data-ttu-id="ee295-102">Lokalizacja danych</span><span class="sxs-lookup"><span data-stu-id="ee295-102">Data location</span></span>

<span data-ttu-id="ee295-103">Lokalizację dzierżawy można wyświetlić w centrum administracyjnym lub łącząc się z usługą Exchange Online za pośrednictwem programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee295-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="ee295-104">**Centrum administracyjne:**</span><span class="sxs-lookup"><span data-stu-id="ee295-104">**Admin center:**</span></span>
1. <span data-ttu-id="ee295-105">Zaloguj się do [centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="ee295-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="ee295-106">Wybierz **pozycję Ustawienia** > **profilu organizacji**.</span><span class="sxs-lookup"><span data-stu-id="ee295-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="ee295-107">W obszarze **Lokalizacja danych**wybierz pozycję **Wyświetl szczegóły**.</span><span class="sxs-lookup"><span data-stu-id="ee295-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="ee295-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="ee295-108">**PowerShell:**</span></span>
1. <span data-ttu-id="ee295-109">Połącz się z usługą Exchange Online przy użyciu programu Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ee295-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="ee295-110">Wykonaj polecenie cmdlet [Get-OrganizationalUnit,](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) aby wyświetlić listę właściwości dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="ee295-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="ee295-111">Spójrz na OrganizationId właściwości.</span><span class="sxs-lookup"><span data-stu-id="ee295-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="ee295-112">Jeśli masz lokalizację danych dla EXO i SPO, możesz określić lokalizację danych dla innych usług, z których można korzystać, z [miejsca, w którym znajdują się dane.](https://products.office.com/where-is-your-data-located)</span><span class="sxs-lookup"><span data-stu-id="ee295-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>