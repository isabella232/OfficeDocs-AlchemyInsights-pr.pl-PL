---
title: Wyłączanie skanowania sieci
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481964"
---
# <a name="disable-network-scan"></a><span data-ttu-id="ef76c-102">Wyłączanie skanowania sieci</span><span class="sxs-lookup"><span data-stu-id="ef76c-102">Disable network scan</span></span>

<span data-ttu-id="ef76c-103">Skany udziału sieciowego mogą mieć wpływ na wydajność.</span><span class="sxs-lookup"><span data-stu-id="ef76c-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="ef76c-104">Aby upewnić się, że klient domyślnie nie skanuje udziałów/plików sieciowych, skonfiguruj następujące ustawienia w aplikacji Windows Defender na **Wartość Prawda:**</span><span class="sxs-lookup"><span data-stu-id="ef76c-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="ef76c-105">Disable JednakoweDaneMappedNetworkDrivesForFull Jednakowe</span><span class="sxs-lookup"><span data-stu-id="ef76c-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="ef76c-106">Disable JednakoweNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="ef76c-106">DisableScanningNetworkFiles</span></span>