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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891759"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Program Outlook nie może łączyć się z folderami publicznymi

Jeśli dostęp do folderów publicznych nie działa dla niektórych użytkowników, spróbuj wykonać następujące czynności:

Połącz się z exo powershell i skonfiguruj parametr DefaultPublicFolderMailbox na koncie użytkownika problematycznych, aby dopasować go do parametru na działającym koncie użytkownika.

Przykład:

Get-MailBox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<wartość z poprzedniego polecenia>

Poczekaj co najmniej godzinę, aż zmiana wejdzie w życie.

Jeśli problem występuje, wykonaj [tę procedurę,](https://aka.ms/pfcte) aby rozwiązać problemy z dostępem do folderów publicznych za pomocą programu Outlook.