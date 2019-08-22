---
title: Konwertowanie skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496445"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Konwertowanie skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej

Skrzynki pocztowej użytkownika można konwertować na udostępnionej skrzynki pocztowej tylko, jeśli użytkownik ma licencję Exchange. Po przekonwertowaniu skrzynki pocztowej, nadal będzie wyświetlane na liście aktywnych użytkowników, ponieważ ten wykaz zawiera udostępnionych skrzynek pocztowych. Jednak przekonwertowane skrzynki pocztowej także pojawi się na liście udostępnionej skrzynki pocztowej. 
  
Jeśli podczas próby konwersji skrzynek pocztowych w konsoli administracyjnej programu Exchange i konwersja kończy się niepowodzeniem, wyczyść pamięć podręczną przeglądarki i pliki cookie i spróbuj ponownie. Jeśli nadal nie działa, spróbuj wykonać konwersji skrzynki pocztowej w programu Exchange Management Shell, uruchamiając następujące polecenie:
  
```
Set-Mailbox -Type Shared
```

Więcej informacji o konwersji skrzynki pocztowej jest dostępna w [konwersji skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
