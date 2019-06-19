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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="b122a-102">Nie można włączyć inspekcji jednolity</span><span class="sxs-lookup"><span data-stu-id="b122a-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="b122a-103">Podczas próby włączenia inspekcji ujednoliconej organizacji usługi Office 365, może wystąpić błąd podobny następujących czynności:</span><span class="sxs-lookup"><span data-stu-id="b122a-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="b122a-104">Aby rozwiązać ten problem, wykonaj następujące kroki:</span><span class="sxs-lookup"><span data-stu-id="b122a-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="b122a-105">[Podłącz do wymiany Online programu Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="b122a-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="b122a-106">Uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="b122a-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="b122a-107">Poczekaj, aż 60 minut dla poprzedniego ustawienia zostały wprowadzone.</span><span class="sxs-lookup"><span data-stu-id="b122a-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="b122a-108">Uruchom następujące polecenie w programie PowerShell Online programu Exchange:</span><span class="sxs-lookup"><span data-stu-id="b122a-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="b122a-109">Aby uzyskać dodatkowe informacje zobacz następujące artykuły:</span><span class="sxs-lookup"><span data-stu-id="b122a-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="b122a-110">Połączyć się wieloczynnikowe uwierzytelnianie za pomocą środowiska PowerShell Online programu Exchange</span><span class="sxs-lookup"><span data-stu-id="b122a-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="b122a-111">Włączanie lub wyłączanie wyszukiwania dziennika inspekcji usługi Office 365</span><span class="sxs-lookup"><span data-stu-id="b122a-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
