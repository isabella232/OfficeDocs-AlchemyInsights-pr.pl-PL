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
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Konfigurowanie ustawień prywatności w przeglądarce Microsoft Edge

Domyślnie, jeśli przeglądarka Microsoft Edge jest wdrożona na platformach innych niż Windows, dane diagnostyczne i informacje o witrynie nie są wysyłane do firmy Microsoft. Jednak w przypadku wdrożenia przeglądarki Microsoft Edge w systemie Windows 10 dane diagnostyczne i informacje o witrynie są wysyłane zgodnie z ustawieniami danych diagnostycznych systemu [Windows użytkowników.](https://go.microsoft.com/fwlink/?linkid=2132472)

Aby skonfigurować obsługę zbierania danych w organizacji przez program Microsoft Edge, należy użyć następujących zasad grupy:
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) włącza raportowanie danych związanych z awariami i użyciami.
- [Polecenie SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) wysyła informacje o witrynie używane do ulepszania usług firmy Microsoft.

Aby dowiedzieć się więcej, zobacz [Konfigurowanie ustawień zasad.](https://go.microsoft.com/fwlink/?linkid=2132577)
