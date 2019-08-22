---
title: Reguła DLP dla USA / numer paszportu UK nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529929"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemy z DLP - USA / numeru paszportu Wielka Brytania

Czy masz problemy z **Zapobiegania utraty danych (DLP)** nie działa dla zawartości zawierające **USA / Wielka Brytania numer paszportu** podczas używania typu informacji poufnych DLP w O365? Jeśli tak, upewnij się, że zawartość zawiera informacje potrzebne co zasad DLP szuka podczas szacowania.
  
Na przykład, dla **USA / UK numer paszportu** zasada skonfigurowana z 75% poziomu ufności, następujące są oceniane i musi zostać wykryty dla reguły do uruchomienia
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dziewięciu cyfr

- **[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Dziewięciu następujących po sobie cyfr

- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma żadnych suma kontrolna

- **[Definicji:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Zasady DLP wynosi 75% pewność, że wykrył tego rodzaju poufnych informacji, jeżeli w ciągu bliskość 300 znaków:

  - Funkcja Func_usa_uk_passport znajduje się zawartość, która pasuje do wzorca.

  - Znajduje słowa kluczowego z Keyword_passport.

    Na przykład poniższy przykładowy pociągałaby za **USA / Wielka Brytania numer paszportu** zasad: numer paszportu USA 123456789

Aby uzyskać więcej informacji, co jest wymagane do USA / numer paszportu UK wykrycie dla zawartości, zobacz następującą sekcję w tym artykule: [co poufnych informacji typy wyglądu dla Stanów Zjednoczonych / numer paszportu UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Przy użyciu typu różnych wbudowanych poufne informacje, zobacz następujący artykuł informacji na co jest wymagane dla innych typów: [poszukaj co poufnych informacji typy](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  