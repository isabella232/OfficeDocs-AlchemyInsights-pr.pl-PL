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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716901"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemy z połączeniem programu SharePoint Designer 

<p>Jeśli program SharePoint Designer występują problemy z połączeniem do witryn programu SharePoint, prosimy spróbować następujących wspólnych rozwiązań.</p> <p><strong>Krok 1:</strong> <strong>Aktualizacja Sprawdź program SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">Program SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">Dodatek Service Pack 1 (SP1) dla programu SharePoint Designer</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Aktualizacja dla programu SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Krok 2:</strong> <strong>Wyczyścić pliki lokalnej pamięci podręcznej</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Zamknij program SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">Na komputerze lokalnym przejdź do następujących folderów, aby usunąć pliki z pamięci podręcznej.&nbsp;</li> <li style="font-weight: 400;">Kliknij <strong>Start -&gt; uruchomić</strong> i usunąć wszystkie pliki znajdujące się pod każdym z poniżej lokalizacjach.&nbsp;<br /><br />Extensions\Cache serwera %appdata%\Microsoft\Web<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Otwórz program SharePoint Designer 2013 i wprowadzić konto ponownie, aby sprawdzić, czy działa.</li> </ol> <p><strong>Krok 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Włączyć uwierzytelnianie nowoczesnych 2013 pakietu Office na urządzeniach z systemem Windows</strong></a>&nbsp;</p> <p><strong>Krok 4:</strong> <strong>Administratorzy należy umożliwić niestandardowego skryptu, aby umożliwić połączenie programu SharePoint Designer</strong>.</p> <p>Aby uzyskać szczegółowe instrukcje, przykłady i uwagi dotyczące zobacz <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Zezwalaj lub zapobiegania niestandardowy skrypt</a>.&nbsp;</p>


