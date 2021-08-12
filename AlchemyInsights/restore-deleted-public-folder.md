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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943385"
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
