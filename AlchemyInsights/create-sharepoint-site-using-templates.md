---
title: Utworzyć witrynę w dokumentacji Online programu SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515008"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tworzenie witryn programu SharePoint przy użyciu szablonów

Szablony witryn programu SharePoint są wbudowane definicje została zaprojektowana dla określonych potrzeb biznesowych. Aby uzyskać więcej informacji zobacz [Używanie szablonów do tworzenia różnego rodzaju witryny programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Poniżej przedstawiono typowe problemy/rozwiązania dotyczące zapisywania witryny lub listy jako szablonu w dokumentacji Online programu Sharepoint. 

**Zapisz przycisk Szablon witryny/lista jest niedostępna lub Brak**

Administratorzy należy umożliwić niestandardowego skryptu do włączenia funkcji szablonu. Aby uzyskać szczegółowe instrukcje Zobacz przykłady i uwagi 

- [Zezwalanie lub blokowanie skryptu niestandardowego](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Zapisz witrynę jako szablon, polecenie nie jest obsługiwane i może być przyczyną problemów w witrynach, które używają publikowania infrastruktury serwera programu SharePoint.

**Nie można utworzyć szablon witryny lub nie działa prawidłowo**

Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie aktywuje. Jeśli funkcja nie jest dostępna uaktywnić w bieżącym zbiorze witryn, nie można użyć szablonu witryny do tworzenia witryny.

- Sprawdź, jeśli list ani bibliotek przekraczają [Próg Limit widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 pozycji jak to zablokowanie tworzenia szablonu witryny.

- Witryny mogą używać zbyt wiele zasobów i w związku z tym szablon witryny przekracza limit 50 MB.


- Istnieją problemy z wyświetlaniem danych z listy, która jest używana kolumna odnośnika. Aby uzyskać więcej informacji zobacz temat [generowany szablon listy nie są wyświetlane dane z listy wyszukiwania poprawne w dokumentacji Online programu SharePoint](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Aby uzyskać bardziej szczegółowe informacje o typowe problemy i rozwiązania Sprawdź, czy [tworzenia i stosowania szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



