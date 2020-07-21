---
title: Pojedynczy użytkownik nie widzi dodatków w programie Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198215"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Pojedynczy użytkownik nie widzi dodatków w programie Outlook

Użytkownik może być częścią roli, która nie ma poprawnego parametru AppsForOfficeEnabled. Uruchom to polecenie cmdlet, aby dowiedzieć się, czy z użytkownikiem jest skojarzona poprawna rola:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegowanie $false | Format-Tabela -Auto Rola,RoleAssigneeName,RoleAssigneeType

Aby uzyskać więcej informacji, zobacz [Określanie administratorów i użytkowników, którzy mogą instalować dodatki do programu Outlook i zarządzać nimi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)
