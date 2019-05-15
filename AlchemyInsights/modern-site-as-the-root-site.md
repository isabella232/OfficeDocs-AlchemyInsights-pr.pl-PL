---
title: Nowoczesne witryny jako witryny głównej
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057751"
---
# <a name="modern-site-as-root-site"></a>Nowoczesne witryny jako witryny głównej

Klienci [Wersji docelowej](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) można włączyć teraz doświadczenie strony nowoczesnej komunikacji w miejscu głównego klasyczne ich dzierżawcy programu SharePoint.

Tę funkcję można aktywować za pomocą prostego polecenia cmdlet programu PowerShell. Na pomyślne wykonanie polecenia środowiska PowerShell witryny głównej ma nową stronę główną witryny komunikacji. Szczegóły dotyczące wymagań funkcji i polecenia cmdlet środowiska PowerShell są dostępne w artykule [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps). 

Firma Microsoft będzie być wprowadzana stopniowo tę możliwość, off domyślnie klientom ukierunkowane zwolnienia z początku maja 2019, a roll się będzie dostępny na całym świecie do końca czerwca 2019. Nadal odnoszą się do [Centrum wiadomości](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) dla innych nowych funkcji z nowoczesnymi. 

**Ważne**: nie należy usuwać klasyczny głównej witrynie do tworzenia nowoczesnych witryny komunikacji. Nie jest to obsługiwane przez firmę Microsoft. Usunięcie katalogu głównego witryny spowoduje, że wszystkie witryny programu SharePoint w organizacji niedostępne dla wszystkich użytkowników, dopóki Przywracanie witryny lub utworzyć nową witrynę o takim samym adresie URL. 
 
 