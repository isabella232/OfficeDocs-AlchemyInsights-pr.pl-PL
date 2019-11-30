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
ms.openlocfilehash: ec8fb91dfe77cb251579ce23eb0579b114b101d9
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627856"
---
# <a name="data-location"></a><span data-ttu-id="fa506-102">Lokalizacja danych</span><span class="sxs-lookup"><span data-stu-id="fa506-102">Data location</span></span>

<span data-ttu-id="fa506-103">Można wyświetlić lokalizację dzierżawy pakietu Office 365 w centrum administracyjnym lub łącząc się z usługą Exchange Online za pomocą programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fa506-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="fa506-104">**Centrum administracyjne:**</span><span class="sxs-lookup"><span data-stu-id="fa506-104">**Admin center:**</span></span>
1. <span data-ttu-id="fa506-105">Zaloguj się w [centrum administracyjnym](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="fa506-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="fa506-106">Wybierz pozycję **Ustawienia** > **profilu organizacji**.</span><span class="sxs-lookup"><span data-stu-id="fa506-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="fa506-107">W obszarze **Lokalizacja danych**wybierz pozycję **Wyświetl szczegóły**.</span><span class="sxs-lookup"><span data-stu-id="fa506-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="fa506-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="fa506-108">**PowerShell:**</span></span>
1. <span data-ttu-id="fa506-109">Połącz się z usługą Exchange Online przy użyciu programu Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fa506-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="fa506-110">Wykonanie [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) polecenia cmdlet, aby wyświetlić listę właściwości dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="fa506-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="fa506-111">Spójrz na Właściwość OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="fa506-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="fa506-112">Jeśli masz lokalizację danych dla EXO i SPO, można określić lokalizację danych dla innych usług, które mogą być używane z [gdzie znajdują się dane](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="fa506-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>