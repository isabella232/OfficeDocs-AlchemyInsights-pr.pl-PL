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
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655292"
---
# <a name="data-location"></a>Lokalizacja danych

Lokalizację dzierżawy można wyświetlić w centrum administracyjnym lub łącząc się z usługą Exchange Online za pośrednictwem programu PowerShell.


**Centrum administracyjne:**
1. Zaloguj się do [centrum administracyjnego](https://admin.microsoft.com/Adminportal/Home).
2. Wybierz **pozycję Ustawienia** > **profilu organizacji**.
3. W obszarze **Lokalizacja danych**wybierz pozycję **Wyświetl szczegóły**.


**Powershell:**
1. Połącz się z usługą Exchange Online przy użyciu programu Windows PowerShell.
2. Wykonaj polecenie cmdlet [Get-OrganizationalUnit,](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) aby wyświetlić listę właściwości dzierżawy. 
3. Spójrz na OrganizationId właściwości.

Jeśli masz lokalizację danych dla EXO i SPO, możesz określić lokalizację danych dla innych usług, z których można korzystać, z [miejsca, w którym znajdują się dane.](https://products.office.com/where-is-your-data-located)