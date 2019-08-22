---
title: Problemy z połączeniem programu SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508433"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

Jeśli program SharePoint Designer występują problemy z połączeniem do witryn programu SharePoint, spróbuj następujących wspólnych rozwiązań.

Krok 1: Sprawdź, czy program SharePoint Designer 2013 jest aktualizowana z [dodatku Service Pack 1 dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2 sierpnia 2016 aktualizacja dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Wyczyść pliki lokalnej pamięci podręcznej:

1. Zamknij program SharePoint Designer 2013.

2. Na komputerze lokalnym należy usunąć wszystkie pliki znajdujące się w każdym z następujących folderów.

    - Extensions\Cache serwera %appdata%\Microsoft\Web
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otwórz program SharePoint Designer 2013 i wprowadzić konto ponownie, aby sprawdzić, czy działa.

Krok 3: [Włącz uwierzytelnianie nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).

Krok 4: Administratorzy należy **Umożliwić niestandardowego skryptu** w ustawieniach Centrum administracyjnego programu SharePoint zezwalające na połączenie programu SharePoint Designer. Zobacz [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) uzyskać więcej informacji.


