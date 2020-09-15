---
title: Nawiązywanie połączenia z modułem MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 15dc7038426a8d436c236a91aa0f3462f6a3e366
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702625"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="46047-102">MSCommerce wymaga konta administratora firmy lub rozliczeń</span><span class="sxs-lookup"><span data-stu-id="46047-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="46047-103">Moduł MSCommerce wymaga konta z uprawnieniami firmy lub administratora rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="46047-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="46047-104">Jeśli otrzymasz następujący komunikat o błędzie, konieczne będzie ponowne nawiązanie połączenia przy użyciu innego konta.</span><span class="sxs-lookup"><span data-stu-id="46047-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="46047-105">*ErrorMessage — serwer zdalny zwrócił błąd: (403) zabroniony. ErrorDetails-at C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 znak: 5*</span><span class="sxs-lookup"><span data-stu-id="46047-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="46047-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError-ErrorContext $ _-CustomErrorMessage "nie można retri...*</span><span class="sxs-lookup"><span data-stu-id="46047-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="46047-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="46047-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="46047-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="46047-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="46047-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft. PowerShell. Commands. WriteErrorException, HandleError*</span><span class="sxs-lookup"><span data-stu-id="46047-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="46047-110">Jeśli konto nie ma uprawnień administratora firmy lub konta Administrator, skontaktuj się z administratorem IT.</span><span class="sxs-lookup"><span data-stu-id="46047-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
