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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542009"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nie można ustawić podstawowy adres e-mail lub zmienić atrybuty użytkownika

Po włączeniu synchronizacji katalogów w danym środowisku niektórych atrybutów obiektu użytkownika lub nie można zmienić za pomocą Centrum administracyjnego usługi Microsoft 365.

Aby w pełni zarządzać zsynchronizowanych użytkowników i ich atrybutów, użyj lokalną usługę active directory użytkownicy i grupy konsoli zarządzania (adsiedit.msc).  

Można również zmienić poszczególnym użytkownikom lub atrybutów dla użytkowników zsynchronizowanych przy użyciu programu powershell, takich jak pokazano w tych przykładach wspólne: 
- Cmdlettogether - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Cmdlettogether - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Użytkownika testowego" - LastName "Użytkownik"-tytuł "Menedżer"-dział "HR"
- Usuń MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com