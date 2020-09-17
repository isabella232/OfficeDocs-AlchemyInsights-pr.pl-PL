---
title: 1065 zaniechanie EOP wychodzącego adresu IP rangesMC146155
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
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806805"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Zaniechanie zakresów wychodzących adresów IP EOP

Wykryliśmy potencjalne problemy w Twojej organizacji, które (jeśli nie zostały naprawione przed 26 października 2018 r.), mogą spowodować przerwanie przepływu poczty w lokalnych lub zewnętrznych obszarach docelowych. Jak już się przekazało, aby uprościć zarządzanie zakresem adresów IP, konsolidujemy zakresy adresów IP usługi Exchange Online Protection (EOP) używane do wysyłania i odbierania wiadomości e-mail poza systemem Microsoft 365. Nasze analizy wskazują, że jeden lub więcej zewnętrznych źródeł wiadomości e-mail lub lokalizacji docelowych skonfigurowanych w łącznikach przepływu poczty nie akceptuje połączeń z pokazanych [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)zakresów adresów IP.

Przed 26 października możesz zapewnić, że te źródła i miejsca docelowe będą akceptować połączenia z wszystkimi [opublikowanymi adresami IP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)i ze wszystkich opublikowanych EOP.

Aby uzyskać więcej informacji na temat tej zmiany, zobacz wpisy w centrum wiadomości [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)lub [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Uwaga**: Jeśli poprzednio korzystano z publikowania adresów IP lub adresów URL za pomocą funkcji HTML, XML i RSS dla aktualizacji punktów końcowych, należy również przeprowadzić migrację do nowych usług sieci Web, aby zautomatyzować te typy aktualizacji. Aby uzyskać więcej informacji, zobacz [Kategorie punktów końcowych microsoft 365 oraz usługa sieci Web microsoft 365 adres IP i adres URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
