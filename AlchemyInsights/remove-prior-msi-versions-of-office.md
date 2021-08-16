---
title: Usuń wcześniejsze wersje programu z Office MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 45e3cac521bc1c2a90dc7d3ddd4958233c3cf7bbd2ea007e581f343bca7b5631
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023784"
---
# <a name="remove-prior-msi-versions-of-office"></a>Usuń wcześniejsze wersje programu z Office MSI

Przed rozpoczęciem instalacji Windows instalatora (MSI) zaleca się usunięcie Office instalatora Office 365 ProPlus. Poniżej opisano, jak to zrobić:

1. Jeśli do instalacji pakietu Office został użyty Office (ODT, Deployment Tool), możesz odinstalować pakiet Office. Możesz użyć elementu RemoveMSI w pliku **configuration.xml** pliku.
1. Postępuj zgodnie z instrukcjami w tym artykule: [Office 365 zabezpieczeń & zgodności.](https://go.microsoft.com/fwlink/p/?linkid=2077143)