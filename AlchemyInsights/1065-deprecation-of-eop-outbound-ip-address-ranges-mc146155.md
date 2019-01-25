---
title: 1065 oczekiwany podniesienie uprawnień wychodzących rangesMC146155 adres IP
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29483204"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Oczekiwany podniesienie poziomu uprawnień wychodzących zakresów adresów IP

Wykryto potencjalny problem z organizacji, (Jeśli nie zostaną usunięte przez 26 października 2018) może przerwać przepływ poczty do lokalnego lub zewnętrznych miejsc docelowych. Jak wcześniej przekazanych Aby uprościć zarządzanie zakres adresów IP, możemy jest konsolidowany na podstawie zakresów adresów IP Exchange Online ochrony (podniesienie uprawnień), które są używane do wysyłania i odbierania wiadomości e-mail, poza usługi Office 365. Nasza analiza wskazuje, że jedną lub kilkoma e-mail zewnętrznych źródeł i miejsc docelowych, które zostały skonfigurowane w łączniki przepływu poczty nie są akceptowanie połączeń z IP adres zakresów pokazano [tutaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Działania przed 26 października do upewnij się, że te źródła i miejsca docelowe będzie akceptować połączenia z wszystkie [opublikowane adresy IP podniesienie poziomu uprawnień](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Aby uzyskać więcej informacji o tej zmianie zobacz Centrum wiadomości poczty, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Uwaga**: Jeśli poprzednio używane adres IP lub adres URL publikowania przez HTML, XML i RSS dla aktualizacji punktu końcowego, również należy dokonać migracji do nowych usług sieci web do automatyzacji typów aktualizacji. Aby uzyskać więcej informacji zobacz [kategorii punktu końcowego usługi Office 365 i adres IP pakietu Office 365 i adres URL usługi sieci web](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  

