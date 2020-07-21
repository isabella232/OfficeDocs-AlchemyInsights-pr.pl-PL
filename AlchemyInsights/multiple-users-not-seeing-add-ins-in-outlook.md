---
title: Wielu użytkowników nie widzi dodatków w programie Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198237"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Wielu użytkowników nie widzi dodatków w programie Outlook

Jeśli testujesz dodatki programu Outlook i żaden nie jest pokazywany, jako pierwszy krok rozwiązywania problemów, użyj polecenia cmdlet **Get-OrganizationConfig** PowerShell, aby wykonać kwerendę parametru _AppsForOfficeEnabled._ Jeśli kwerenda zwraca wartość **False,** ustaw ten parametr na **True** przy użyciu polecenia cmdlet **Set-OrganizationConfig,** więc dodatki są wyświetlane zgodnie z oczekiwaniami.

Nie zaleca się, aby parametr _AppsForOfficeEnabled_ był ustawiony na **False**. Wartość **False** zastępuje wszystkie powyższe ustawienia roli administracyjne i użytkownika i zapobiega aktywowaniu nowych aplikacji przez dowolnego użytkownika w organizacji.

Aby uzyskać więcej informacji, zobacz [Określanie administratorów i użytkowników, którzy mogą instalować dodatki programu Outlook i zarządzać nimi.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)