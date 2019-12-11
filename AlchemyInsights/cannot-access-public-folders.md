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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="18172-102">Program Outlook nie może nawiązać połączenia z folderami publicznymi</span><span class="sxs-lookup"><span data-stu-id="18172-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="18172-103">Jeśli dostęp do folderu publicznego nie działa w przypadku kilku użytkowników, wypróbuj następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="18172-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="18172-104">Połącz się z programu PowerShell EXO i skonfiguruj DefaultPublicFolderMailbox na konto użytkownika problem, aby dopasować jeden na konto użytkownika pracy.</span><span class="sxs-lookup"><span data-stu-id="18172-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="18172-105">Przykład:</span><span class="sxs-lookup"><span data-stu-id="18172-105">Example:</span></span>

<span data-ttu-id="18172-106">Get-Skrzynka pocztowa WorkingUser | FT DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="18172-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="18172-107">Zestaw-Mailbox Problemużytkownik-DefaultPublicFolderMailbox \<wartość z poprzedniego polecenia></span><span class="sxs-lookup"><span data-stu-id="18172-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="18172-108">Poczekaj co najmniej jedną godzinę, aby zmiany zostały uwzględnione.</span><span class="sxs-lookup"><span data-stu-id="18172-108">Wait at least one hour for the change to take effect.</span></span>