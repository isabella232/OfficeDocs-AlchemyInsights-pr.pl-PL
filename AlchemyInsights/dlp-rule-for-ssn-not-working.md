---
title: Reguła DLP dla SSN nie działa
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004992"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemy w zakresie ochrony przed zagrożeniami (DLP) dotyczące numerów PESEL

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy dotyczące DLP związane z sieciami SSN**

Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention)** nie działa w przypadku zawartości zawierającej numer **PE** PESZ podczas korzystania z typu informacji poufnych w programie Microsoft 365? Jeśli tak, upewnij się, że zawartość zawiera niezbędne informacje na temat zasad DLP. 
  
Na przykład w przypadku zasad SSN skonfigurowanych z poziomem ufności 85%, następujące zasady są sprawdzane i należy je wykrywać, aby reguła wyzwalała:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cyfr, które mogą być sformatowane lub niesformatowane

- **[Wzorzec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje szukają sieci SSN w czterech różnych wzorcach:

  - Func_ssn umożliwia znalezienie ssnów o formatowaniu silnych danych przed 2011 r. sformatowanych za pomocą kresek lub spacji (ddd-dd-dddd OR ddd dddd)

  - Func_unformatted_ssn umożliwia znalezienie ssnów z formatowaniem znaczącym przed 2011 erą, które są niesformatowane jako dziewięć kolejnych cyfr (dddddddddd)

  - Func_randomized_formatted_ssn umożliwia znalezienie po 2011 r. SNS sformatowanych za pomocą kresek lub spacji (ddd-dd-dddd OR ddd dddd)

  - Func_randomized_unformatted_ssn umożliwia znalezienie po 2011 r. numerów SSN, które są niesformatowane jako dziewięć następujących po sobie cyfr (dddddddddd)

- **[Sumy kontrolne:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zasady DLP mają 85% pewności, że wykrywane są tego typu informacje poufne, jeśli w odległości 300 znaków:

  - Funkcja [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) umożliwia znalezienie zawartości, która pasuje do wzorca.

  - Słowo kluczowe z [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) znajduje się. Przykładowe słowa kluczowe to:  *Ubezpieczenia społecznego, Ubezpieczenia Społecznego#, Soc S, SSN*  . Na przykład następująca próbka powoduje uruchomienie zasad DLP **SSN: SSN: 489-36-8350**
  
Aby uzyskać więcej informacji na temat tego, co jest wymagane, aby sieci SSNs zostały wykryte dla Twojej zawartości, zobacz następującą sekcję w tym artykule: Co typ informacji poufnych ma dla [tych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) typów.
  
Informacje wymagane dla innych typów można znaleźć w następującym artykule, w którym podano informacje o innych [typach:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Typy informacji poufnych
  