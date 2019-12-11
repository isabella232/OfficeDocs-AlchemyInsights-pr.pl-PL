---
title: Nie można uzyskać dostępu do folderów publicznych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959504"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook nie może nawiązać połączenia z folderami publicznymi

Jeśli dostęp do folderu publicznego nie działa w przypadku kilku użytkowników, wypróbuj następujące czynności:

Połącz się z programu PowerShell EXO i skonfiguruj DefaultPublicFolderMailbox na konto użytkownika problem, aby dopasować jeden na konto użytkownika pracy.

Przykład:

Get-Skrzynka pocztowa WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Zestaw-Mailbox Problemużytkownik-DefaultPublicFolderMailbox \<wartość z poprzedniego polecenia>

Poczekaj co najmniej jedną godzinę, aby zmiany zostały uwzględnione.