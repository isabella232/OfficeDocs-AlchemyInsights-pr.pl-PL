---
title: Zmienianie adresu e-mail grupy usługi Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283267"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="f748a-102">Zmienianie adresu e-mail grupy usługi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f748a-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="f748a-103">Adres e-mail grupy usługi Microsoft 365 można zmienić za pomocą centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="f748a-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="f748a-104">Wystarczy wybrać grupę i wybrać @edit adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="f748a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f748a-105">Można również użyć następującego polecenia EXO PowerShell, aby zmienić podstawowy adres SMTP grupy microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="f748a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="f748a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="f748a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="f748a-107">Przykład:</span><span class="sxs-lookup"><span data-stu-id="f748a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
