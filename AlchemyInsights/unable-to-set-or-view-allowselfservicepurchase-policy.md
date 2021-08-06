---
title: Nie można ustawić ani wyświetlić zasad AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020202"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie można ustawić ani wyświetlić zasad AllowSelfServicePurchase

Podczas próby ustawienia lub wyświetlenia zasad AllowSelfServicePurchase jest wyświetlany następujący komunikat o błędzie:

*HandleError: Nie można pobrać zasad produktu przy użyciu wartości PolicyId 'AllowSelfServicePurchase', ErrorMessage — połączenie źródłowe zostało zamknięte: Wystąpił nieoczekiwany błąd podczas wysyłania.*

Może to być spowodowane starszą wersją usługi Transport Layer Security (TLS). Aby połączyć usługę MS Commerce, musisz użyć usługi TLS 1.2 lub większej.  

Spróbuj wykonać poniższe czynności, aby włączyć/ustawić dla protokołu TLS wartość 1.2, zweryfikować i ponowić próbę.
 1. W wierszu polecenia programu PowerShell (PS C: wprowadź następujące polecenie, aby ustawić protokół \) TLS na wersję 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Sprawdź, czy są używani protokoły TLS, za pomocą następującego polecenia:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. W razie potrzeby ponownie spróbuj wykonać polecenia Pobierz lub Aktualizuj.

