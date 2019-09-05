---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747758"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Odmowa dostępu podczas wyświetlania przepływu pracy

SharePoint 2013 przepływy pracy, które próbują wysłać wiadomość e-mail do grupy programu SharePoint może zakończyć się niepowodzeniem z komunikatem o błędzie "odmowa dostępu", jeśli członkostwo w grupie programu SharePoint nie jest ustawiona na wszyscy.
  
 **Aby rozwiązać ten problem, wykonaj następujące kroki:**
  
 1. Zezwalaj wszystkim, aby zobaczyć członków grupy programu SharePoint.
  
 2. Usuń grupę programu SharePoint z wiersza do lub DW wiadomości e-mail.
  
 3. Jawnie dodać użytkowników do do lub DW wiersza, jeśli nie można zmienić widoczność członkostwa dla grupy programu SharePoint.
  
Aby wyświetlić więcej szczegółów, zapoznaj się [http nieautoryzowane do/_vti_bin/Client.svc/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  