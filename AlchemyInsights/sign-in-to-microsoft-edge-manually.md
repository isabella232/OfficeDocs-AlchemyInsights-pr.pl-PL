---
title: Zaloguj się Microsoft Edge ręcznie
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
- "8332"
- "9004625"
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050776"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Zaloguj się Microsoft Edge ręcznie

Jeśli użytkownik nie jest automatycznie zalogowany podczas pierwszego uruchomienia, może ręcznie zalogować się za pomocą ustawień przeglądarki lub wysuwu tożsamości. Aby zarządzać logowaniem, użyj następujących zasad:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) — aby mieć pewność, że użytkownik zawsze ma profil służbowy w Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) — aby ograniczyć logowanie do zestawu zaufanych kont.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) — aby wyłączyć logowanie lub wymusić zalogowanie się przez użytkowników.

