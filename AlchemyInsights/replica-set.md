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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110690"
---
# <a name="replica-set"></a>Zestaw replik

AADDS jest również nazywana domeną zarządzaną. Są to w rzeczywistości dwa kontrolery domeny uruchamiane i utrzymywane przez zaplecza. Oba te komputery zawierają jeden główny kontroler dc i jeden kontroler dc replikacji. Kopie zapasowe w usłudze AADDS (domena zarządzana) to zautomatyzowany proces zarządzany przez platformę Azure. W przypadku problemu z domeną zarządzaną pomoc techniczna platformy Azure może pomóc w przywracaniu z kopii zapasowej.

Każdy replikę należy utworzyć w sieci wirtualnej. Każda sieć wirtualna musi być komunikacji równorzędnej z co drugą siecią wirtualną hostową repliki domeny zarządzanej. Ta konfiguracja tworzy topologię sieci siatki, która obsługuje replikację katalogów. Sieć wirtualna może obsługiwać wiele replik zestawów, pod warunkiem że każdy zestaw replik znajduje się w innej wirtualnej podsieci.

Aby uzyskać więcej szczegółowych informacji na temat zestawu replik, zobacz [Zestawy replik pojęć.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
