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
# <a name="identify-windows-virtual-desktop-issues"></a>Identyfikowanie problemów z pulpitem wirtualnym systemu Windows

Narzędzie Diagnostyka pulpitu wirtualnego systemu Windows używa tylko jednego polecenia cmdlet programu PowerShell, ale zawiera wiele opcjonalnych parametrów, które ułatwiają zawężenie i odizolowanie problemów. Aby rozpocząć: 

1. Pobierz i zaimportuj moduł programu Windows Virtual Desktop PowerShell. Aby uzyskać szczegółowe informacje, zobacz Polecenia cmdlet pulpitu [wirtualnego systemu Windows dla programu Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Uruchom następujące polecenie cmdlet, aby zalogować się do swojego konta:
    
    Przykład: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**UWAGA:** Wszystkie zapytania używające programu PowerShell muszą zawierać parametry -UserName lub -ActivityID. Aby uzyskać informacje na temat możliwości monitorowania, zobacz Używanie analizy [dziennika dla funkcji diagnostyki.](https://go.microsoft.com/fwlink/?linkid=2126847)

Aby filtrować działania diagnostyczne według użytkownika, uruchom następujące polecenie cmdlet:

Przykład: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Istnieje lista filtrów, które można uruchomić w celu zdiagnozowania problemów. Aby dowiedzieć się więcej o diagnozowaniu problemów, zobacz Identyfikowanie i [diagnozowanie problemów z pulpitem wirtualnym systemu Windows.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Aby dowiedzieć się więcej o typowych błędach, zobacz [Typowe błędy sen sens.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)
