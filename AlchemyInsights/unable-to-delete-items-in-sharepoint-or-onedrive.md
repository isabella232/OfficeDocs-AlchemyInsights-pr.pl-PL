---
title: Nie można usunąć elementów w SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038527"
---
# <a name="unable-to-delete-items"></a>Nie można usunąć elementów

- Zasady przechowywania mogą to powodować, należy wyłączyć lub wykluczyć odpowiednie hold, które powoduje ten problem. Po usunięciu zasad przechowywania lub ich przechowywania może upłynieć do 24 godzin, aż zmiana zostanie w życie. Upewnij się, że dla [tego](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) elementu nie ma konfiguracji zasad przechowywania.

- Witryna mogła przekroczyć limit magazynowania, zwiększyć [przydział witryny i](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) usunąć element.

- Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) dla innego użytkownika.

- Na koniec administratorzy mogą używać wzorców i praktyk programu [SharePoint,](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) która zawiera bibliotekę poleceń programu PowerShell, która umożliwia wykonywanie złożonych akcji zarządzania, takich jak wymuszanie usuwania elementów uporczywych.
- [Usuń plik PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Usuń folder PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Usuwanie elementu listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Usuwanie listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Usuwanie pola PNP (kolumny)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)