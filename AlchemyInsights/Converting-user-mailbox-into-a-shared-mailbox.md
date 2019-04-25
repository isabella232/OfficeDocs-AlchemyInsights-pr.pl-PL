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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374333"
---
Skrzynki pocztowej użytkownika można konwertować na udostępnionej skrzynki pocztowej tylko, jeśli użytkownik ma licencję Exchange. Po przekonwertowaniu skrzynki pocztowej, nadal będzie wyświetlane na liście aktywnych użytkowników, ponieważ ten wykaz zawiera udostępnionych skrzynek pocztowych. Jednak przekonwertowane skrzynki pocztowej także pojawi się na liście udostępnionej skrzynki pocztowej. 
  
Jeśli podczas próby konwersji skrzynek pocztowych w konsoli administracyjnej programu Exchange i konwersja kończy się niepowodzeniem, wyczyść pamięć podręczną przeglądarki i pliki cookie i spróbuj ponownie. Jeśli nadal nie działa, spróbuj wykonać konwersji skrzynki pocztowej w programu Exchange Management Shell, uruchamiając następujące polecenie:
  
```
Set-Mailbox -Type Shared
```

Więcej informacji o konwersji skrzynki pocztowej jest dostępna w [konwersji skrzynki pocztowej użytkownika na udostępnionej skrzynki pocztowej](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
