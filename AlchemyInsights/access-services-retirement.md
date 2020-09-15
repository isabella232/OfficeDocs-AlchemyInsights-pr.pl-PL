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
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698692"
---
# <a name="access-services-retirement"></a>Wycofanie usług programu Access

Ponieważ został pierwotnie ogłoszony w MC97576, w marcu 2017 r. i kontynuując komunikację w ciągu ubiegłych rocznych usług programu Access. Kolejnym etapem tego procesu będzie usunięcie baz danych sieci Web programu Access, które używają list programu SharePoint jako podstawowego magazynu danych.

**Jak to wpłynie?**

Począwszy od czerwca 2019, my zakończymy tworzenie nowych baz danych programu Access w usłudze SharePoint Online oraz zamkniją usługę i wszystkie pozostałe aplikacje do 2020 kwietnia.

**Co muszę zrobić, aby przygotować się na tę zmianę?**

Zachęcamy do utworzenia planu migracji dla baz danych sieci Web programu Access w organizacji. Administratorzy mogą korzystać ze [skanera aplikacji programu SharePoint](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) w celu uzyskania spisu aplikacji programu Access, których używają witryny.

Istnieje kilka sposobów migrowania danych baz danych sieci Web programu Access:

- Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub pliku programu Excel.
- Zalecamy również Eksplorowanie usługi Microsoft PowerApps jako alternatywnej platformy, która umożliwia tworzenie bez kodu rozwiązania biznesowego dla sieci Web i urządzeń przenośnych.