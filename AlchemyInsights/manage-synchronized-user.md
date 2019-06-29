---
title: Zarządzanie synchronizowanych użytkowników
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380515"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nie można ustawić podstawowy adres e-mail lub zmienić atrybuty użytkownika

Po włączeniu synchronizacji katalogów w danym środowisku niektórych atrybutów obiektu użytkownika lub nie można zmienić przy użyciu Centrum administracyjnego.
Aby w pełni zarządzać zsynchronizowanych użytkowników i ich atrybutów, użyj lokalną usługę active directory użytkownicy i grupy konsoli zarządzania (adsiedit.msc).  

Można również zmienić poszczególnym użytkownikom lub atrybutów dla użytkowników zsynchronizowanych przy użyciu programu powershell, takich jak pokazano w tych przykładach wspólne: 
- Cmdlettogether - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Cmdlettogether - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Użytkownika testowego" - LastName "Użytkownik"-tytuł "Menedżer"-dział "HR"
- Usuń MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com