---
title: Zestaw replik
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714253"
---
# <a name="replica-set"></a>Zestaw replik

Identyfikator AADDS jest również nazywany domeną zarządzaną. W rzeczywistości są to dwa kontrolery domeny uruchamiane i utrzymywane przez zaplecza. Oba te kontrolery obejmują jeden główny kontroler dc i jeden kontroler dc replikacji. Kopie zapasowe w domenie zarządzanej AADDS to zautomatyzowany proces zarządzany przez platformę Azure. W przypadku problemu z domeną zarządzaną pomoc techniczna platformy Azure może pomóc w przywracaniu z kopii zapasowej.

Każdy zestaw replik tworzy się w sieci wirtualnej. Każda sieć wirtualna musi być równorzędna z co drugą siecią wirtualną hostową repliki domeny zarządzanej. Ta konfiguracja tworzy topologię sieci siatki, która obsługuje replikację katalogów. Sieć wirtualna może obsługiwać wiele replik zestawów, pod warunkiem że każdy zestaw replik znajduje się w innej wirtualnej podsieci.

Aby uzyskać więcej szczegółowych informacji na temat zestawu replik, zobacz [zestawy replik pojęć.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
