---
title: Nie można usunąć elementów w programie SharePoint lub OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748584"
---
# <a name="unable-to-delete-items"></a>Nie można usunąć elementów

Masz problemy z usunięciem elementów programu SharePoint?

- Zawsze upewnij się, że masz [odpowiednie uprawnienia](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) do usunięcia elementu lub próba usunięcia elementu przez [administratora zbioru witryn](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .

- Upewnij się, że w elemencie nie ma ustawienia [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .

- Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) dla innego użytkownika.

- Na koniec Administratorzy mogą używać [wzorców i praktyk programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), który zawiera bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych działań zarządzania, takich jak wymuszenie usunięcia uparty elementów.
- [Usuń plik PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Usuń folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Usuń element listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Usuń listę PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Usuń pole PNP (kolumna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)