---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750530"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemy podczas tworzenia lub grupowania połączonych witryn w programie SharePoint Online

Istnieje kilka typowych problemów napotkanych podczas tworzenia lub ponownego tworzenia grupy połączonej witryny.

 W przypadku usunięcia grupy i jej połączonej witryny i chęci utworzenia innej witryny z tym samym adresem URL, należy trwale usunąć poprzednią witrynę.

Pobierz za darmo [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Aby uzyskać więcej informacji na wprowadzenie do programu PowerShell, zobacz [wprowadzenie do programu SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Usuń witrynę z usuniętych witryn za pomocą polecenia cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.

Jeśli tworzysz grupę połączonej witryny i otrzymujesz ostrzeżenie inna grupa o tym samym aliasie już istnieje, Sprawdź istniejące grupy z [pakietu Office 365 z centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Aby rozwiązać ten problem, Usuń istniejącą grupę, jeśli nie jest już potrzebna lub Utwórz witrynę z innym przypisanym aliasem.

Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.

Istniejące witryny można połączyć z grupą 365 pakietu Office. Aby uzyskać więcej informacji, zobacz [łączenie grupy 365 pakietu Office za pomocą ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Aby utworzyć witrynę grupy 365 pakietu Office, należy utworzyć witrynę zespołu. Aby uzyskać więcej informacji, zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

