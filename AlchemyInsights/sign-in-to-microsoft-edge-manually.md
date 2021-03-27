---
title: Ręczne logowanie się do programu Microsoft Edge
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
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398667"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="ad552-102">Ręczne logowanie się do programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ad552-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="ad552-103">Jeśli użytkownik nie jest automatycznie zalogowany podczas pierwszego uruchomienia, może ręcznie zalogować się za pomocą ustawień przeglądarki lub wysuwu tożsamości.</span><span class="sxs-lookup"><span data-stu-id="ad552-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="ad552-104">Aby zarządzać logowaniem, użyj następujących zasad:</span><span class="sxs-lookup"><span data-stu-id="ad552-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="ad552-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) — aby mieć pewność, że użytkownik zawsze ma profil służbowy w programie Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="ad552-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="ad552-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) — aby ograniczyć logowanie do zestawu zaufanych kont.</span><span class="sxs-lookup"><span data-stu-id="ad552-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="ad552-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) — aby wyłączyć logowanie lub wymusić zalogowanie się przez użytkowników.</span><span class="sxs-lookup"><span data-stu-id="ad552-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

