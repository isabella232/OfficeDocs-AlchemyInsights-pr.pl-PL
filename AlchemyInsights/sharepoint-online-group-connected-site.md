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
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758740"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Tworzenie grupy witryn połączonych w dokumentacji Online programu SharePoint

Istnieje kilka typowych problemów napotykanych podczas tworzenia lub ponownego tworzenia grupy połączenia witryny.

 Jeśli usunięto grupę i jej witryn połączonych i chcesz utworzyć inną witrynę z tego samego adresu URL, należy trwale usunąć poprzedniej witryny.

Pobierz [powłoki zarządzania SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Aby uzyskać więcej informacji na temat korzystania ze środowiska powershell zobacz [Online powłoki zarządzania programu SharePoint — wprowadzenie](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Usuń witrynę z witryn usunięte za pomocą polecenia cmdlet [Remove-Spodeletedsitedla](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) środowiska powershell.

Jeśli tworzysz witrynę grupy a pojawia się ostrzeżenie, że innej grupy z takiego samego aliasu już istnieje, sprawdź istniejących grup z [usługi Office 365 z Centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebne lub utworzyć witrynę z inny alias przydzielony.

Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.

Istniejące witryny można połączyć się z grupą usługi Office 365. Aby uzyskać więcej informacji zobacz [Łączenie grupę Office 365 przy użyciu ineterface użytkownika programu SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Aby utworzyć witrynę połączonych grup usługi Office 365, musisz utworzyć witrynę zespołu. Aby uzyskać więcej informacji zobacz [Tworzenie witryny zespołu w programie SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

