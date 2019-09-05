---
title: Zapisywanie witryny lub listy jako szablonu
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752042"
---
# <a name="save-site-or-list-as-a-template"></a>Zapisywanie witryny lub listy jako szablonu

Szablony witryn programu SharePoint są wstępnie skompilowanymi definicjami zaprojektowanymi wokół konkretnej potrzeby biznesowej. Aby uzyskać więcej informacji, zobacz [za pomocą szablonów do tworzenia różnych rodzajów witryn programu SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablon w programie SharePoint Online.

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brak**. 

- Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu. Szczegółowe kroki, przykłady i zagadnienia zobacz [Zezwalaj lub zapobieganie skryptu niestandardowego](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach, które korzystają z infrastruktury publikowania programu SharePoint Server.


**Nie można utworzyć szablonu witryny lub nie działa poprawnie**

- Szablon może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie uaktywni się. Jeśli funkcja nie jest dostępna do aktywowania w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.


- Sprawdź, czy wszystkie listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować Tworzenie szablonu witryny.


- Witryna może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 megabajtów (MB).


- Istnieją problemy z wyświetlaniem danych z listy, która używa kolumny odnośnika. Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z listy wyszukiwania poprawne w programie SharePoint w trybie online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, należy odwoływać się, [tworzyć i używać szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

