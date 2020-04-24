---
title: W portalu brakuje urządzeń programu Configuration Manager
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790227"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>W portalu brakuje urządzeń programu Configuration Manager

Aby mogła działać synchronizacja urządzeń, na serwerze lokalnym, który obsługuje rolę punktu połączenia usługi, muszą być dostępne [wymagane internetowe punkty końcowe](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints). Aby rozwiązać problem z synchronizacją urządzeń, przejrzyj plik **CMGatewaySyncUploadWorker.log** znajdujący się w punkcie połączenia usługi.

Dowiedz się więcej o [dołączaniu dzierżawy w programie Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
