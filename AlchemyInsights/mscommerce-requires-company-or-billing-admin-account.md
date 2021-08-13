---
title: Połączenie do modułu MS Commerce
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
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974679"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MS Commerce wymaga konta firmy lub administratora rozliczeń

Moduł MS Commerce wymaga konta z uprawnieniami Firma lub Administrator rozliczeń. Jeśli jest wyświetlany następujący błąd, należy ponownie nawiązać połączenie z innym kontem.

*ErrorMessage — serwer zdalny zwrócił błąd: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MS Commerce\1.2\MS Commerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nie można ponownie...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Informacje o kategorii: Nieokreślone: (:) [Błąd zapisu], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Jeśli Twoje konto nie ma uprawnień Firma ani Administrator rozliczeń, skontaktuj się z administratorem IT.
