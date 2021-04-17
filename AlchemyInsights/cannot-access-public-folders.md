---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819522"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook nie może połączyć się z folderami publicznymi

Jeśli niektórzy użytkownicy nie mogą uzyskać dostępu do folderu publicznego, spróbuj wykonać następujące czynności:

Połącz się z programem POWERShell programu EXO i skonfiguruj parametr DefaultPublicFolderMailbox na koncie użytkownika problemu, aby dopasować go do parametru na roboczym koncie użytkownika.

Przykład: 

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Poczekaj co najmniej godzinę, aby zmiana obowiązywała.

Jeśli problem pozostanie, [](https://aka.ms/pfcte) wykonaj tę procedurę, aby rozwiązać problemy z dostępem do folderu publicznego przy użyciu programu Outlook.
 
**Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych za pomocą programu Outlook:**

1.  Użyj Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true lub $false  
      
    $true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w programie Outlook  
      
    $false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook. Jest to wartość domyślna.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Uwaga** Ta procedura pozwala kontrolować połączenia tylko za pomocą klasycznego programu Outlook dla klientów systemu Windows. Użytkownik może nadal mieć dostęp do folderów publicznych przy użyciu aplikacji OWA lub Outlook dla komputerów Mac.
 
Aby uzyskać więcej informacji, zobacz Ogłaszanie obsługi kontrolowanego połączenia z folderami [publicznymi w programie Outlook.](https://aka.ms/controlpf)