---
title: Przywracanie usuniętego folderu publicznego
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774541"
---
# <a name="restore-a-deleted-public-folder"></a>Przywracanie usuniętego folderu publicznego

**Aby przywrócić elementy usunięte z folderu publicznego**:

- Zobacz [nie można odzyskać elementów usuniętych z folderu publicznego niebędącego pocztą e-mail w programie Outlook 2016](https://aka.ms/pfrec).
 
**Aby przywrócić usunięty folder publiczny (dowolnego typu)**: 

- Użyj następującego polecenia programu PowerShell w EXO:

    Polecenia

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Przykład: poniższe polecenie spowoduje przywrócenie Subfolder1 i umieszczenie go w obszarze \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Aby uzyskać więcej informacji, zobacz [Przywracanie usuniętego folderu publicznego](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
