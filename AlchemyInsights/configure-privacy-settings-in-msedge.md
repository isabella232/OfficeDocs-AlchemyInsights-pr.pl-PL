---
title: Konfigurowanie ustawień prywatności w przeglądarce Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405101"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="ea71b-102">Konfigurowanie ustawień prywatności w przeglądarce Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ea71b-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="ea71b-103">Domyślnie, jeśli przeglądarka Microsoft Edge jest wdrożona na platformach innych niż Windows, dane diagnostyczne i informacje o witrynie nie są wysyłane do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea71b-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="ea71b-104">Jednak w przypadku wdrożenia przeglądarki Microsoft Edge w systemie Windows 10 dane diagnostyczne i informacje o witrynie są wysyłane zgodnie z ustawieniami danych diagnostycznych systemu [Windows użytkowników.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="ea71b-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="ea71b-105">Aby skonfigurować obsługę zbierania danych w organizacji przez program Microsoft Edge, należy użyć następujących zasad grupy:</span><span class="sxs-lookup"><span data-stu-id="ea71b-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="ea71b-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) włącza raportowanie danych związanych z awariami i użyciami.</span><span class="sxs-lookup"><span data-stu-id="ea71b-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="ea71b-107">[Polecenie SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) wysyła informacje o witrynie używane do ulepszania usług firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea71b-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="ea71b-108">Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="ea71b-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
