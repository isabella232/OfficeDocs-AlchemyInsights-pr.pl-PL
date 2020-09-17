---
title: Kod błędu 550 5.7.501 — odmowa dostępu, wykryto nadużycia spamu
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 6542450ca4d03daef4a7f63783d431d2091bc5e7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784065"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="c5b69-102">550 5.7.501 — odmowa dostępu, wykryto nadużycia spamu</span><span class="sxs-lookup"><span data-stu-id="c5b69-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="c5b69-103">Zazwyczaj ten komunikat jest wyświetlany, gdy użytkownicy wysyłają wiadomości e-mail z adresów IP przy użyciu początkowej domeny *. onmicrosoft.com* , która jest przypisana do nowych dzierżawców w programie Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c5b69-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="c5b69-104">Najprostszym sposobem rozwiązania tego problemu jest:</span><span class="sxs-lookup"><span data-stu-id="c5b69-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="c5b69-105">[Dodaj domenę do dzierżawy](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="c5b69-105">[Add a domain to your tenant](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="c5b69-106">[Zmień podstawowy adres e-mail użytkownika](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) na nowo dodaną domenę niestandardową.</span><span class="sxs-lookup"><span data-stu-id="c5b69-106">[Change your users' primary email address](https://docs.microsoft.com/microsoft-365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
