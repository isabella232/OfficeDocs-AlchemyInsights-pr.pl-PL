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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642154"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemy podczas tworzenia witryny połączonej z grupą w programie SharePoint

1. Niektóre typowe problemy napotkane podczas tworzenia lub ponownego tworzenia witryny połączonej z grupą.
Jeśli grupa i jej połączona witryna zostały usunięte i chcesz utworzyć inną witrynę o tym samym adresie URL, musisz trwale usunąć poprzednią witrynę.

   - Pobierz [powłokę zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Aby uzyskać więcej informacji na temat rozpoczynania pracy z programem Powershell, zobacz [Wprowadzenie do powłoki zarządzania usługi SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Usuń witrynę z usuniętych witryn za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Program Powershell jest wymagany do trwałego usuwania witryn grupowych.

1. Jeśli tworzysz witrynę połączoną z grupą i otrzymujesz ostrzeżenie: **Inna grupa o tym samym aliasie już istnieje,** sprawdź istniejące grupy z Centrum [administracyjnego usługi Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebna, lub utwórz witrynę z przypisanym innym aliasem.

1. Istnieją różne sposoby tworzenia i używania nowoczesnych grup w programie SharePoint.

   - Istniejące witryny można połączyć z grupą usługi Office 365. Aby uzyskać więcej informacji, zobacz [Łączenie grupy usługi Office 365 przy użyciu interfejsu użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Aby utworzyć witrynę połączoną z grupą usługi Office 365, musisz utworzyć [witrynę zespołu](https://admin.microsoft.com/sharepoint).
