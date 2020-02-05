---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770361"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemy podczas tworzenia połączonej witryny grupy w programie SharePoint

1. Niektóre typowe problemy napotkane podczas tworzenia lub ponownego tworzenia połączonej witryny grupy.
Jeśli usunięto grupę i połączoną z nią witrynę i chcesz utworzyć inną witrynę z tym samym adresem URL, musisz trwale usunąć poprzednią witrynę.

   - Pobierz [powłokę zarządzania spojm](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Aby uzyskać więcej informacji na temat rozpoczynania pracy z usługą PowerShell, zobacz [Wprowadzenie do programu SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Usuń witrynę z usuniętych witryn za pomocą polecenia cmdlet [Programu Powershell remove-SPODeletedSite.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell jest wymagany do trwałego usuwania witryn grupowych.

1. Jeśli tworzysz połączoną witrynę grupy i otrzymujesz ostrzeżenie: **Inna grupa o tym samym aliasie już istnieje,** sprawdź istniejące grupy z [Usługi Office 365 w Centrum administracyjnym](https://admin.microsoft.com/AdminPortal/Home#/groups). Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebna, lub utwórz witrynę z przypisanym innym aliasem.

1. Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programu SharePoint.

   - Istniejące witryny można połączyć z grupą usługi Office 365. Aby uzyskać więcej informacji, zobacz [Łączenie grupy usługi Office 365 przy użyciu interfejsu użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Aby utworzyć połączoną witrynę grupy usługi Office 365, musisz utworzyć [witrynę zespołu](https://admin.microsoft.com/sharepoint).
