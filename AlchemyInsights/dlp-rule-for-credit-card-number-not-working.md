---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704211"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemy z DLP z numerami kart kredytowych

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP z numerami kart kredytowych**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer karty kredytowej** podczas korzystania z typu poufnych informacji DLP w UO365? Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne do wyzwolenia zasad DLP, gdy jest oceniana. Na przykład dla **zasad kart kredytowych** skonfigurowanych z poziomem zaufania równym 85%, aby reguła wyzwoliła, należy wykryć następujące zasady:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowane (ddddddddddddddd) i muszą przejść test Luhna.

- **[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Bardzo złożony i solidny wzór, który wykrywa karty wszystkich głównych marek na całym świecie, w tym Visa, MasterCard, Discover Card, JCB, American Express, karty upominkowe i karty do kolacji.

- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna

- **[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP są w 85% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:

  - Funkcja Func_credit_card znajduje zawartość, która pasuje do wzorca.

  - Jedna z następujących elementów jest prawdziwa:

  - Zostanie znalezione słowo kluczowe z Keyword_cc_verification.

  - Znaleziono słowo kluczowe z Keyword_cc_name

  - Funkcja Func_expiration_date znajduje datę w odpowiednim formacie daty.

  - Suma kontrolna przechodzi

    Na przykład następujący przykład może wyzwolić zasady numeru karty kredytowej DLP:

  - Wiza: 4485 3647 3952 7352
  
  - Wygasa: 2/2009

Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia **numeru karty kredytowej** dla twojej zawartości, zobacz następującą sekcję w tym artykule: Jakie [typy poufnych informacji szukają dla karty kredytowej#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  