---
title: Kontrolowanie dostępu do folderów publicznych za pomocą Outlook
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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032568"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrolowanie dostępu do folderów publicznych za pomocą Outlook

Aby kontrolować, którzy użytkownicy mogą uzyskać dostęp do folderów publicznych przy użyciu Outlook:

1. Zastosowanie `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: Zezwalaj użytkownikom na uzyskiwanie dostępu do folderów publicznych w Outlook  
$false: Uniemożliwianie użytkownikowi dostępu do folderów publicznych w programie Outlook. Jest to wartość domyślna.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Uwaga: Ta procedura może dotyczyć tylko Outlook komputerowych dla Windows klientów. Użytkownicy mogą nadal mieć dostęp do folderów publicznych za pomocą aplikacji OWA Outlook dla komputerów Mac.

Aby uzyskać więcej informacji, zobacz Kontrolowane połączenia z folderami publicznymi w [programie Outlook,](https://aka.ms/controlpf) aby uzyskać więcej informacji.
