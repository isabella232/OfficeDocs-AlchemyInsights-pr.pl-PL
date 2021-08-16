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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996640"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nie można połączyć się z folderami publicznymi

Jeśli niektórzy użytkownicy nie mogą uzyskać dostępu do folderu publicznego, spróbuj wykonać następujące czynności:

Połączenie z programem EXO PowerShell i skonfiguruj parametr DefaultPublicFolderMailbox na koncie użytkownika problemu w celu dopasowania go do parametru na roboczym koncie użytkownika.

Przykład:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Poczekaj co najmniej godzinę, aby zmiana obowiązywała.

Jeśli problem nadal występuje, wykonaj [tę](https://aka.ms/pfcte) procedurę, aby rozwiązać problemy z dostępem do folderu publicznego przy użyciu Outlook.
 
**Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych przy użyciu Outlook:**

1.  Użyj Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true lub $false  
      
    $true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w Outlook  
      
    $false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook. Jest to wartość domyślna.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Uwaga** Ta procedura pozwala kontrolować połączenia tylko w przypadku Outlook komputerów Windows klientów. Użytkownik może nadal mieć dostęp do folderów publicznych za pomocą aplikacji OWA lub Outlook dla komputerów Mac.
 
Aby uzyskać więcej informacji, zobacz Ogłaszanie obsługi kontrolowanego połączenia z folderami publicznymi w [programie Outlook.](https://aka.ms/controlpf)