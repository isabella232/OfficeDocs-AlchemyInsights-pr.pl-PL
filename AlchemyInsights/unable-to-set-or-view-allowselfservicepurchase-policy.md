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
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826101"
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

