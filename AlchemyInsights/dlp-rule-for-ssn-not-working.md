---
title: Reguła DLP dla SSN nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788712"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemy Z DLP z numerami ubezpieczenia społecznego

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP z sieciami SSN**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla zawartości zawierającej **numer ubezpieczenia społecznego (SSN)** podczas korzystania z typu poufnych informacji w usłudze Microsoft 365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP. 
  
Na przykład dla zasad SSN skonfigurowanych z poziomem ufności 85%, następujące są oceniane i muszą zostać wykryte, aby reguła wyzwoliła:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cyfr, które mogą znajdować się w sformatowanym lub niesformatowanym wzorze

- **[Wzór:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje wyszukuje sieci SSN w czterech różnych wzorcach:

  - Func_ssn wyszukuje sieci SSN z silnym formatowaniem sprzed 2011 r., sformatowanym z myślnikami lub spacjami (ddd-dddd LUB ddd dd ddd dddd)

  - Func_unformatted_ssn wyszukuje sieci SSN z silnym formatowaniem sprzed 2011 r., które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddddd)

  - Func_randomized_formatted_ssn znajdzie sieci SSN po 2011 r., które są sformatowane myślnikami lub spacjami (ddd-ddd-ddd ddd ddddd)

  - Func_randomized_unformatted_ssn znajduje sieci SSN po 2011 r., które są niesformatowane jako dziewięć kolejnych cyfr (ddddddddd)

- **[Suma kontrolna:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie ma sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Zasady DLP są w 85% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:

  - [Funkcja Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) znajduje zawartość, która pasuje do wzorca.

  - Zostanie znalezione słowo kluczowe z [Keyword_ssn.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) Przykłady słów kluczowych obejmują: *Social Security, Social Security#, Soc Sec , SSN* . Na przykład następujący przykład może wyzwolić dla zasad DLP SSN: **SSN: 489-36-8350**
  
Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrywania sieci SSN dla zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają w sieci SSNS](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  