---
title: Tworzenie witryny w programie SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755318"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tworzenie witryn programu SharePoint przy użyciu szablonów

Szablony witryn programu SharePoint są wstępnie skompilowanymi definicjami zaprojektowanymi wokół konkretnej potrzeby biznesowej. Aby uzyskać więcej informacji, zobacz [za pomocą szablonów do tworzenia różnych rodzajów witryn programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablon w programie SharePoint Online. 

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brak**

Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu. Szczegółowe kroki, przykłady i zagadnienia Zobacz 

- [Zezwalanie lub zapobieganie skryptowaniu niestandardowym](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach, które korzystają z infrastruktury publikowania programu SharePoint Server.

**Nie można utworzyć szablonu witryny lub nie działa poprawnie**

Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie uaktywni się. Jeśli funkcja nie jest dostępna do aktywowania w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.

- Sprawdź, czy wszystkie listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować Tworzenie szablonu witryny.

- Witryna może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 MB.


- Istnieją problemy z wyświetlaniem danych z listy, która używa kolumny odnośnika. Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z listy wyszukiwania poprawne w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, należy sprawdzić [Tworzenie i używanie szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



