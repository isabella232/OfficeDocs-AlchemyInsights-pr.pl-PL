---
title: Dodawanie grupy do witryny SharePoint sieci Web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093720"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Typowe problemy podczas tworzenia witryny połączonej z grupą w programie SharePoint

1. Jeśli usunięto grupę i połączną z nim witrynę i chcesz utworzyć nową witrynę o tym samym adresie URL, musisz trwale usunąć poprzednią witrynę.

   - Pobierz [powłokę zarządzania usługą SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Aby uzyskać więcej informacji na temat rozpoczynania pracy z programem PowerShell, zobacz Wprowadzenie do [powłoki SharePoint zarządzania online.](/powershell/module/sharepoint-online/remove-sposite)
   - Usuń witrynę z usuniętych witryn przy użyciu polecenia cmdlet [remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) programu Powershell. Program PowerShell jest wymagany do trwałego usunięcia witryn grup.

1. Jeśli tworzysz witrynę połączenią z grupą i otrzymujesz ostrzeżenie: Inna grupa o tym samym **aliasie** już istnieje, sprawdź istniejące grupy na stronie [centrum administracyjne platformy Microsoft 365.](https://admin.microsoft.com/AdminPortal/Home#/groups) Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebna, lub utwórz witrynę z przypisanym innym aliasem.

1. Istnieją różne sposoby tworzenia i używania nowoczesnych grup za pomocą SharePoint.

   - Istniejące witryny można połączyć z Microsoft 365 grupy. Aby uzyskać więcej informacji, [Połączenie Microsoft 365 za pomocą SharePoint interfejsu użytkownika.](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Aby utworzyć witrynę Microsoft 365 połączonej z grupą, musisz utworzyć [witrynę zespołu.](https://admin.microsoft.com/sharepoint)
