---
title: Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu z systemem macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491810"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="c7525-102">Ustawianie programu Microsoft Edge jako domyślnej przeglądarki na urządzeniu z systemem macOS</span><span class="sxs-lookup"><span data-stu-id="c7525-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="c7525-103">Użyj jednej z tych dwóch metod, aby ustawić przeglądarkę Microsoft Edge jako domyślną:</span><span class="sxs-lookup"><span data-stu-id="c7525-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="c7525-104">Metoda 1. Flashuj urządzenie za pomocą obrazu systemu macOS, w którym program Microsoft Edge został już ustawiony jako domyślna przeglądarka.</span><span class="sxs-lookup"><span data-stu-id="c7525-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="c7525-105">Metoda 2. Ustaw zasady DefaultBrowserSettingEnabled, aby monitować użytkownika o ustawienie przeglądarki Microsoft Edge jako domyślnej.</span><span class="sxs-lookup"><span data-stu-id="c7525-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="c7525-106">Każda z tych metod umożliwia użytkownikowi zmianę domyślnej przeglądarki.</span><span class="sxs-lookup"><span data-stu-id="c7525-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="c7525-107">Z tego powodu zalecamy wdrożenie zasad DefaultBrowserSettingEnabled, nawet jeśli została użyta metoda 1.</span><span class="sxs-lookup"><span data-stu-id="c7525-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="c7525-108">Jeśli po wdrożeniu zasad użytkownik zmieni przeglądarkę domyślną, zasady monituje użytkownika o ustawienie przeglądarki domyślnej z powrotem na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c7525-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
