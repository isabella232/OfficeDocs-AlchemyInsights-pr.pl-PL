---
title: 2419-niemożna włączyć inspekcji
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510438"
---
# <a name="unable-to-enable-unified-auditing"></a>Nie można włączyć ujednoliconej inspekcji

Podczas próby włączenia ujednoliconej inspekcji w organizacji może pojawić się błąd podobny do następujących czynności:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Aby rozwiązać ten problem, wykonaj następujące kroki:

1. [Połącz się z programem Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Uruchom następujące polecenie cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Poczekaj 60 minut, aż poprzednie ustawienie wejdzie w życie.

4. Uruchom następujące polecenie w programie Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Aby uzyskać dodatkowe informacje, zobacz następujące artykuły:

- [Łączenie się z programem Exchange Online PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Włączanie lub wyłączanie wyszukiwania w dzienniku inspekcji](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
