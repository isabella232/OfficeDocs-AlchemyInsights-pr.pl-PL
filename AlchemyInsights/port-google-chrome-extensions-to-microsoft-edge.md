---
title: Przenoszenie rozszerzeń Google Chrome do przeglądarki Microsoft Edge (chrom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678986"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Przenoszenie rozszerzeń Google Chrome do przeglądarki Microsoft Edge (chrom)

[Przenoszenie rozszerzeń Google Chrome do programu Microsoft Edge (chrom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)jest łatwe. W większości przypadków wymagane są tylko minimalne zmiany w celu uruchomienia tych rozszerzeń w przeglądarce Microsoft Edge.

Interfejsy API rozszerzenia i klucze manifestu obsługiwane przez aplikację Google Chrome są zgodne ze standardem Code w przeglądarce Microsoft Edge. Program Microsoft Edge nie obsługuje jednak interfejsów API rozszerzeń Service. GCM, Chrome. Identity. getaccounts, Chrome. Identity. getAuthToken i Chrome. instanceID.