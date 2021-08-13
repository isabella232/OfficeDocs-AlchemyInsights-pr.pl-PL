---
title: W portalu brakuje urządzeń programu Configuration Manager
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966119"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>W portalu brakuje urządzeń programu Configuration Manager

Aby mogła działać synchronizacja urządzeń, na serwerze lokalnym, który obsługuje rolę punktu połączenia usługi, muszą być dostępne [wymagane internetowe punkty końcowe](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints). Aby rozwiązać problem z synchronizacją urządzeń, przejrzyj plik **CMGatewaySyncUploadWorker.log** znajdujący się w punkcie połączenia usługi.

Dowiedz się więcej o [dołączaniu dzierżawy w programie Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
