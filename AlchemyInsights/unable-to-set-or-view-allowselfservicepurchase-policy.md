---
title: Nie można ustawić lub wyświetlić zasad AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735209"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nie można ustawić lub wyświetlić zasad AllowSelfServicePurchase

Podczas próby ustawienia lub wyświetlenia zasad AllowSelfServicePurchase jest wyświetlany następujący komunikat o błędzie:

*HandleError: nie można pobrać zasad dotyczących produktu z PolicyId "AllowSelfServicePurchase", ErrorMessage — połączenie podstawowe zostało zakończone: Wystąpił nieoczekiwany błąd podczas wysyłania.*

Może to być spowodowane starszą wersją protokołu TLS (Transport Layer Security). Aby połączyć usługę MSCommerce, musisz użyć protokołu TLS 1,2 lub nowszego.  

Spróbuj wykonać poniższe czynności, aby włączyć/ustawić protokół TLS na 1,2, sprawdź, a następnie ponów próbę.
 1. W wierszu polecenia programu PowerShell (PS C: \) wprowadź następujące polecenie, aby ustawić protokół TLS w wersji 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Sprawdź używane protokoły TLS za pomocą następującego polecenia:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Spróbuj ponownie wykonać polecenia Pobierz lub Aktualizuj stosownie do potrzeb.

