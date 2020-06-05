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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580667"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="ed1c3-102">Zmienianie adresu e-mail grupy usługi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ed1c3-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="ed1c3-103">Adres e-mail grupy usługi Microsoft 365 można zmienić za pomocą centrum administracyjnego.</span><span class="sxs-lookup"><span data-stu-id="ed1c3-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="ed1c3-104">Wystarczy wybrać grupę i wybrać @edit adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="ed1c3-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="ed1c3-105">Można również użyć następującego polecenia EXO PowerShell, aby zmienić podstawowy adres SMTP grupy microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="ed1c3-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="ed1c3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="ed1c3-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="ed1c3-107">Przykład:</span><span class="sxs-lookup"><span data-stu-id="ed1c3-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
