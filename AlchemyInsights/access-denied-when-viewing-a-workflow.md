---
title: Odmowa dostępu podczas przeglądania przepływu pracy
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883601"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Odmowa dostępu podczas przeglądania przepływu pracy

2013 przepływów pracy programu SharePoint, która próbuje wysłać wiadomość e-mail do grupy programu SharePoint może się niepowodzeniem z komunikatem o błędzie "Odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawiona dla wszystkich.
  
 **Aby rozwiązać ten problem, wykonaj następujące kroki:**
  
 1. Zezwalaj wszystkim zobaczyć członków grupy programu SharePoint.
  
 2. Usuń grupę programu SharePoint z do lub DW wiersz wiadomości e-mail.
  
 3. Jawnie dodać użytkowników do do lub DW linii, jeśli nie można zmienić widoczności członkostwa grupy programu SharePoint.
  
Aby wyświetlić więcej szczegółów można znaleźć [HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)nieuprawnione do /_vti_bin/client.svc/sp.utilities.utility.SendEmail.
  