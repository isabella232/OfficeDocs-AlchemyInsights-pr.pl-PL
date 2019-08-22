---
title: Dodawanie grupy do witryny programu SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507857"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemy podczas tworzenia lub grupy witryn programu SharePoint Online połączony

Istnieje kilka typowych problemów napotykanych podczas tworzenia lub ponownego tworzenia grupy połączenia witryny.

 Jeśli usunięto grupę i jej witryn połączonych i chcesz utworzyć inną witrynę z tego samego adresu URL, należy trwale usunąć poprzedniej witryny.

Pobierz [powłoki zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Aby uzyskać więcej informacji na temat korzystania ze środowiska powershell zobacz [Online powłoki zarządzania programu SharePoint — wprowadzenie](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Usuń witrynę z witryn usunięte za pomocą polecenia cmdlet [Remove-Spodeletedsitedla](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) środowiska powershell.

Jeśli tworzysz witrynę grupy a pojawia się ostrzeżenie, że innej grupy z takiego samego aliasu już istnieje, sprawdź istniejących grup z [usługi Office 365 z Centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebne lub utworzyć witrynę z inny alias przydzielony.

Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.

Istniejące witryny można połączyć się z grupą usługi Office 365. Aby uzyskać więcej informacji zobacz [Łączenie grupę Office 365 przy użyciu ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Aby utworzyć witrynę połączonych grup usługi Office 365, musisz utworzyć witrynę zespołu. Aby uzyskać więcej informacji zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

