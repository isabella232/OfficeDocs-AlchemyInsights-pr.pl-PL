---
title: Zarządzanie zsynchronizowanym użytkownikiem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407360"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika lub usunąć/usunąć zsynchronizowanego użytkownika

Jeśli synchronizacja katalogów jest włączona w twoim środowisku, nie można zmienić niektórych atrybutów użytkownika lub obiektu za pomocą centrum administracyjnego usługi Microsoft 365.

Aby w pełni zarządzać zsynchronizowanymi użytkownikami i wszystkimi ich atrybutami, użyj lokalnej konsoli zarządzania usługi Active Directory (adsiedit.msc).  

Alternatywnie można zmienić poszczególnych użytkowników lub atrybuty dla zsynchronizowanych użytkowników przy użyciu programu PowerShell, takie jak pokazano w poniższych typowych przykładach: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
