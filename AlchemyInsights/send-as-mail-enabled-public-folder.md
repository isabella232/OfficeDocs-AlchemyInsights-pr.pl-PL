---
title: Folder publiczny z włączoną funkcją Wyślij jako pocztę w EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461965"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="586ce-102">Folder publiczny z włączoną obsługą poczty SendAs</span><span class="sxs-lookup"><span data-stu-id="586ce-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="586ce-103">W poniższym przykładzie przypisano uprawnienia "Wyślij jako" dla folderu publicznego z włączoną obsługą poczty NewPF1 do Jason użytkownika.</span><span class="sxs-lookup"><span data-stu-id="586ce-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="586ce-104">Add-RecipientPermission-Identity "NewPF1"-powiernik "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="586ce-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="586ce-105">Aby uzyskać szczegółowe informacje o składni i parametrach, zobacz [przypisywanie uprawnień "Wyślij jako" lub "Wyślij w imieniu" dla folderów publicznych z włączoną obsługą poczty](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="586ce-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

