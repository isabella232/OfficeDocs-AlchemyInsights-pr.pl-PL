---
title: Zarządzanie zsynchronizowanym użytkownikiem
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114788"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika ani usunąć zsynchronizowanego użytkownika

Jeśli w środowisku włączono synchronizację katalogów, niektórych atrybutów użytkowników lub obiektów nie można zmienić przy użyciu centrum administracyjne platformy Microsoft 365.

Aby w pełni zarządzać zsynchronizowanymi użytkownikami i ich wszystkimi atrybutami, użyj lokalnej konsoli zarządzania użytkownikami i grupami usługi Active Directory (adsiedit.msc).  

Możesz również zmienić pojedynczych użytkowników lub atrybuty dla zsynchronizowanych użytkowników za pomocą programu PowerShell, jak pokazano w tych typowych przykładach:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
