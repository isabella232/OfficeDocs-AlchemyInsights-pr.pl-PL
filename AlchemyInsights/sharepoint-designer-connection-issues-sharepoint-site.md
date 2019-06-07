---
title: Poziomy uprawnień programu SharePoint w trybie Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760702"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

Jeśli program SharePoint Designer występują problemy z połączeniem do witryn programu SharePoint, prosimy spróbować następujących wspólnych rozwiązań.

Krok 1: Sprawdź aktualizacja programu SharePoint Designer.

- [Program SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [Dodatek Service Pack 1 (SP1) dla programu SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [Aktualizacja dla programu SharePoint Designer 2013 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

Krok 2: Wyczyść lokalnej pamięci podręcznej plików

- Zamknij program SharePoint Designer 2013.

- Na komputerze lokalnym przejdź do następujących folderów, aby usunąć pliki z pamięci podręcznej.

- Kliknij przycisk Start, uruchom i Usuń wszystkie pliki znajdują się w obszarze każdego z poniżej lokalizacjach.

Serwer %appdata%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

Otwórz program SharePoint Designer 2013 i wprowadzić konto ponownie, aby sprawdzić, czy działa.

Krok 3: [Włącz uwierzytelnianie nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

Krok 4: Administratorzy należy umożliwić niestandardowego skryptu zezwalające na połączenie programu SharePoint Designer.

Aby uzyskać szczegółowe instrukcje, przykłady i uwagi dotyczące zobacz [Zezwalaj lub zapobiegania niestandardowy skrypt](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


