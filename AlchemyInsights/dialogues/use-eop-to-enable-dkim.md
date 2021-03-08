---
title: Włączanie funkcji DKIM dla określonej domeny przy użyciu programu PowerShell dla usługi Exchange Online
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525239"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Włączanie funkcji DKIM dla określonej domeny przy użyciu programu PowerShell dla usługi Exchange Online

Jeśli nie możesz utworzyć rekordów DNS DKIM w centrum administracyjnym, spróbuj użyć programu PowerShell dla usługi Exchange Online. 

Aby utworzyć rekord DNS DKIM przy użyciu programu PowerShell dla usługi Exchange Online, wykonaj następujące czynności:

1. Otwórz program Windows PowerShell jako administrator i uruchom następujące polecenia w opisanej sekwencji:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jeśli masz problem z nawiązaniem połączenia z programem PowerShell dla usługi Exchange Online, zobacz [Nawiązywanie połączenia z programem PowerShell dla usługi Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Po na połączeniu się z programem PowerShell dla usługi Exchange Online uruchom następujące polecenie:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po pomyślnym wykonaniu powyższego polecenia uruchom następujące polecenie, aby zakończyć sesję programu PowerShell dla usługi Exchange Online:

    `Remove-PSSession $Session` 



