---
title: 2419-nie można włączyć-Inspekcja
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767609"
---
# <a name="unable-to-enable-unified-auditing"></a>Nie można włączyć ujednoliconej inspekcji

Podczas próby włączenia funkcji ujednoliconej inspekcji dla organizacji może zostać wyświetlony komunikat o błędzie podobny do następującego:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Aby rozwiązać ten problem, wykonaj następujące czynności:

1. [Nawiązywanie połączenia z programem Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Uruchom następujące polecenie cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Poczekaj na 60 minut, zanim poprzednie ustawienie zostanie zastosowane.

4. Uruchom następujące polecenie w usłudze Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Aby uzyskać dodatkowe informacje, zobacz następujące artykuły:

- [Nawiązywanie połączenia z programem Exchange Online PowerShell przy użyciu uwierzytelniania wieloskładnikowego](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Włączanie lub wyłączanie wyszukiwania w dzienniku inspekcji](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
