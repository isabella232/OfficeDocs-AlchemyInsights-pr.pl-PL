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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719491"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Tworzenie grupy witryn połączonych w dokumentacji Online programu SharePoint

<p><strong>Istnieje kilka typowych problemów napotykanych podczas tworzenia lub ponownego tworzenia grupy połączenia witryny.&nbsp;</strong></p>  <p>1.Jeśli usunięto grupę i jej witryn połączonych i chcesz utworzyć inną witrynę z tego samego adresu URL, należy trwale usunąć poprzedniej witryny.</p>  <ul>  <li>Pobierz <a title="powłoki zarządzania SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Powłoka zarządzania SPO</a> - uzyskać więcej informacji na temat korzystania ze środowiska powershell, zobacz <a title="wprowadzenie do programu SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Wprowadzenie do programu SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Usuń witrynę z witryn usunięte za pomocą <a title="Usuń Spodeletedsitedla" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-Spodeletedsitedla</a> polecenia cmdlet programu powershell.</li>  </ul>  <p>Jeśli tworzysz witrynę grupy i otrzymać ostrzeżenie <strong>'innej grupy z takiego samego aliasu już istnieje'</strong>, Sprawdź istniejące grupy z <a title="Office 365 z Centrum administracyjnego" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Usługi Office 365 z Centrum administracyjnego</a>. Aby rozwiązać ten problem, usuń istniejącą grupę, jeśli nie jest już potrzebne lub utworzyć witrynę z inny alias przydzielony.&nbsp;</p>  <p><strong>Istnieją różne sposoby tworzenia i używania nowoczesnych grup z programem SharePoint.&nbsp;</strong></p>  <ol>  <li>Istniejące witryny można połączyć się z grupą usługi Office 365. Aby uzyskać więcej informacji, zobacz <a title="połączyć grupę Office 365 przy użyciu ineterface użytkownika programu SharePoint" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Połączyć grupę Office 365 przy użyciu programu SharePoint ineterface użytkownik</a>.</li>  <li>Aby utworzyć witrynę połączonych grup usługi Office 365, musisz utworzyć witrynę zespołu. Aby uzyskać więcej informacji, zobacz <a title="utworzyć witrynę zespołu w programie SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Utwórz witrynę zespołu w programie SharePoint.</a></li>  </ol>

