---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005100"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemy z DLP dotyczące numerów kart kredytowych

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP dotyczące numerów kart kredytowych**

Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention)** nie działa w przypadku zawartości zawierającej numer karty kredytowej podczas korzystania z typu informacji poufnych związanych z zapobieganiem utracie danych w u usługi O365?  Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne do uruchomienia zasad DLP podczas ich oceny. Na przykład w  przypadku zasad karty kredytowej skonfigurowanych z poziomem ufności 85% następujące zasady są sprawdzane i muszą zostać wykryte, aby uruchamiała regułę:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowane (ddddddddd) i muszą przejść test Luhna.

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Bardzo złożony i niezawodny wzór, który wykrywa karty od wszystkich głównych marek na całym świecie, w tym Visa, MasterCard, Discover Card, JCB, American Express, bony upominkowe i karty wyeksłowe.

- **[Sumy kontrolne:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Tak, w przypadku sumy kontrolnej Luhna

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zasady DLP mają 85% pewności, że wykrywane są tego typu informacje poufne, jeśli w odległości 300 znaków:

  - Funkcja Func_credit_card znajdzie zawartość, która pasuje do wzorca.

  - Prawdziwe jest jedno z następujących argumentów:

  - Słowo kluczowe z Keyword_cc_verification znajduje się.

  - Słowo kluczowe z Keyword_cc_name znajduje się

  - Funkcja Func_expiration_date znajdzie datę w odpowiednim formacie daty.

  - Sumy kontrolne przechodzą przez

    Na przykład następująca próbka może spowodować uruchomienie zasad numerowania kart kredytowych DLP:

  - Visa: 4485 3647 3952 7352
  
  - Wygasa: 2009-02-02

Aby uzyskać więcej informacji na  temat tego, co jest wymagane, aby numer karty kredytowej był wykrywany dla zawartości, zobacz następującą sekcję w tym artykule: Typy informacji poufnych mają wartość Karta [kredytowa#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Informacje wymagane dla innych typów można znaleźć w następującym artykule, w którym podano informacje o innych [typach:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Typy informacji poufnych
  