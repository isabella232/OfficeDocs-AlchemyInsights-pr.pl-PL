---
title: Zarządzanie synchronizowanym użytkownikiem
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777687"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika ani usunąć/usunąć synchronizowanego użytkownika

Jeśli dla danego środowiska włączono synchronizację katalogów, niektóre atrybuty użytkowników i obiektów nie mogą być zmieniane przy użyciu Centrum administracyjnego Microsoft 365.

Aby w pełni zarządzać synchronizowanymi użytkownikami i wszystkimi ich atrybutami, użyj konsoli zarządzania lokalni użytkownicy i grupy usługi Active Directory (Adsiedit. msc).  

Możesz też zmienić poszczególnych użytkowników lub atrybuty dla synchronizowanych użytkowników przy użyciu programu PowerShell, takich jak pokazano w następujących typowych przykładach: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
