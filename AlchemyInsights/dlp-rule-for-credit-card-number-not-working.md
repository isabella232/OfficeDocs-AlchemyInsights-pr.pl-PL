---
title: Reguła DLP dla numeru karty kredytowej nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28304144"
---
Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer karty kredytowej** , używając typu informacji poufnych DLP w O365? Jeśli tak, upewnij się, treści zawiera informacje potrzebne do wyzwalania zasad DLP podczas szacowania. Na przykład dla **zasad karty kredytowej** skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia: 
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cyfr, które mogą być sformatowane lub niesformatowany (dddddddddddddddd) i musi pomyślnie przejść test Luhna. 
    
- **[Wzór:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Wzór bardzo złożone i niezawodne, który wykrywa kart z wszystkich głównych marek na świecie, w tym Visa, Mastercard, Discover Card, JCB, American Express, kart upominkowych i karty diner. 
    
- **[Suma kontrolna:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Tak, suma kontrolna Luhna 
    
- **[Definicji:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków: 
    
  - Funkcja Func_credit_card znajduje się zawartość, która pasuje do wzorca.
    
  - Spełniony jest jeden z następujących czynności: 
    
  - Znajduje słowa kluczowego z Keyword_cc_verification.
    
  - Znalezione słowa kluczowego z Keyword_cc_name
    
  - Funkcja Func_expiration_date znajdzie datę w formacie daty prawo.
    
  - Przekazuje sumy kontrolnej
    
    Na przykład poniższy przykładowy wywołałoby zasad DLP numer karty kredytowej:
    
  - Wizy: 4485 3647 3952 7352 
    
  - Wygasa: 2/2009
    
Aby uzyskać więcej informacji na to, co jest wymagany **Numer karty kredytowej** wykryć dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy Poszukaj karty kredytowej #](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

