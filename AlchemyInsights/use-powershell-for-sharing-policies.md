---
title: Używanie programu PowerShell w przypadku zasad udostępniania i relacji organizacji
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709476"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Używanie programu PowerShell w przypadku zasad udostępniania i relacji organizacji


W przypadku relacji organizacji przejrzyj szczegółowe informacje dotyczące składni i parametrów dla następujących poleceń: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ORAZ [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Aby utworzyć zasady udostępniania, użyj polecenia [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Aby  [zastosować zasady udostępniania w stosunku do skrzynki pocztowej lub użytkownika ](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  musisz użyć kombinacji poleceń   [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) wraz z nowo utworzonymi zasadami. Aby  [zmodyfikować, wyłączyć lub usunąć zasady udostępniania](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  , musisz użyć poleceń  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Aby w pełni zrozumieć to zagadnienie, przeczytaj artykuł:**

[Udostępnianie w usłudze Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)