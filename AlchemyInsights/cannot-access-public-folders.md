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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6f43a-102">Program Outlook nie może łączyć się z folderami publicznymi</span><span class="sxs-lookup"><span data-stu-id="6f43a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6f43a-103">Jeśli dostęp do folderów publicznych nie działa dla niektórych użytkowników, spróbuj wykonać następujące czynności:</span><span class="sxs-lookup"><span data-stu-id="6f43a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="6f43a-104">Połącz się z exo powershell i skonfiguruj parametr DefaultPublicFolderMailbox na koncie użytkownika problematycznych, aby dopasować go do parametru na działającym koncie użytkownika.</span><span class="sxs-lookup"><span data-stu-id="6f43a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="6f43a-105">Przykład:</span><span class="sxs-lookup"><span data-stu-id="6f43a-105">Example:</span></span>

<span data-ttu-id="6f43a-106">Get-MailBox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox ft DefaultPublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="6f43a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6f43a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<wartość z poprzedniego polecenia></span><span class="sxs-lookup"><span data-stu-id="6f43a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6f43a-108">Poczekaj co najmniej godzinę, aż zmiana wejdzie w życie.</span><span class="sxs-lookup"><span data-stu-id="6f43a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="6f43a-109">Jeśli problem występuje, wykonaj [tę procedurę,](https://aka.ms/pfcte) aby rozwiązać problemy z dostępem do folderów publicznych za pomocą programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f43a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>