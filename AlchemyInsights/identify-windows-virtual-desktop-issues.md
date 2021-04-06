---
title: Identyfikowanie problemów z pulpitem wirtualnym systemu Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595855"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="44545-102">Identyfikowanie problemów z pulpitem wirtualnym systemu Windows</span><span class="sxs-lookup"><span data-stu-id="44545-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="44545-103">Narzędzie Diagnostyka pulpitu wirtualnego systemu Windows używa tylko jednego polecenia cmdlet programu PowerShell, ale zawiera wiele opcjonalnych parametrów, które ułatwiają zawężenie i odizolowanie problemów.</span><span class="sxs-lookup"><span data-stu-id="44545-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="44545-104">Aby rozpocząć:</span><span class="sxs-lookup"><span data-stu-id="44545-104">To get started:</span></span> 

1. <span data-ttu-id="44545-105">Pobierz i zaimportuj moduł programu Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="44545-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="44545-106">Aby uzyskać szczegółowe informacje, zobacz Polecenia cmdlet pulpitu [wirtualnego systemu Windows dla programu Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="44545-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="44545-107">Uruchom następujące polecenie cmdlet, aby zalogować się do swojego konta:</span><span class="sxs-lookup"><span data-stu-id="44545-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="44545-108">Przykład: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="44545-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="44545-109">**UWAGA:** Wszystkie zapytania używające programu PowerShell muszą zawierać parametry -UserName lub -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="44545-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="44545-110">Aby uzyskać informacje na temat możliwości monitorowania, zobacz Używanie analizy [dziennika dla funkcji diagnostyki.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="44545-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="44545-111">Aby filtrować działania diagnostyczne według użytkownika, uruchom następujące polecenie cmdlet:</span><span class="sxs-lookup"><span data-stu-id="44545-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="44545-112">Przykład: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="44545-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="44545-113">Istnieje lista filtrów, które można uruchomić w celu zdiagnozowania problemów.</span><span class="sxs-lookup"><span data-stu-id="44545-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="44545-114">Aby dowiedzieć się więcej o diagnozowaniu problemów, zobacz Identyfikowanie i [diagnozowanie problemów z pulpitem wirtualnym systemu Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="44545-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="44545-115">Aby dowiedzieć się więcej o typowych błędach, zobacz [Typowe błędy sen sens.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)</span><span class="sxs-lookup"><span data-stu-id="44545-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
