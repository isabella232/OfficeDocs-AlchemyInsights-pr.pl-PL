---
title: Odmowa dostępu podczas wyświetlania przepływu pracy
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955211"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Odmowa dostępu podczas wyświetlania przepływu pracy

Przepływy pracy programu SharePoint 2013 próbujące wysłać wiadomość e-mail do grupy programu SharePoint mogą się nie powieść z komunikatem o błędzie "Odmowa dostępu", jeśli członkostwo w grupie usługi SharePoint nie jest ustawione na Wszyscy.
  
 **Aby rozwiązać ten problem, wykonaj następujące czynności:**
  
 1. Pozwól wszystkim na wyświetlanie członków grupy SharePoint grupy.
  
 2. Usuń SharePoint z wiersza Do lub DW wiadomości e-mail.
  
 3. Jeśli nie można zmienić widoczności członkostwa w grupie, jawnie dodaj użytkowników do wiersza Do SharePoint DW.
  
Aby wyświetlić więcej szczegółów, zobacz [HTTP Nieautoryzowany do /_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  