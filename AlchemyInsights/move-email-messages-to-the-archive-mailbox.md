---
title: Przenoszenie wiadomości e-mail do skrzynki pocztowej archiwum
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762375"
---
# <a name="move-email-to-the-archive-mailbox"></a>Przenoszenie wiadomości e-mail do skrzynki pocztowej archiwum
 
1. Upewnij się, że **archiwum skrzynki pocztowej** zostało włączone. Jeśli tak nie jest, wykonaj kroki w [tym artykule](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , aby umożliwić archiwum skrzynki pocztowej.

2. Aby zarchiwizować wiadomości automatycznie do archiwum skrzynki pocztowej, tag przechowywania za pomocą operacji **Przenieś do archiwum** musi być równa **stosowane automatycznie do znaczników całej skrzynki pocztowej (ustawienie domyślne)**. Wykonaj kroki w tym miejscu, aby utworzyć znacznik: [domyślne archiwum tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Następnie należy dodać tag **archiwum** do zasad przechowywania. W Centrum administracyjnego programu Exchange, wybierz **Zasady przechowywania** > dodać **Przenieś do archiwum tag** do > zasady **zapisywania**. 
    
4. Teraz [Przypisywanie zasad przechowywania](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) do skrzynki pocztowej danego użytkownika. Takie same zasady zostaną zastosowane do **podstawowego** i **archiwum** skrzynki pocztowej. 
    
Może być konieczne wymuszenie zarządzanych folderów Asystenta (MFA) do uruchomienia i Zastosuj nowe ustawienia do skrzynki pocztowej danego użytkownika. Uruchom następujące polecenie podczas [podłączony do środowiska PowerShell EKSO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) uruchomić Asystenta folderów zarządzanych w konkretnej skrzynce pocztowej: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Aby uzyskać więcej informacji o konfigurowaniu zasad archiwizacji zobacz [Konfigurowanie zasad archiwizacji i usuwania dla skrzynek pocztowych](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

