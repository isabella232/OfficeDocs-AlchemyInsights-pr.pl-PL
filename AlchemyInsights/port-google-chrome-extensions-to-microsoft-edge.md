---
title: Przenoszenie rozszerzeń Google Chrome na Microsoft Edge (Chromium)
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
- "8297"
- "9004617"
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973707"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Przenoszenie rozszerzeń Google Chrome na Microsoft Edge (Chromium)

Przenoszenie rozszerzeń Google Chrome do programu [Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)jest łatwe. W większości przypadków do uruchomienia tych rozszerzeń na tym Microsoft Edge są potrzebne tylko minimalne Microsoft Edge.

Interfejsy API rozszerzenia i klucze manifestu obsługiwane przez program Google Chrome są zgodne z kodami Microsoft Edge. Jednak Microsoft Edge nie obsługuje interfejsów API rozszerzenia chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken i chrome.instanceID.