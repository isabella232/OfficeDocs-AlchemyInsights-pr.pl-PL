---
title: Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: pl-PL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015699"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Program Exchange PowerShell i wycofanie uwierzytelniania podstawowego

Aby uzyskać najnowsze informacje na temat sposobu łączenia się z programem PowerShell dla usługi Exchange Online bez używania uwierzytelniania podstawowego, [przejdź tutaj](https://aka.ms/psbasicauth).

Pamiętaj, że na Twoim komputerze klienckim wciąż musi być włączone uwierzytelnianie podstawowe.
Nowy moduł programu PowerShell V2 korzysta z nowoczesnego uwierzytelniania do nawiązywania połączeń w celu włączenia wszystkich poleceń cmdlet V2 opartych na usłudze REST. Poza poleceniami cmdlet V2 pozwala on również uzyskać dostęp do starszych poleceń cmdlet RPS (Remote PowerShell — zdalna obsługa programu PowerShell), co wymaga ustanowienia sesji zdalnej programu PowerShell. Ustanowienie sesji RPS na komputerze z systemem Windows wymaga, aby na komputerze klienckim było włączone uwierzytelnianie podstawowe, mimo że w celu uwierzytelnienia usługi moduł wykorzystuje nowoczesne uwierzytelnianie. Potok uwierzytelniania podstawowego WinRM jest wykorzystywany do transportu tokenów nowoczesnego uwierzytelniania. Jeśli na komputerze klienckim wyłączone jest uwierzytelnianie podstawowe WinRM, nowe polecenia cmdlet V2 będą nadal działać (ale nie będą działać starsze polecenia cmdlet RPS).
