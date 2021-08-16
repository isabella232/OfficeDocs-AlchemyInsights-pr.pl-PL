---
title: Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 7b5acf4dd3061c7d9ed23d52a8355865592b9a1d743025fc9300dcda5a18831a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069254"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego

Aby uzyskać najnowsze informacje na temat sposobu łączenia się z programem PowerShell dla usługi Exchange Online bez używania uwierzytelniania podstawowego, [przejdź tutaj](https://aka.ms/exops-docs). Moduł V2 programu PowerShell nie używa uwierzytelniania podstawowego.

Pamiętaj, że na Twoim komputerze klienckim wciąż musi być włączone uwierzytelnianie podstawowe.
Nowy moduł programu PowerShell V2 korzysta z nowoczesnego uwierzytelniania do nawiązywania połączeń w celu włączenia wszystkich poleceń cmdlet V2 opartych na usłudze REST. Poza poleceniami cmdlet V2 pozwala on również uzyskać dostęp do starszych poleceń cmdlet RPS (Remote PowerShell — zdalna obsługa programu PowerShell), co wymaga ustanowienia sesji zdalnej programu PowerShell. Ustanowienie sesji RPS na komputerze z systemem Windows wymaga, aby na komputerze klienckim było włączone uwierzytelnianie podstawowe, mimo że w celu uwierzytelnienia usługi moduł wykorzystuje nowoczesne uwierzytelnianie. Potok uwierzytelniania podstawowego WinRM jest wykorzystywany do transportu tokenów nowoczesnego uwierzytelniania. Jeśli na komputerze klienckim wyłączone jest uwierzytelnianie podstawowe WinRM, nowe polecenia cmdlet V2 będą nadal działać (ale nie będą działać starsze polecenia cmdlet RPS).
