---
title: Zapisywanie witryny lub listy jako szablonu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727541"
---
# <a name="save-site-or-list-as-a-template"></a>Zapisywanie witryny lub listy jako szablonu

Szablony witryn programu SharePoint są wstępnie zbudowanymi definicjami zaprojektowanymi wokół konkretnych potrzeb biznesowych. Aby uzyskać więcej informacji, zobacz [Tworzenie różnych rodzajów witryn programu SharePoint za pomocą szablonów](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Poniżej przedstawiono kilka typowych problemów i rozwiązań dotyczących zapisywania witryny lub listy jako szablonu w usłudze SharePoint Online.

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brakuje**go. 

- Aby umożliwić administratorom niestandardowym Włączanie funkcji szablonu, Administratorzy muszą zezwolić na używanie skryptu niestandardowego. Aby uzyskać szczegółowe instrukcje, przykłady i zagadnienia, zobacz [Zezwalanie lub zapobieganie skryptowi niestandardowemu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy z witrynami korzystającymi z infrastruktury publikowania w programie SharePoint Server.


**Nie można utworzyć szablonu witryny lub nie działa on poprawnie**

- W szablonie może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie można jej aktywować. Jeśli ta funkcja nie jest dostępna do aktywacji w bieżącym zbiorze witryn, nie można utworzyć witryny przy użyciu szablonu witryny.


- Sprawdź, czy jakieś listy lub biblioteki nie przekraczają [progu limitów widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) dla 5000 elementów, ponieważ może blokować Tworzenie szablonu witryny.


- Witryna może używać zbyt wielu zasobów, więc szablon witryny przekracza limit 50 megabajtów (MB).


- Występują problemy z wyświetlaniem danych z listy używającej kolumny odnośnika. Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablony nie wyświetla danych z odpowiedniej listy odnośników w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Aby uzyskać bardziej szczegółowe informacje o typowych problemach i rozwiązaniach, zobacz [Tworzenie i używanie szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

