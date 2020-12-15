---
title: Narzędzie do diagnostyki usług dla pulpitu wirtualnego systemu Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680227"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="56572-102">Narzędzie do diagnostyki usług dla pulpitu wirtualnego systemu Windows</span><span class="sxs-lookup"><span data-stu-id="56572-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="56572-103">Pulpit wirtualny systemu Windows (WVD) oferuje narzędzie diagnostyczne, które umożliwia administratorom identyfikowanie błędów za pośrednictwem jednego interfejsu.</span><span class="sxs-lookup"><span data-stu-id="56572-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="56572-104">To narzędzie rejestruje informacje dotyczące diagnostyki, ilekroć WVD jest używana przez osobę, która przypisała rolę WVD.</span><span class="sxs-lookup"><span data-stu-id="56572-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="56572-105">Każdy dziennik zawiera informacje dotyczące roli WVD, w której występują działania, komunikaty o błędach wyświetlane podczas sesji oraz informacje o dzierżawie i użytkowniku.</span><span class="sxs-lookup"><span data-stu-id="56572-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="56572-106">Analiza dzienników Azure może być skonfigurowana do przechwytywania dziennika aktywności utworzonego przez narzędzie diagnostyczne.</span><span class="sxs-lookup"><span data-stu-id="56572-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="56572-107">W tym celu wykonaj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="56572-107">Here's how:</span></span>

1. <span data-ttu-id="56572-108">Tworzenie obszaru roboczego Analiza dzienników za pomocą [usługi Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) lub [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="56572-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="56572-109">[Połącz komputery z systemem Windows z usługą Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="56572-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="56572-110">Pobierz identyfikator obszaru roboczego i klucz podstawowy obszaru roboczego.</span><span class="sxs-lookup"><span data-stu-id="56572-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="56572-111">Kreator konfiguracji potrzebuje tych informacji, aby poprawnie skonfigurować agenta i umożliwić mu komunikację z usługą Azure Monitoring.</span><span class="sxs-lookup"><span data-stu-id="56572-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="56572-112">[Przekazywanie danych diagnostycznych do obszaru roboczego](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="56572-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="56572-113">Możesz wypchnąć dane diagnostyczne od dzierżawy WVD do analizy dziennika w obszarze roboczym.</span><span class="sxs-lookup"><span data-stu-id="56572-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="56572-114">[Zidentyfikuj i Diagnozuj problemy](https://go.microsoft.com/fwlink/?linkid=2128338) , które są wewnętrzne lub zewnętrzne w stosunku do WVD.</span><span class="sxs-lookup"><span data-stu-id="56572-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="56572-115">Aby dowiedzieć się więcej o konfigurowaniu narzędzia diagnostycznego usługi dla WVD, zobacz [Korzystanie z funkcji diagnostycznej analizy dzienników](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="56572-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
