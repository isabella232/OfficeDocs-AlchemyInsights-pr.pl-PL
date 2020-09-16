---
title: Problemy z połączeniem programu SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727181"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

Jeśli w programie SharePoint Designer występują problemy z połączeniem z witrynami programu SharePoint, Skorzystaj z poniższych typowych rozwiązań.

Krok 1. Upewnij się, że program SharePoint Designer 2013 został zaktualizowany za pomocą [dodatku Service Pack 1 dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [, oraz aktualizacji 2 sierpnia 2016 dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2. Wyczyść lokalne pliki pamięci podręcznej:

1. Zamknij program SharePoint Designer 2013.

2. Na komputerze lokalnym Usuń wszystkie pliki Znalezione w każdym z poniższych folderów.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otwórz program SharePoint Designer 2013 i ponownie wprowadź konto, aby sprawdzić, czy działa.

Krok 3: [Włączanie nowoczesnego uwierzytelniania dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Administratorzy muszą zezwolić na **używanie skryptu niestandardowego** w ustawieniach centrum administracyjnego programu SharePoint, aby umożliwić połączenie programu SharePoint Designer. Aby uzyskać więcej informacji [, zobacz Zezwalanie lub uniemożliwianie niestandardowego skryptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


