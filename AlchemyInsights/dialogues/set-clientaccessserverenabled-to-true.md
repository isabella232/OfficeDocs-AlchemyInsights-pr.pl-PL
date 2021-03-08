---
title: Set ClientAccessServerEnabled to True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525966"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Set ClientAccessServerEnabled to True

Jeśli nie możesz otworzyć zaszyfrowanej wiadomości e-mail i zamiast tego zobaczysz **załącznik,** wykonaj następujące czynności:

1. Połącz się z programem PowerShell dla usługi Exchange Online.

> [!NOTE]
> Aby nawiązać połączenie z programem PowerShell dla usługi Exchange Online, musisz zalogować się przy użyciu konta administratora globalnego lub administratora programu Exchange.

   a. Otwórz program Windows PowerShell, a następnie uruchom następujące polecenie: `$UserCredential = Get-Credential`
b. W **oknie dialogowym Żądanie** poświadczeń programu Windows PowerShell wprowadź poświadczenia konta służbowego i hasło, c. Kliknij przycisk **OK**. 

2. Uruchom następujące polecenie, aby utworzyć nową sesję:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Uruchom następujące polecenie:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Polecenie `Get-IRMConfiguration` Uruchom.

4. Sprawdź ustawienie **ClientAccessServerEnabled.** 

    a. Jeśli **ustawienie ClientAccessServerEnabled** ma wartość False (Fałsz), uruchom następujące polecenie cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Zawsze zamykaj sesję programu PowerShell za pomocą następującego polecenia: `Remove-PSSession $Session`

Aby uzyskać więcej informacji, zobacz program [PowerShell dla usługi Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

