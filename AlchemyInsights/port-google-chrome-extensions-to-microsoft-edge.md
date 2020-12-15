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
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="6b52c-102">Przenoszenie rozszerzeń Google Chrome do przeglądarki Microsoft Edge (chrom)</span><span class="sxs-lookup"><span data-stu-id="6b52c-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="6b52c-103">[Przenoszenie rozszerzeń Google Chrome do programu Microsoft Edge (chrom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)jest łatwe.</span><span class="sxs-lookup"><span data-stu-id="6b52c-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="6b52c-104">W większości przypadków wymagane są tylko minimalne zmiany w celu uruchomienia tych rozszerzeń w przeglądarce Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6b52c-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="6b52c-105">Interfejsy API rozszerzenia i klucze manifestu obsługiwane przez aplikację Google Chrome są zgodne ze standardem Code w przeglądarce Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6b52c-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="6b52c-106">Program Microsoft Edge nie obsługuje jednak interfejsów API rozszerzeń Service. GCM, Chrome. Identity. getaccounts, Chrome. Identity. getAuthToken i Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="6b52c-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>