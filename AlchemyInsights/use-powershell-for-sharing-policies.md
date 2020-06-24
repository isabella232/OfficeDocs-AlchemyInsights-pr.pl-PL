---
title: Używanie programu PowerShell do udostępniania zasad i relacji organizacyjnych
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862151"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Używanie programu PowerShell do udostępniania zasad i relacji organizacyjnych


W przypadku relacji organizacji zapoznaj się ze szczegółowymi informacjami o składni i parametrach: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) and [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Aby utworzyć zasady udostępniania, użyj [new-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Aby [zastosować zasady udostępniania do skrzynki pocztowej lub użytkownika,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) należy użyć kombinacji Skrzynki [pocztowej](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [Skrzynki odbiorczej](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) z nowo utworzonymi zasadami. Aby [zmodyfikować, wyłączyć lub usunąć zasady udostępniania,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) które należy użyć [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Aby uzyskać pełne zrozumienie tego tematu, przeczytaj:**

[Udostępnianie w usłudze Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)