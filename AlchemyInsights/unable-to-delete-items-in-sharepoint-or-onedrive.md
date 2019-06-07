---
title: Nie można usunąć elementów w programie SharePoint lub OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757934"
---
# <a name="unable-to-delete-items"></a>Nie można usunąć elementów

Masz problemy z usunięciem elementów?

- Zawsze upewnij się, że masz [odpowiednie uprawnienia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) , aby usunąć element lub mają próba [administrator zbioru witryn](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) , Usuń element.

- Upewnij się, że nie ma ustawienia [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) dla towaru.

- Upewnij się, że element nie jest [wyewidencjonowany przez](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) innego użytkownika.

- Wreszcie Administratorzy mogą używać [programu SharePoint wzorce i praktyki](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) który zawiera biblioteki programu PowerShell polecenia, które pozwalają na przeprowadzenie kompleksowego zarządzania akcje takie jak wymusić usunięcie elementów uporczywe. 
- [Usuń plik PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Usuwanie folderu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Usuwanie elementu listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Usuwanie listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Usuwanie PNP pola (kolumny)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)