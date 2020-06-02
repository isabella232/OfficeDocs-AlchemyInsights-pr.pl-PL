---
title: Reguła DLP dla numeru konta bankowego w USA nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507344"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemy z DLP z numerami amerykańskich kont bankowych

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP z numerami amerykańskich kont bankowych**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer konta bankowego w USA** podczas korzystania z typu poufnych informacji DLP w UO365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.
  
Na przykład dla zasad **numeru konta bankowego w USA** skonfigurowanych z poziomem zaufania równym 85%, aby reguła wyzwoliła, są oceniane następujące zasady:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cyfr

- **[Wzór:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 kolejnych cyfr.

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:

  - Wyrażenie regularne Regex_usa_bank_account_number znajduje zawartość odpowiadającą wzorcowi

  - Zostanie znalezione słowo kluczowe z Keyword_usa_Bank_Account.

    Na przykład następujący przykład może wyzwolić zasady **numeru konta bankowego w USA:** Sprawdzanie konta 78344011

Aby uzyskać więcej informacji na temat tego, co jest wymagane do **wykrycia numeru konta bankowego w USA** dla zawartości, zobacz następującą sekcję w tym artykule: Jakie [typy poufnych informacji szukają numeru konta bankowego w USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  