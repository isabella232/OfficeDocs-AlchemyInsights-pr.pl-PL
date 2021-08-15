---
title: Ustaw wartość ClientAccessServerEnabled na True
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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994875"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ustaw wartość ClientAccessServerEnabled na True

Jeśli nie możesz otworzyć zaszyfrowanej wiadomości e-mail i zamiast tego zobaczysz **załącznik,** wykonaj następujące czynności:

1. Połączenie do Exchange Online PowerShell.

> [!NOTE]
> Aby nawiązać połączenie Exchange Online programu PowerShell, musisz zalogować się przy użyciu konta administratora globalnego Exchange administratora.

   a. Otwórz Windows PowerShell, a następnie uruchom następujące polecenie:`$UserCredential = Get-Credential`
b. W **oknie Windows PowerShell poświadczenia** poświadczenia wprowadź swoje konto służbowe i hasło, c. Kliknij przycisk **OK**. 

2. Uruchom następujące polecenie, aby utworzyć nową sesję:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Uruchom następujące polecenie:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Polecenie `Get-IRMConfiguration` Uruchom.

4. Sprawdź ustawienie **ClientAccessServerEnabled.** 

    a. Jeśli **ustawienie ClientAccessServerEnabled** ma ustawioną wartość **False,** uruchom następujące polecenie cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Zawsze zamykaj sesję programu PowerShell za pomocą następującego polecenia: `Remove-PSSession $Session`

Aby uzyskać więcej informacji, zobacz [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

