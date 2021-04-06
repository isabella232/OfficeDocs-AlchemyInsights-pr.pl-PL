---
title: Narzędzie do diagnostyki usługi dla pulpitu wirtualnego systemu Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595864"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="13bfc-102">Narzędzie do diagnostyki usługi dla pulpitu wirtualnego systemu Windows</span><span class="sxs-lookup"><span data-stu-id="13bfc-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="13bfc-103">Pulpit wirtualny systemu Windows (WVD) oferuje narzędzie diagnostyczne, które pozwala administratorom identyfikować błędy za pomocą jednego interfejsu.</span><span class="sxs-lookup"><span data-stu-id="13bfc-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="13bfc-104">To narzędzie rejestruje informacje diagnostyczne za każdym razem, gdy WVD jest używane przez osobę z przypisaną rolą WVD.</span><span class="sxs-lookup"><span data-stu-id="13bfc-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="13bfc-105">Każdy dziennik zawiera informacje o roli WVD biorącej udział w działaniu, komunikaty o błędach wyświetlane w trakcie sesji oraz informacje o dzierżawie i użytkowniku.</span><span class="sxs-lookup"><span data-stu-id="13bfc-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="13bfc-106">Usługę Azure Log Analytics można skonfigurować do przechwytywania dziennika aktywności utworzonego za pomocą narzędzia diagnostycznego, korzystając z następujących kroków:</span><span class="sxs-lookup"><span data-stu-id="13bfc-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="13bfc-107">Utwórz obszar roboczy usługi Log Analytics za pomocą [portalu Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) lub programu Azure [PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="13bfc-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="13bfc-108">[Połącz komputery z systemem Windows z programem Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="13bfc-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="13bfc-109">Uzyskaj identyfikator obszaru roboczego i klucz podstawowy obszaru roboczego.</span><span class="sxs-lookup"><span data-stu-id="13bfc-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="13bfc-110">Kreator konfiguracji potrzebuje tych informacji do poprawnego skonfigurowania agenta i zapewnienia komunikacji z monitorem Azure.</span><span class="sxs-lookup"><span data-stu-id="13bfc-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="13bfc-111">[Wypychanie danych diagnostycznych do obszaru roboczego](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="13bfc-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="13bfc-112">Możesz wypychać dane diagnostyczne z dzierżawy WVD do analizy dziennika dla swojego obszaru roboczego.</span><span class="sxs-lookup"><span data-stu-id="13bfc-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="13bfc-113">[Identyfikowanie i diagnozowanie](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemów wewnętrznych lub zewnętrznych w odniesieniu do WVD.</span><span class="sxs-lookup"><span data-stu-id="13bfc-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="13bfc-114">Aby dowiedzieć się więcej o konfigurowaniu narzędzia diagnostyki usługi dla funkcji WVD, zobacz Korzystanie z funkcji analizy dziennika dla funkcji diagnostyki.</span><span class="sxs-lookup"><span data-stu-id="13bfc-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>