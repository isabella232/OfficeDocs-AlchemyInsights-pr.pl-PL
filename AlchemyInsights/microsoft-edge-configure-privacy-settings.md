---
title: Microsoft Edge — Konfigurowanie ustawień prywatności
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
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678855"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="b1d62-102">Microsoft Edge — Konfigurowanie ustawień prywatności</span><span class="sxs-lookup"><span data-stu-id="b1d62-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="b1d62-103">Domyślnie, jeśli program Microsoft Edge jest wdrożony na platformach innych niż Windows, dane diagnostyczne i informacje o witrynie nie są wysyłane do firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1d62-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="b1d62-104">Jeśli jednak program Microsoft Edge jest wdrożony w systemie Windows 10, dane diagnostyczne i informacje o witrynie są wysyłane zgodnie z [ustawieniami danych diagnostycznych użytkowników systemu Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="b1d62-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="b1d62-105">Aby skonfigurować sposób, w jaki program Microsoft Edge obsługuje zbieranie danych dla organizacji, użyj następujących zasad grupy:</span><span class="sxs-lookup"><span data-stu-id="b1d62-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="b1d62-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ta zasada umożliwia raportowanie danych dotyczących użycia i niezwiązanych z awariami.</span><span class="sxs-lookup"><span data-stu-id="b1d62-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="b1d62-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ta zasada wysyła informacje o witrynie, które są używane do ulepszania usług firmy Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b1d62-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="b1d62-108">Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="b1d62-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>