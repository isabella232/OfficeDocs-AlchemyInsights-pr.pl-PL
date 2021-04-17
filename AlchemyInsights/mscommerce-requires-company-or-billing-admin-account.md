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
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MS Commerce wymaga konta firmy lub administratora rozliczeń

Moduł MS Commerce wymaga konta z uprawnieniami Firma lub Administrator rozliczeń. Jeśli jest wyświetlany następujący błąd, należy ponownie nawiązać połączenie z innym kontem.

*ErrorMessage — serwer zdalny zwrócił błąd: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MS Commerce\1.2\MS Commerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nie można ponownie...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Informacje o kategorii: Nieokreślone: (:) [Błąd zapisu], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId: Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Jeśli Twoje konto nie ma uprawnień Firma ani Administrator rozliczeń, skontaktuj się z administratorem IT.
