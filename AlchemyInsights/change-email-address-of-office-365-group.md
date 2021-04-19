---
title: Zmienianie adresu e-mail grupy platformy Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819054"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="0a8cc-102">Zmienianie adresu e-mail grupy platformy Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0a8cc-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="0a8cc-103">Za pomocą centrum administracyjnego możesz zmienić adres e-mail grupy usługi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0a8cc-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="0a8cc-104">Po prostu zaznacz grupę, a następnie wybierz pozycję @edytuj adres e-mail.</span><span class="sxs-lookup"><span data-stu-id="0a8cc-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="0a8cc-105">Podstawowy adres SMTP grupy platformy Microsoft 365 można również zmienić za pomocą polecenia PROGRAMU EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0a8cc-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="0a8cc-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="0a8cc-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="0a8cc-107">Przykład: </span><span class="sxs-lookup"><span data-stu-id="0a8cc-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
