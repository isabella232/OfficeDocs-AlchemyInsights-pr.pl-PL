---
title: Włącz urządzenie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256875"
---
# <a name="enable-device"></a><span data-ttu-id="94e39-102">Włącz urządzenie</span><span class="sxs-lookup"><span data-stu-id="94e39-102">Enable Device</span></span>

<span data-ttu-id="94e39-103">**Aby włączyć urządzenie przy użyciu polecenia programu PowerShell**</span><span class="sxs-lookup"><span data-stu-id="94e39-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="94e39-104">Uruchom następujące polecenia:</span><span class="sxs-lookup"><span data-stu-id="94e39-104">Run the following commands:</span></span>

- <span data-ttu-id="94e39-105">Aby uzyskać obiekt urządzenia: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="94e39-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="94e39-106">Aby włączyć urządzenie: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="94e39-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="94e39-107">Aby uzyskać więcej informacji na temat konfigurowania sprzężenia hybrydowego w domenach zarządzanych, zobacz [Konfigurowanie sprzężenia hybrydowego.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)</span><span class="sxs-lookup"><span data-stu-id="94e39-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
