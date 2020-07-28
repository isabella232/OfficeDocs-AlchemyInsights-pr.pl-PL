---
title: Nie można zmienić nazwy użytkownika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440303"
---
# <a name="unable-to-change-username"></a>Nie można zmienić nazwy użytkownika

W niektórych przypadkach zmiany nazwy UPN (UserPrincipalName) nie są propagowane do chmury. Mogą pojawić się błędy sprawdzania poprawności w portalu usługi Office 365 lub nie można zmienić nazwy użytkownika lub adresu e-mail. Aby rozwiązać ten problem, należy ręcznie ustawić userPrincipalName przy użyciu tego polecenia programu PowerShell.

**Przykład: Zmienianie nazwy użytkownika**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

To polecenie zmienia nazwę davidc@contoso.com na davidchew@contoso.com.

Aby uzyskać więcej informacji, zobacz [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).