---
title: Lokalizacja danych
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207271"
---
# <a name="data-location"></a>Lokalizacja danych

Można wyświetlić lokalizację dzierżawy pakietu Office 365 w centrum administracyjnym lub łącząc się z usługą Exchange Online za pomocą programu PowerShell.


**Centrum administracyjne:**
1. Zaloguj się w [centrum administracyjnym](https://admin.microsoft.com/Adminportal/Home).
2. Wybierz pozycję **Ustawienia** > **profilu organizacji**.
3. W obszarze **Lokalizacja danych**wybierz pozycję **Wyświetl szczegóły**.


**Powershell:**
1. Połącz się z usługą Exchange Online przy użyciu programu Windows PowerShell.
2. Wykonanie [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) polecenia cmdlet, aby wyświetlić listę właściwości dzierżawy. 
3. Spójrz na Właściwość OrganizationId.

Jeśli masz lokalizację danych dla EXO i SPO, można określić lokalizację danych dla innych usług, które mogą być używane z [gdzie znajdują się dane](https://products.office.com/where-is-your-data-located).