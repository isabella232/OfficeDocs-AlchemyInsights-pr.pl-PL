---
title: Ręczne logowanie się do przeglądarki Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678854"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Ręczne logowanie się do przeglądarki Microsoft Edge

Jeśli użytkownik nie jest automatycznie logowany podczas pierwszego uruchomienia, użytkownik może ręcznie zalogować się za pomocą ustawień przeglądarki lub z menu wysuwanego tożsamości. Aby zarządzać logowaniem, Skorzystaj z następujących zasad:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) , aby upewnić się, że użytkownik ma zawsze profil służbowy w programie Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) -ograniczanie logowania do zestawu zaufanych kont.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) — aby wyłączyć logowanie lub zmusić użytkowników do zalogowania się.

