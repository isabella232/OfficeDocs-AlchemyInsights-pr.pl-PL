---
title: Tworzenie witryny w aplikacji SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057976"
---
# <a name="create-sharepoint-sites-using-templates"></a>Tworzenie SharePoint przy użyciu szablonów

Możliwość zapisywania witryny jako szablonu nie jest obsługiwana w nowoczesnej witrynach komunikacji ani zespołu. Aby uzyskać więcej informacji o używaniu szablonów, zobacz [Zapisywanie, pobieranie i przekazywanie witryny programu SharePoint jako szablonu](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Oto kilka typowych problemów lub rozwiązań dotyczących zapisywania witryny lub listy jako szablonu w usłudze SharePoint Online. 

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub go brakuje**

Administratorzy muszą zezwolić na skrypt niestandardowy w celu włączenia funkcji szablonów. Aby uzyskać szczegółowe instrukcje, przykłady i zagadnienia, zobacz 

- [Zezwalanie na skrypt niestandardowy lub zakazywanie go](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może być przyczyną problemów w witrynach, w których jest używana infrastruktura publikowania programu SharePoint Server.

**Nie można utworzyć szablonu witryny lub nie działa on poprawnie**

W szablonie może brakować [funkcji i](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) nie można go aktywować. Jeśli funkcja nie jest dostępna do uaktywnienia w bieżącym zbiorze witryn, nie możesz utworzyć witryny przy użyciu szablonu witryny.

- Upewnij się, że żadna z list lub bibliotek nie przekracza [progu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) wynoszącego 5000 elementów, ponieważ może to uniemożliwiać utworzenie szablonu witryny.

- Witryna może używać zbyt wielu zasobów i w związku z tym rozmiar szablonu witryny przekracza limit 50 MB.


- Występują problemy z wyświetlaniem danych z listy, w której jest używana kolumna odnośnika. Aby uzyskać więcej informacji, zobacz [W usłudze SharePoint Online na liście wygenerowanej na podstawie szablonu nie są wyświetlane dane z odpowiedniej listy odnośników](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i ich rozwiązań, zobacz [Tworzenie i używanie szablonów witryn.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



