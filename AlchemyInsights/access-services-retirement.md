---
title: Dostęp do usług emerytalnych
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
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050499"
---
# <a name="access-services-retirement"></a>Dostęp do usług emerytalnych

Jak pierwotnie ogłosiliśmy w MC97576, w marcu 2017, i nadal komunikować się w ciągu ostatnich lat Access Services są wycofane z pakietu Office 365. Następnym etapem w tym procesie będzie usunięcie baz danych programu Access w sieci Web, które używają list SharePoint jako ich podstawowej pamięci masowej.

**Jak to wpływa na mnie?**

Począwszy od czerwca 2019, firma będzie zatrzymać tworzenie nowych baz danych programu Access w programie SharePoint Online i zamknąć usługę i wszystkie pozostałe aplikacje do kwietnia 2020.

**Co muszę zrobić, aby przygotować się do tej zmiany?**

Zachęcamy do utworzenia planu przejściowego dla baz danych programu Access w organizacji. Administratorzy mogą używać [skanera aplikacji programu SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) do uzyskiwania spisu aplikacji programu Access korzystających z witryn.

Istnieje kilka sposobów migracji danych programu Access w sieci Web:

- Importowanie do lokalnej bazy danych programu Access (. ACCDB) lub do pliku programu Excel.
- Zalecamy również Eksplorowanie usługi Microsoft PowerApps jako alternatywnej platformy do tworzenia niekodowych rozwiązań biznesowych dla sieci Web i urządzeń przenośnych.