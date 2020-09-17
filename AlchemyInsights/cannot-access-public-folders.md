---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812557"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook nie może połączyć się z folderami publicznymi

Jeśli dostęp do folderu publicznego nie działa w przypadku niektórym użytkownikom, spróbuj wykonać następujące czynności:

Nawiązywanie połączenia z programem EXO programu PowerShell i Konfigurowanie parametru DefaultPublicFolderMailbox na koncie użytkownika z problemem w celu dopasowania go do parametru na działającym koncie użytkownika.

Przykłady

Get-Skrzynka pocztowa WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Odczekaj co najmniej godzinę, aby zmiana została uwzględniona.

Jeśli problem nadal występuje, wykonaj poniższą [procedurę](https://aka.ms/pfcte) , aby rozwiązać problemy z dostępem do folderów publicznych przy użyciu programu Outlook.
 
**Aby określić, którzy użytkownicy mogą uzyskiwać dostęp do folderów publicznych przy użyciu programu Outlook**:

1.  Użyj ustawień-Casmailboxhttps <mailboxname> -PublicFolderClientAccess $true lub $false  
      
    $true: Zezwalaj użytkownikom na dostęp do folderów publicznych w programie Outlook  
      
    $false: uniemożliwić użytkownikom dostęp do folderów publicznych w programie Outlook. Jest to wartość domyślna.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Uwaga** Ta procedura może kontrolować połączenia tylko z aplikacją pulpitową programu Outlook dla klientów systemu Windows. Użytkownik może nadal uzyskiwać dostęp do folderów publicznych przy użyciu programu OWA lub Outlook dla komputerów Mac.
 
Aby uzyskać więcej informacji, zobacz [ogłaszanie obsługi połączeń sterowanych z folderami publicznymi w programie Outlook](https://aka.ms/controlpf).