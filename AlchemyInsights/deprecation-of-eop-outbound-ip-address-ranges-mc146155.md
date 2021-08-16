---
title: '1065: Deprecation of EOP outbound IP address rangesMC146155'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031272"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Wykryliśmy potencjalny problem z Twoją organizacją, który (jeśli nie zostanie poprawiony do 26 października 2018 r.), może spowodować przerwę w przepływie poczty do Twoich miejsc lokalnych lub zewnętrznych. Jak wcześniej wspomniano, aby uprościć zarządzanie zakresem adresów IP, konsolidujemy zakresy adresów IP usługi Exchange Online Protection (EOP), które są używane do wysyłania i odbierania wiadomości e-mail poza Microsoft 365. Nasza analiza wskazuje, że co najmniej jedno z zewnętrznych źródeł poczty e-mail lub miejsc docelowych skonfigurowanych w łącznikach przepływu poczty e-mail nie akceptuje połączeń z podanych tutaj zakresów [adresów](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)IP.

Działanie przed 26 października, aby zapewnić, że te źródła i miejsca docelowe będą akceptować połączenia ze wszystkimi opublikowanymi adresami [IP usługi EOP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Aby uzyskać więcej informacji na temat tej zmiany, zobacz Wpisy w Centrum wiadomości [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Uwaga:** Jeśli wcześniej używano publikowania adresów IP lub adresów URL za pośrednictwem kodu HTML, XML i RSS do aktualizacji punktów końcowych, należy również przeprowadzić migrację do nowych usług sieci Web w celu zautomatyzowania tych typów aktualizacji. Aby uzyskać więcej informacji, zobacz Microsoft 365 punktów końcowych i Microsoft 365 sieci Web adres [IP i adres URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
