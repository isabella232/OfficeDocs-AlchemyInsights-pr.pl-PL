---
title: Microsoft Edge ustawień prywatności
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
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114182"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge ustawień prywatności

Domyślnie, jeśli Microsoft Edge na platformach Windows, dane diagnostyczne i informacje o witrynie nie są wysyłane do firmy Microsoft. Jednak jeśli Microsoft Edge na urządzeniach Windows 10, dane diagnostyczne i informacje o witrynie są wysyłane zgodnie z ustawieniami usługi Windows [danych diagnostycznych.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Aby skonfigurować sposób Microsoft Edge zbierania danych w organizacji, należy użyć następujących zasad grupy:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Te zasady umożliwiają raportowanie użycia i danych związanych z awariami.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Te zasady wysyłają informacje o witrynie używane do ulepszania usługi firmy Microsoft.

Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)