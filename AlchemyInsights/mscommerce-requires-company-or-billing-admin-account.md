---
title: Nawiązywanie połączenia z modułem MS Commerce
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829746"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="b9dcb-102">MS Commerce wymaga konta firmy lub administratora rozliczeń</span><span class="sxs-lookup"><span data-stu-id="b9dcb-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="b9dcb-103">Moduł MS Commerce wymaga konta z uprawnieniami Firma lub Administrator rozliczeń.</span><span class="sxs-lookup"><span data-stu-id="b9dcb-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="b9dcb-104">Jeśli jest wyświetlany następujący błąd, należy ponownie nawiązać połączenie z innym kontem.</span><span class="sxs-lookup"><span data-stu-id="b9dcb-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="b9dcb-105">*ErrorMessage — serwer zdalny zwrócił błąd: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MS Commerce\1.2\MS Commerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="b9dcb-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="b9dcb-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nie można ponownie...*</span><span class="sxs-lookup"><span data-stu-id="b9dcb-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="b9dcb-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="b9dcb-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="b9dcb-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Informacje o kategorii: Nieokreślone: (:) [Błąd zapisu], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="b9dcb-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="b9dcb-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="b9dcb-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="b9dcb-110">Jeśli Twoje konto nie ma uprawnień Firma ani Administrator rozliczeń, skontaktuj się z administratorem IT.</span><span class="sxs-lookup"><span data-stu-id="b9dcb-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
