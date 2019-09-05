---
title: Kod błędu 550 5.7.501 odmowa dostępu, wykryto nadużycie spamu
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36740151"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="9eb66-102">550 5.7.501 odmowa dostępu, wykryto nadużycia spamu</span><span class="sxs-lookup"><span data-stu-id="9eb66-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="9eb66-103">Zazwyczaj ten komunikat występuje, gdy użytkownicy wysyłać wiadomości e-mail z adresów IP przy użyciu Initial *. onmicrosoft.com* domeny, która jest przypisana do nowych dzierżawców w pakiecie Office 365.</span><span class="sxs-lookup"><span data-stu-id="9eb66-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="9eb66-104">Najprostszym sposobem rozwiązania tego problemu jest:</span><span class="sxs-lookup"><span data-stu-id="9eb66-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="9eb66-105">[Dodaj domenę do dzierżawy](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="9eb66-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="9eb66-106">[Zmień podstawowy adres e-mail użytkowników](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) na nową domenę niestandardową, którą właśnie dodałeś.</span><span class="sxs-lookup"><span data-stu-id="9eb66-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
