---
title: Nie można ustawić lub wyświetlić zasad Zezwalania na zakup usługi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158571"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie można ustawić lub wyświetlić zasad Zezwalania na zakup usługi

Podczas próby ustawienia lub wyświetlenia zasad Zezwalania na zakup usługi wyświetlany jest następujący komunikat o błędzie:

*HandleError: Nie można pobrać zasady produktu z PolicyId "AllowSelfServicePurchase", ErrorMessage — połączenie źródłowe zostało zamknięte: Wystąpił nieoczekiwany błąd podczas wysyłania.*

Może to być spowodowane starszą wersją zabezpieczeń warstwy transportowej (TLS). Aby połączyć usługę MSCommerce, musisz użyć tls 1.2 lub więcej.  

Spróbuj wykonać następujące kroki, aby włączyć/ustawić protokół TLS na 1.2, zweryfikować i ponowić próbę.
 1. W wierszu polecenia programu PowerShell (PS C:\) wprowadź następujące polecenie, aby ustawić protokół TLS na wersję 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Sprawdź używane protokoły TLS za pomocą następującego polecenia:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. W razie potrzeby ponów próbę polecenia Pobierz lub Aktualizuj.

