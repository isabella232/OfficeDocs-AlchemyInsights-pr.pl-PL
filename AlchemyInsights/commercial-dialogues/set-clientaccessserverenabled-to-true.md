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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320366"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Ustaw wartość ClientAccessServerEnabled na True

Jeśli nie możesz otworzyć zaszyfrowanej wiadomości e-mail i zamiast tego zobaczysz **załącznik,** wykonaj następujące czynności:

1. Połączenie do Exchange Online PowerShell.

    **Uwaga:** aby nawiązać połączenie z programem Exchange Online PowerShell, musisz zalogować się przy użyciu konta administratora globalnego Exchange administratora.

   a. Otwórz Windows PowerShell, a następnie uruchom następujące polecenie:`$UserCredential = Get-Credential`
   b. W **oknie Windows PowerShell poświadczeń** wprowadź swoje konto służbowe i hasło, c. Kliknij przycisk **OK**. 

2. Uruchom następujące polecenie, aby utworzyć nową sesję:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Uruchom następujące polecenie:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Polecenie `Get-IRMConfiguration` Uruchom.

4. Sprawdź ustawienie **ClientAccessServerEnabled.** 

    a. Jeśli **ustawienie ClientAccessServerEnabled** ma ustawioną wartość **False,** uruchom następujące polecenie cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Porada:** Zawsze zamykaj sesję programu PowerShell za pomocą następującego polecenia: `Remove-PSSession $Session`

Aby uzyskać więcej informacji, zobacz [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

