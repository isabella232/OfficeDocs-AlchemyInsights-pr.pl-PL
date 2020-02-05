---
title: Tworzenie witryny w usłudze SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770433"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tworzenie witryn programu SharePoint przy użyciu szablonów

Możliwość zapisywania witryny jako szablonu nie jest obsługiwana w nowoczesnych witrynach komunikacyjnych lub zespołowych. Aby uzyskać więcej informacji na temat używania szablonów, zobacz [Zapisywanie, pobieranie i przekazywanie witryny programu SharePoint jako szablonu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Oto kilka typowych problemów/rozwiązań dotyczących zapisywania witryny lub listy jako szablonu w usłudze Sharepoint Online. 

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub brakuje przycisku**

Administratorzy będą musieli zezwolić na skrypt niestandardowy, aby włączyć funkcje szablonu. Szczegółowe kroki, przykłady i zagadnienia można znaleźć 

- [Zezwalanie na skrypt niestandardowy lub zapobieganie mu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może powodować problemy w witrynach korzystających z infrastruktury publikowania programu SharePoint Server.

**Nie można utworzyć szablonu witryny lub nie działa poprawnie**

W szablonie może brakować [funkcji](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i nie zostanie uruchomiony. Jeśli funkcja nie jest dostępna do aktywacji w bieżącym zbiorze witryn, nie można użyć szablonu witryny do utworzenia witryny.

- Sprawdź, czy jakiekolwiek listy lub biblioteki przekraczają [próg limitu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 elementów, ponieważ może to blokować tworzenie szablonu witryny.

- Lokacja może używać zbyt wielu zasobów i dlatego szablon witryny przekracza limit 50 MB.


- Występują problemy z wyświetlaniem danych z listy, która używa kolumny odlotowej. Aby uzyskać więcej informacji, zobacz [Lista wygenerowana przez szablon nie wyświetla danych z poprawnej listy odstawień w usłudze SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, zapoznaj się z [temattworzenia i używania szablonów witryn](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



