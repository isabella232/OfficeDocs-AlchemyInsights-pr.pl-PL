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
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge — Konfigurowanie ustawień prywatności

Domyślnie, jeśli program Microsoft Edge jest wdrożony na platformach innych niż Windows, dane diagnostyczne i informacje o witrynie nie są wysyłane do firmy Microsoft. Jeśli jednak program Microsoft Edge jest wdrożony w systemie Windows 10, dane diagnostyczne i informacje o witrynie są wysyłane zgodnie z [ustawieniami danych diagnostycznych użytkowników systemu Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Aby skonfigurować sposób, w jaki program Microsoft Edge obsługuje zbieranie danych dla organizacji, użyj następujących zasad grupy:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ta zasada umożliwia raportowanie danych dotyczących użycia i niezwiązanych z awariami.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ta zasada wysyła informacje o witrynie, które są używane do ulepszania usług firmy Microsoft.

Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).