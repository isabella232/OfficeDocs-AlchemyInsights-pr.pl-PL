---
title: Przywracanie usuniętego folderu publicznego
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063712"
---
# <a name="restore-a-deleted-public-folder"></a>Przywracanie usuniętego folderu publicznego

**Aby przywrócić usunięte elementy z folderu publicznego:**

- Zobacz [Nie można odzyskać usuniętych elementów z folderu publicznego niebędącego pocztą w programie Outlook 2016](https://aka.ms/pfrec).
 
**Aby przywrócić usunięty folder publiczny (dowolnego typu):** 

- Użyj następującego polecenia EXO PowerShell:

    Składni:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nazwa -eq\<" name_of_deleted_public_Folder"}; Set-PublicFolder $pf.identity \<-Ścieżka ścieżki, w której folder zostanie przywrócony>

    Przykład: Następujące polecenie przywróci podfolder1 i umieści go w obszarze \Parent1:

    >$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ? {$_. Nazwa -eq "Podfolder1"}; Ustaw-PublicFolder $pf.identity -Path \Parent1

Aby uzyskać więcej informacji, zobacz [Przywracanie usuniętego folderu publicznego.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
