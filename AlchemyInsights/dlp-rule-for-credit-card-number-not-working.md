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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679451"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemy dotyczące DLP z numerami kart kredytowych

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy dotyczące DLP z numerami kart kredytowych**

Czy problemy związane z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer karty kredytowej** przy użyciu informacji poufnych dla DLP w usłudze Office 365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje, aby wyzwolić zasady DLP podczas jej szacowania. Na przykład w przypadku **zasad dotyczących karty kredytowej** skonfigurowanych z poziomem ufności 85% obliczane są następujące wartości, które muszą zostać wykryte, aby reguła była wyzwalana:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cyfr, które mogą być formatowane lub niesformatowane (dddddddddddddddd) i muszą przebiegać test LUHN.

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Bardzo skomplikowany i niezawodny deseń wykrywający karty ze wszystkich głównych marek na całym świecie, w tym karty Visa, MasterCard, Discover Card, JCB, American Express, karty upominkowe i karty Diner.

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Tak, suma kontrolna LUHN

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Zasady DLP to 85% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:

  - Funkcja Func_credit_card umożliwia Znajdowanie zawartości zgodnej ze wzorcem.

  - Jest spełniony co najmniej jedna z następujących warunków:

  - Znaleziono słowo kluczowe from Keyword_cc_verification.

  - Znaleziono słowo kluczowe z Keyword_cc_name

  - Funkcja Func_expiration_date umożliwia znalezienie daty w prawidłowym formacie daty.

  - Przekazanie sumy kontrolnej

    Na przykład w przypadku numeru karty kredytowej DLP jest wyzwalana następująca przykład:

  - Wiza: 4485 3647 3952 7352
  
  - Wygasa: 2/2009

Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia **numeru karty kredytowej** dla zawartości, zobacz poniższą sekcję w tym artykule: co to są [typy informacji wrażliwych na typ karty kredytowej #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .
  