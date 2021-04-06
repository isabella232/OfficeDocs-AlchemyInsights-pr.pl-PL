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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Narzędzie do diagnostyki usługi dla pulpitu wirtualnego systemu Windows

Pulpit wirtualny systemu Windows (WVD) oferuje narzędzie diagnostyczne, które pozwala administratorom identyfikować błędy za pomocą jednego interfejsu. To narzędzie rejestruje informacje diagnostyczne za każdym razem, gdy WVD jest używane przez osobę z przypisaną rolą WVD. Każdy dziennik zawiera informacje o roli WVD biorącej udział w działaniu, komunikaty o błędach wyświetlane w trakcie sesji oraz informacje o dzierżawie i użytkowniku. Usługę Azure Log Analytics można skonfigurować do przechwytywania dziennika aktywności utworzonego za pomocą narzędzia diagnostycznego, korzystając z następujących kroków:

1. Utwórz obszar roboczy usługi Log Analytics za pomocą [portalu Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) lub programu Azure [PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Połącz komputery z systemem Windows z programem Azure Monitor.](https://go.microsoft.com/fwlink/?linkid=2129913) Uzyskaj identyfikator obszaru roboczego i klucz podstawowy obszaru roboczego. Kreator konfiguracji potrzebuje tych informacji do poprawnego skonfigurowania agenta i zapewnienia komunikacji z monitorem Azure.

1. [Wypychanie danych diagnostycznych do obszaru roboczego](https://go.microsoft.com/fwlink/?linkid=2128284). Możesz wypychać dane diagnostyczne z dzierżawy WVD do analizy dziennika dla swojego obszaru roboczego.

1. [Identyfikowanie i diagnozowanie](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemów wewnętrznych lub zewnętrznych w odniesieniu do WVD.

Aby dowiedzieć się więcej o konfigurowaniu narzędzia diagnostyki usługi dla funkcji WVD, zobacz Korzystanie z funkcji analizy dziennika dla funkcji diagnostyki.