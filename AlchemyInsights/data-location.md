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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207271"
---
# <a name="data-location"></a><span data-ttu-id="63cc7-102">Lokalizacja danych</span><span class="sxs-lookup"><span data-stu-id="63cc7-102">Data location</span></span>

<span data-ttu-id="63cc7-103">Można wyświetlić lokalizację dzierżawy pakietu Office 365 w centrum administracyjnym lub łącząc się z usługą Exchange Online za pomocą programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="63cc7-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="63cc7-104">**Centrum administracyjne:**</span><span class="sxs-lookup"><span data-stu-id="63cc7-104">**Admin center:**</span></span>
1. <span data-ttu-id="63cc7-105">Zaloguj się w [centrum administracyjnym](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="63cc7-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="63cc7-106">Wybierz pozycję **Ustawienia** > **profilu organizacji**.</span><span class="sxs-lookup"><span data-stu-id="63cc7-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="63cc7-107">W obszarze **Lokalizacja danych**wybierz pozycję **Wyświetl szczegóły**.</span><span class="sxs-lookup"><span data-stu-id="63cc7-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="63cc7-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="63cc7-108">**PowerShell:**</span></span>
1. <span data-ttu-id="63cc7-109">Połącz się z usługą Exchange Online przy użyciu programu Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="63cc7-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="63cc7-110">Wykonanie [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) polecenia cmdlet, aby wyświetlić listę właściwości dzierżawy.</span><span class="sxs-lookup"><span data-stu-id="63cc7-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="63cc7-111">Spójrz na Właściwość OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="63cc7-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="63cc7-112">Jeśli masz lokalizację danych dla EXO i SPO, można określić lokalizację danych dla innych usług, które mogą być używane z [gdzie znajdują się dane](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="63cc7-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>