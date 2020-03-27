---
title: Reguła DLP dla numeru paszportu USA/Wielkiej Brytanii nie działa
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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977116"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemy z DLP - numery paszportów USA/Wielkiej Brytanii

**Ważne:** W tych bezprecedensowych czasach podejmujemy kroki w celu zapewnienia, że usługi SharePoint Online i OneDrive pozostaną wysoce dostępne — odwiedź [witrynę SharePoint Online, aby](https://aka.ms/ODSPAdjustments) uzyskać więcej informacji.

**Problemy z DLP z numerami paszportów USA/Wielkiej Brytanii**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla treści zawierających **numer paszportu USA / Wielkiej Brytanii** podczas korzystania z DLP typu poufnych informacji w O365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.
  
Na przykład w przypadku zasad **dotyczących numerów paszportów w STANACH Zjednoczonych/Wielkiej Brytanii** skonfigurowanych z poziomem ufności równym 75%, następujące zasady są oceniane i muszą zostać wykryte, aby reguła
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Dziewięć cyfr

- **[Wzór:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Dziewięć kolejnych cyfr

- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie ma sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:

  - Funkcja Func_usa_uk_passport znajduje zawartość, która pasuje do wzorca.

  - Zostanie znalezione słowo kluczowe z Keyword_passport.

    Na przykład następująca próbka spowoduje uruchomienie dla zasad **dotyczących numerów paszportów USA/Wielkiej Brytanii:** numer paszportu USA 123456789

Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia numeru paszportu USA/WIELKIEJ BRYTANII dla twojej zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają numeru paszportu USA/Wielkiej Brytanii](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  