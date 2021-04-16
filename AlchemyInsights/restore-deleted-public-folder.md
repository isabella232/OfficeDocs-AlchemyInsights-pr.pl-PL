---
title: Przywracanie usuniętego folderu publicznego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809449"
---
# <a name="restore-a-deleted-public-folder"></a>Przywracanie usuniętego folderu publicznego

**Aby przywrócić usunięte elementy z folderu publicznego:**

- Zobacz Nie można odzyskać elementów usuniętych z folderu publicznego, który nie jest [pocztą, w programie Outlook 2016.](https://aka.ms/pfrec)
 
**Aby przywrócić usunięty folder publiczny (dowolnego typu):** 

- Użyj następującego polecenia programu EXO PowerShell:

    Składnia:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Przykład: Następujące polecenie spowoduje przywrócenie podfolderu1 i umieść go w obszarze \Element_nadrzędny1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Aby [uzyskać więcej szczegółowych informacji,](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) zobacz Przywracanie usuniętego folderu publicznego.
