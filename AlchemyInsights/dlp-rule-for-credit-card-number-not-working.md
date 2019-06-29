---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389587"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemy dotyczące DLP numery kart kredytowych

Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer karty kredytowej** , używając typu informacji poufnych DLP w O365? Jeśli tak, upewnij się, treści zawiera informacje potrzebne do wyzwalania zasad DLP podczas szacowania. Na przykład dla **zasad karty kredytowej** skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowany (dddddddddddddddd) i musi pomyślnie przejść test Luhna.

- **[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Wzór bardzo złożone i niezawodne, który wykrywa kart z wszystkich głównych marek na świecie, w tym Visa, MasterCard, Discover Card, JCB, American Express, kart upominkowych i karty diner.

- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna

- **[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:

  - Funkcja Func_credit_card znajduje się zawartość, która pasuje do wzorca.

  - Spełniony jest jeden z następujących czynności:

  - Znajduje słowa kluczowego z Keyword_cc_verification.

  - Znalezione słowa kluczowego z Keyword_cc_name

  - Funkcja Func_expiration_date znajdzie datę w formacie daty prawo.

  - Przekazuje sumy kontrolnej

    Na przykład poniższy przykładowy wywołałoby zasad DLP numer karty kredytowej:

  - Wizy: 4485 3647 3952 7352
  
  - Wygasa: 2/2009

Aby uzyskać więcej informacji na to, co jest wymagany **Numer karty kredytowej** wykryć dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy Poszukaj karty kredytowej #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  