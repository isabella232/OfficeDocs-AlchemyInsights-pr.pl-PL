---
title: Włączanie Exchange Online DKIM dla określonej domeny przy użyciu programu PowerShell
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070320"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Włączanie Exchange Online DKIM dla określonej domeny przy użyciu programu PowerShell

Jeśli nie możesz utworzyć rekordów DNS DKIM w centrum administracyjnym, spróbuj użyć programu Exchange Online PowerShell. 

Aby utworzyć rekord DNS DKIM przy Exchange Online PowerShell, wykonaj następujące czynności:

1. Otwórz Windows PowerShell jako administrator i uruchom następujące polecenia w opisanej kolejności:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Jeśli masz problemy z połączeniem się z programem Exchange Online PowerShell, zobacz Połączenie się z [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Po na połączeniu się z programem Exchange Online PowerShell uruchom następujące polecenie:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Po pomyślnym wykonaniu powyższego polecenia uruchom następujące polecenie, aby zakończyć sesję programu PowerShell Exchange Online powershell:

    `Remove-PSSession $Session` 



