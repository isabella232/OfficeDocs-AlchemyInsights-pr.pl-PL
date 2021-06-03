---
title: Ochrona DLP punktu końcowego nie jest wdrożona na urządzeniu użytkownika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731591"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="a33c0-102">Ochrona DLP punktu końcowego nie jest wdrożona na urządzeniu użytkownika</span><span class="sxs-lookup"><span data-stu-id="a33c0-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="a33c0-103">Jeśli ustawienie zapobieganie utracie danych w punkcie końcowym (DLP, Endpoint data loss prevention) nie ma zastosowania do urządzenia użytkownika, potwierdź, że spełniasz następujące wymagania:</span><span class="sxs-lookup"><span data-stu-id="a33c0-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="a33c0-104">Windows 10 x64 kompilacja 1809 lub nowszy jest instalowana na urządzeniu.</span><span class="sxs-lookup"><span data-stu-id="a33c0-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="a33c0-105">Zainstalowany jest klient ochrony przed złośliwym oprogramowaniem w wersji 4.18.2009.7 lub nowszej.</span><span class="sxs-lookup"><span data-stu-id="a33c0-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="a33c0-106">Urządzenie jest **jednym z** tych:</span><span class="sxs-lookup"><span data-stu-id="a33c0-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="a33c0-107">Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="a33c0-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="a33c0-108">Dołączyć do hybrydowej usługi Azure AD</span><span class="sxs-lookup"><span data-stu-id="a33c0-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="a33c0-109">Zarejestrowano AAD</span><span class="sxs-lookup"><span data-stu-id="a33c0-109">AAD registered</span></span>

- <span data-ttu-id="a33c0-110">Aby wymusić akcje zasad, upewnij się, że Chromium Microsoft Edge jest zainstalowana na urządzeniu końcowym.</span><span class="sxs-lookup"><span data-stu-id="a33c0-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="a33c0-111">Aby uzyskać dodatkowe wymagania dotyczące wdrażania ochrony przed utratą danych w punktach końcowych, zobacz Wprowadzenie do ochrony przed utratą danych [w punkcie końcowym.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="a33c0-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>