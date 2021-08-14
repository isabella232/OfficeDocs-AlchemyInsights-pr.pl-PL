---
title: SharePoint Problemy z połączeniem projektanta
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942035"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemy z połączeniem projektanta 

Jeśli SharePoint ma problemy z połączeniem z witrynami firmy SharePoint, wypróbuj następujące typowe rozwiązania.

Krok 1. Sprawdź, czy program SharePoint Designer 2013 został zaktualizowany za pomocą dodatku [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) dla programu SharePoint Designer i aktualizacji z 2 sierpnia 2016 r. dla SharePoint [Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



Krok 2. Wyczyść pliki lokalnej pamięci podręcznej:

1. Zamknij SharePoint 2013 Projektanta.

2. Na komputerze lokalnym usuń wszystkie pliki z poniższych folderów.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otwórz SharePoint 2013 i ponownie wprowadź konto, aby sprawdzić, czy działa.

Krok 3. [Włączanie nowoczesnego uwierzytelniania dla Office 2013 na Windows urządzeniach.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

Krok 4. Administratorzy  muszą zezwolić na skrypt niestandardowy w SharePoint centrum administracyjnym, aby zezwolić na połączenie SharePoint Projektanta. Aby [uzyskać więcej informacji, zobacz](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) Zezwalanie na skrypty niestandardowe i zapobieganie im.


