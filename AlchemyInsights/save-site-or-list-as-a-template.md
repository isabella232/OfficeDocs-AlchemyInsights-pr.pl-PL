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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109214"
---
# <a name="save-site-or-list-as-a-template"></a>Zapisywanie witryny lub listy jako szablonu

SharePoint witryny to wstępnie skonstruowane definicje zaprojektowane w celu określonej potrzeby biznesowej. Aby uzyskać więcej informacji, zobacz Tworzenie różnych rodzajów witryn w SharePoint za [pomocą SharePoint szablonów.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Oto niektóre typowe problemy lub rozwiązania dotyczące zapisywania witryny lub listy jako szablonu w u SharePoint Online.

**Przycisk Zapisz szablon witryny/listy nie jest dostępny lub go brakuje**. 

- Administratorzy muszą zezwolić na skrypt niestandardowy w celu włączenia funkcji szablonów. Aby uzyskać szczegółowe instrukcje, przykłady i zagadnienia, zobacz Zezwalanie na skrypt niestandardowy lub [zapobieganie nim.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Polecenie Zapisz witrynę jako szablon nie jest obsługiwane i może być przyczyną problemów w witrynach, w których jest używana infrastruktura publikowania programu SharePoint Server.


**Nie można utworzyć szablonu witryny lub nie działa on poprawnie**

- W szablonie może brakować [funkcji i](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) nie można go aktywować. Jeśli funkcja nie jest dostępna do uaktywnienia w bieżącym zbiorze witryn, nie możesz utworzyć witryny przy użyciu szablonu witryny.


- Upewnij się, że żadna z list lub bibliotek nie przekracza [progu widoku listy](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) wynoszącego 5000 elementów, ponieważ może to uniemożliwiać utworzenie szablonu witryny.


- Witryna może korzystać z zbyt wielu zasobów, a w związku z tym rozmiar szablonu witryny przekracza limit 50 megabajtów (MB).


- Występują problemy z wyświetlaniem danych z listy, w której jest używana kolumna odnośnika. Aby uzyskać więcej informacji, zobacz Na liście wygenerowanej na podstawie szablonu nie są wyświetlane dane z odpowiedniej listy odnośników w aplikacji [SharePoint online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Aby uzyskać bardziej szczegółowe informacje na temat typowych problemów i rozwiązań, zobacz [Tworzenie i używanie szablonów witryn.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

