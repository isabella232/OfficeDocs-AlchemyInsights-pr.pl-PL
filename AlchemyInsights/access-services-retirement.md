---
title: Przejście na emeryturę usług dostępu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687268"
---
# <a name="access-services-retirement"></a>Przejście na emeryturę usług dostępu

Jak pierwotnie ogłosiliśmy w MC97576, w marcu 2017 r., i nadal komunikować się w ciągu ostatniego roku Usługi dostępu są na emeryturze. Następną fazą tego procesu będzie usunięcie baz danych sieci Web programu Access, które używają list programu SharePoint jako bazowego magazynu danych.

**Jak to wpływa na mnie?**

Od czerwca 2019 r. przestaniemy tworzenie nowych baz danych programu Access w usłudze SharePoint Online i do kwietnia 2020 r. wyłączymy usługę i wszystkie pozostałe aplikacje.

**Co muszę zrobić, aby przygotować się do tej zmiany?**

Zachęcamy do utworzenia planu przejścia dla baz danych sieci Web programu Access w organizacji. Administratorzy mogą korzystać ze [skanera aplikacji programu SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) w celu uzyskania spisu aplikacji programu Access używanych przez witryny.

Istnieje kilka sposobów migracji danych baz danych sieci Web programu Access:

- Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub do pliku programu Excel.
- Zalecamy również zbadanie usługi Microsoft PowerApps jako alternatywnej platformy do tworzenia rozwiązań biznesowych bez kodu dla urządzeń sieci Web i urządzeń przenośnych.