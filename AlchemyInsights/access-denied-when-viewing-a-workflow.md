---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687340"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Odmowa dostępu podczas wyświetlania przepływu pracy

Przepływy pracy programu SharePoint 2013, które próbują wysłać wiadomość e-mail do grupy programu SharePoint, mogą zakończyć się niepowodzeniem, za pomocą komunikatu o błędzie "Odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawione na Wszyscy.
  
 **Aby rozwiązać ten problem, wykonaj następujące czynności:**
  
 1. Zezwalaj wszystkim na wyświetlanie członków grupy programu SharePoint.
  
 2. Usuń grupę programu SharePoint z wiersza Do lub DW wiadomości e-mail.
  
 3. Jawnie dodaj użytkowników do linii Do lub DW, jeśli nie można zmienić widoczności członkostwa dla grupy programu SharePoint.
  
Aby wyświetlić więcej szczegółów, zapoznaj się z [http nieautoryzowane do /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  