---
title: Wycofanie usług programu Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938705"
---
# <a name="access-services-retirement"></a>Wycofanie usług programu Access

Jak pierwotnie informowaliśmy w programie MC97576, w marcu 2017 r. i nadal komunikowaliśmy się w ciągu ostatniego roku, Usługi programu Access są wy wycofane. Następnym etapem tego procesu będzie usunięcie baz danych sieci Web programu Access, które używają list SharePoint jako podstawowego magazynu danych.

**Jak to na mnie wpłynie?**

Począwszy od czerwca 2019 r., zaprzestanie tworzenia nowych baz danych programu Access w usłudze SharePoint Online i wyłączenie usługi i pozostałych aplikacji do kwietnia 2020 r.

**Co muszę zrobić, aby przygotować się na tę zmianę?**

Zachęcamy do utworzenia planu przejścia dla baz danych sieci Web programu Access organizacji. Administratorzy mogą za pomocą [skanera SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) uzyskać spis aplikacji programu Access, z których korzystają witryny.

Istnieje kilka sposobów migrowania danych baz danych sieci Web programu Access:

- Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub do Excel pliku.
- Zalecamy również zapoznanie się Microsoft PowerApps alternatywnej platformy w celu tworzenia rozwiązań biznesowych bez kodu dla sieci Web i urządzeń przenośnych.