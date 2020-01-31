---
title: Nie można usunąć elementów w programie SharePoint lub OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571281"
---
# <a name="unable-to-delete-items"></a>Nie można usunąć elementów

Zasady przechowywania może to spowodować, należy wyłączyć lub wykluczyć odpowiednie wstrzymanie, które jest przyczyną tego problemu. Po usunięciu zasad przechowywania lub blokady zmiana może potrwać do 24 godzin. Upewnij się, że nie ma konfiguracji [zasad przechowywania](https://docs.microsoft.com/office365/securitycompliance/retention-policies) w elemencie.

Lokacja mogła przekroczyć limit magazynowania, zwiększyć [przydział lokacji](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i usunąć element.

Upewnij się, że element nie jest [wyewidencjonowany](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) do innego użytkownika.

Na koniec administratorzy mogą używać [wzorców i praktyk programu SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), który zawiera bibliotekę poleceń programu PowerShell, które umożliwiają wykonywanie złożonych akcji zarządzania, takich jak wymuszanie usuwania upartych elementów.
- [Usuwanie pliku PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Usuwanie folderu PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Usuń element listy PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Usuń listę PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Usuwanie pola PNP (kolumna)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)