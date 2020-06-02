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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511554"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

Jeśli program SharePoint Designer ma problemy z połączeniem z witrynami programu SharePoint, wypróbuj następujące typowe rozwiązania.

Krok 1: Sprawdź, czy program SharePoint Designer 2013 jest aktualizowany za pomocą [programu SharePoint Designer z dodatkiem Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [aktualizacji z 2 sierpnia 2016 r. dla programu SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



Krok 2: Wyczyść pliki lokalnej pamięci podręcznej:

1. Zamknij program SharePoint Designer 2013.

2. Na komputerze lokalnym usuń wszystkie pliki znalezione w każdym z następujących folderów.

    - %APPDATA%\Rozszerzenia serwera sieci Web Firmy Microsoft\Pamięć podręczna
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otwórz program SharePoint Designer 2013 i ponownie wprowadź konto, aby sprawdzić, czy działa.

Krok 3: [Włącz nowoczesne uwierzytelnianie dla pakietu Office 2013 na urządzeniach z systemem Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

Krok 4: Administratorzy muszą **zezwolić na skrypt niestandardowy** w ustawieniach Centrum administracyjnego programu SharePoint, aby zezwolić na połączenie programu SharePoint Designer. Aby uzyskać więcej [informacji, zobacz Zezwalaj na skrypt niestandardowy lub zapobiegaj mu.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


