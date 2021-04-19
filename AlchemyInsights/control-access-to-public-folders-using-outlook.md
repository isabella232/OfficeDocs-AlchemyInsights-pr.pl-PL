---
title: Kontrolowanie dostępu do folderów publicznych za pomocą programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816750"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrolowanie dostępu do folderów publicznych za pomocą programu Outlook

Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych za pomocą programu Outlook:

1. Zastosowanie `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w programie Outlook  
$false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook. Jest to wartość domyślna.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Uwaga: Ta procedura może dotyczyć tylko połączeń z programem stacjonarnym Outlook dla klientów systemu Windows. Użytkownicy nadal mogą uzyskać dostęp do folderów publicznych za pomocą aplikacji OWA lub programu Outlook dla komputerów Mac.

Aby uzyskać więcej informacji, zobacz [Kontrolowane połączenia z folderami publicznymi w](https://aka.ms/controlpf) programie Outlook, aby uzyskać więcej informacji.
