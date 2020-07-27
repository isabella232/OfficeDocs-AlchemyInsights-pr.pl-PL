---
title: Wielu użytkowników otrzymuje błąd odmowy dostępu podczas dodawania dodatków w programie Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424170"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Wielu użytkowników otrzymuje błąd odmowy dostępu podczas dodawania dodatków w programie Outlook

Można określić, którzy administratorzy w organizacji mają uprawnienia do instalowania dodatków programu Outlook i zarządzania nimi. Można również określić, którzy użytkownicy w organizacji mają uprawnienia do instalowania dodatków i zarządzania nimi na własny użytek.

Aby uzyskać szczegółowe informacje, zobacz [Określanie administratorów i użytkowników, którzy mogą instalować dodatki dla programu Outlook i zarządzać nimi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)

Aby sprawdzić, czy pomyślnie przypisano uprawnienia użytkownikowi, <Role Name> zastąp nazwą roli do zweryfikowania i uruchom następujące polecenie w programie Exchange Online PowerShell:

Get-ManagementRoleAssignment -Rola " <Role Name> " -GetEffectiveUsers

W tym przykładzie pokazano, jak sprawdzić, komu przypisano uprawnienia do instalowania dodatków ze Sklepu Office dla organizacji.

Powershell

-Rola "Org Marketplace Apps" -GetEffectiveUsers

W wynikach, Get-ManagementRoleAssignment, przejrzyj wpisy w kolumnie Skuteczni użytkownicy.

Aby uzyskać szczegółowe informacje o składni i parametrach, zobacz [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 