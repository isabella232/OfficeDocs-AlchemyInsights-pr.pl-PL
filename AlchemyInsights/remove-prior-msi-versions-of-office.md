---
title: Usuwanie wcześniejszych wersji MSI pakietu Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680728"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="142d4-102">Usuwanie wcześniejszych wersji MSI pakietu Office</span><span class="sxs-lookup"><span data-stu-id="142d4-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="142d4-103">Zalecamy usunięcie wcześniejszych wersji Instalatora Windows (MSI) pakietu Office przed zainstalowaniem usługi Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="142d4-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="142d4-104">Poniżej opisano, jak to zrobić:</span><span class="sxs-lookup"><span data-stu-id="142d4-104">Here's how to do this:</span></span>

1. <span data-ttu-id="142d4-105">Jeśli do zainstalowania pakietu Office użyto Instalatora MSI, możesz odinstalować pakiet Office za pomocą narzędzia wdrażania pakietu Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="142d4-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="142d4-106">Elementu RemoveMSI można użyć w pliku **configuration.xml** .</span><span class="sxs-lookup"><span data-stu-id="142d4-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="142d4-107">Postępuj zgodnie z instrukcjami w tym artykule: [zabezpieczenia pakietu Office 365 — Centrum zgodności &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="142d4-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>