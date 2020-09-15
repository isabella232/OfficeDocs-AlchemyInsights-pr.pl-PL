---
title: Reguła DLP dla numeru PESEL nie działa
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
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679379"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problemy dotyczące DLP z numerami PESEL

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z aplikacją DLP SSNs**

Czy występują problemy z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer PESEL (SSN)** , gdy jest używany typ informacji wrażliwych w programie Microsoft 365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące działania zasad DLP. 
  
Na przykład w przypadku zasad SSN skonfigurowanych z poziomem ufności 85% obliczane są następujące wartości, które muszą zostać wykryte, aby reguła była wyzwalana:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cyfr, które mogą znajdować się w sformatowanym lub niesformatowanym deseniu

- **[Wzorzec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Cztery funkcje Szukaj SSNs w czterech różnych wzorach:

  - Func_ssn odnajduje SSNs przy użyciu funkcji 2011 wcześniejszego formatowania, które są sformatowane za pomocą kresek lub spacji (DDD-DD-dddd lub DDD DD dddd)

  - Func_unformatted_ssn znajduje SSNs o silnym formatowaniu sprzed 2011, które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddd)

  - Func_randomized_formatted_ssn znajduje znaki post-2011 SSNs, które są sformatowane za pomocą kresek lub spacji (DDD-DD-dddd lub DDD DD dddd)

  - Func_randomized_unformatted_ssn znajduje znaki post-2011 SSNs, które nie są sformatowane jako dziewięć kolejnych cyfr (ddddddddd)

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Zasady DLP to 85% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:

  - [Funkcja Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) umożliwia Znajdowanie zawartości zgodnej ze wzorcem.

  - Znaleziono słowo kluczowe from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Przykłady słów kluczowych:  *zabezpieczenia społecznego, ubezpieczenie społeczne, #, SOC SEC, SSN*  . Na przykład poniższa przykład wywoła zasady SSN dla DLP: **SSN: 489-36-8350**
  
Aby uzyskać więcej informacji na temat tego, co jest wymagane, aby SSNs został wykryty dla zawartości, zobacz poniższą sekcję w tym artykule: co to są [typy informacji wrażliwych na SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .
  