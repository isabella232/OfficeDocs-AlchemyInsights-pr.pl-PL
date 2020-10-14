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
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451410"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nie można ustawić podstawowego adresu e-mail, zmienić atrybutów użytkownika ani usunąć/usunąć synchronizowanego użytkownika

Jeśli dla danego środowiska włączono synchronizację katalogów, niektóre atrybuty użytkowników i obiektów nie mogą być zmieniane przy użyciu Centrum administracyjnego Microsoft 365.

Aby w pełni zarządzać synchronizowanymi użytkownikami i wszystkimi ich atrybutami, użyj konsoli zarządzania lokalni użytkownicy i grupy usługi Active Directory (Adsiedit. msc).  

Możesz też zmienić poszczególnych użytkowników lub atrybuty dla synchronizowanych użytkowników przy użyciu programu PowerShell, takich jak pokazano w następujących typowych przykładach:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
