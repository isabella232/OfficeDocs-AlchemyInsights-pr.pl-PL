---
title: 2419-do enable inspekcji
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065681"
---
# <a name="unable-to-enable-unified-auditing"></a>Nie można włączyć inspekcji jednolity

Podczas próby włączenia inspekcji ujednoliconej organizacji usługi Office 365, może wystąpić błąd podobny następujących czynności:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Aby rozwiązać ten problem, wykonaj następujące kroki:

1. [Podłącz do wymiany Online programu Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Uruchom następujące polecenia:

   ```
   Enable-OrganizationCustomization
   ```

3. Poczekaj, aż 60 minut dla poprzedniego ustawienia zostały wprowadzone.

4. Uruchom następujące polecenie w programie PowerShell Online programu Exchange:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Aby uzyskać dodatkowe informacje zobacz następujące artykuły:

- [Połączyć się wieloczynnikowe uwierzytelnianie za pomocą środowiska PowerShell Online programu Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Włączanie lub wyłączanie wyszukiwania dziennika inspekcji usługi Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
