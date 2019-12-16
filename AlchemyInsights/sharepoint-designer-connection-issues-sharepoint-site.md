---
title: Problemy z połączeniem programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051723"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

Jeśli program SharePoint Designer występuje problemy z połączeniem do witryn programu SharePoint, wypróbuj następujące typowe rozwiązania.

Krok 1: Sprawdź, czy 2013 programu SharePoint Designer jest aktualizowany za pomocą [dodatku Service Pack 1 dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2 sierpnia 2016 aktualizacja dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Wyczyść pliki lokalnej pamięci podręcznej:

1. Zamknij program SharePoint Designer 2013.

2. Na komputerze lokalnym Usuń wszystkie pliki Znalezione w każdym z następujących folderów.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otwórz program SharePoint Designer 2013 i wprowadź ponownie konto, aby sprawdzić, czy działa.

Krok 3: [Włącz nowoczesnych uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Krok 4: Administratorzy będą musieli **zezwolić na niestandardowy skrypt** w ustawieniach centrum administracyjnego programu SharePoint, aby zezwolić na połączenie programu SharePoint Designer. Aby uzyskać więcej informacji, zobacz [Zezwalanie lub zapobieganie skryptowaniu niestandardowym](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


