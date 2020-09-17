---
title: Nie można usunąć elementów w programie SharePoint ani w usłudze OneDrive
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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806121"
---
# <a name="unable-to-delete-items"></a>Nie można usunąć elementów

Zasady przechowywania mogą być przyczyną tego problemu, należy wyłączyć lub wykluczyć odpowiednie zawieszenie, które powoduje ten problem. Gdy zasady przechowywania lub wstrzymanie zostaną usunięte, może upłynąć do 24 godzin, aby zmiana została uwzględniona. Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) dla elementu.

Witryna mogła Przekroczono limit miejsca, zwiększyć [przydział witryny](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.

Upewnij się, że element nie został [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) przez innego użytkownika.

Na koniec Administratorzy mogą używać [wzorów i procedur programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), które zawierają bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak Wymuś usuwanie stubborn elementów.
- [Usuwanie pliku PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Usuwanie folderu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Usuwanie elementu listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Usuwanie listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Usuwanie pola PNP (kolumny)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)