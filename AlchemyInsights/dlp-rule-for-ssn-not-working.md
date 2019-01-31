---
title: Reguła DLP dla numeru PESEL nie działa
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 7242bf2b101b45fec0fe00ab33fa6db150004ee5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657369"
---
Czy występują problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **Numer PESEL (SSN)** podczas używania typu informacji poufnych w usłudze Office 365? Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne dla czego szuka zasad DLP. 
  
Na przykład polityki SSN skonfigurowany z poziomu ufności 85%, następujące czynności są oceniane i musi zostać wykryty dla reguły do uruchomienia:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cyfr, które mogą być we wzorcu sformatowaną lub niesformatowaną 
    
- **[Wzór:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje szukać SSNs w czterech różnych wzorów: 
    
  - Func_ssn znajdzie SSNs z pre-2011 silne formatowania, które są sformatowane za pomocą kresek ani spacji (ddd-dd-dddd lub ddd dd dddd)
    
  - Func_unformatted_ssn znajdzie SSNs z pre-2011 silne formatowania, które są formatowane jako dziewięciu następujących po sobie cyfr (ddddddddd)
    
  - Func_randomized_formatted_ssn znajdzie SSNs post-2011, które są sformatowane za pomocą kresek ani spacji (ddd-dd-dddd lub ddd dd dddd)
    
  - Func_randomized_unformatted_ssn znajdzie SSNs post-2011, które są formatowane jako dziewięciu następujących po sobie cyfr (ddddddddd)
    
- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie ma żadnych suma kontrolna 
    
- **[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Zasady DLP jest 85% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków: 
    
  - [Funkcja Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) znajduje się zawartość, która pasuje do wzorca. 
    
  - Znajduje słowa kluczowego z [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Zawiera przykłady słów kluczowych: *zabezpieczenia społecznego, zabezpieczenia społecznego #, s Soc, numer PESEL* . Na przykład poniższy przykładowy wywołałoby zasad DLP SSN: **SSN: 489-36-8350**
    
Aby uzyskać więcej informacji na co jest wymagane dla SSNs do wykrycia dla zawartości, zobacz następującą sekcję w tym artykule: [Co poufnych informacji typy szukać SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

