---
title: Reguła DLP dla nas numer konta bankowego nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29482554"
---
Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer konta bankowego w Stanach Zjednoczonych** , używając typu informacji poufnych DLP w O365? Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne co zasad DLP szuka podczas szacowania. 
  
Na przykład dla zasady **Numer konta bankowego w Stanach Zjednoczonych** , skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia: 
  
- **[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cyfr 
    
- **[Wzór:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 cyfr. 
    
- **[Suma kontrolna:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma żadnych suma kontrolna 
    
- **[Definicji:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Zasady DLP wynosi 75% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków: 
    
  - Wyrażenie regularne Regex_usa_bank_account_number znajduje się zawartość, która pasuje do wzorca
    
  - Znajduje słowa kluczowego z Keyword_usa_Bank_Account.
    
    Na przykład poniższy przykładowy wywołałoby zasady **Numer konta bankowego w Stanach Zjednoczonych** : 78344011 konto bankowe 
    
Aby uzyskać więcej informacji na co jest wymagane dla **USA numer konta bankowego** do wykrycia dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy wyszukać numer konta bankowego w Stanach Zjednoczonych](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

