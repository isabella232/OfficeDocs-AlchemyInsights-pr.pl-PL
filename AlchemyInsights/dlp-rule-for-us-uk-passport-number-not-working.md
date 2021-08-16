---
title: Reguła DLP nie działa dla numeru paszportu Stanów Zjednoczonych/Zjednoczonego Królestwa
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004956"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemy z dlp — numery paszportów Stanów Zjednoczonych/Zjednoczonego Królestwa

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z dlp dotyczące numerów paszportu Stanów Zjednoczonych/Zjednoczonego Królestwa**

Czy masz problemy z zapobieganiem utracie danych **(DLP, Data Loss Prevention)** nie działa w przypadku zawartości zawierającej numer paszportu Stanów **Zjednoczonych/Zjednoczonego** Królestwa podczas korzystania z typu informacji poufnych ochrony przed utratą danych w U365? Jeśli tak, upewnij się, że zawartość zawiera niezbędne informacje na potrzeby oceny zasad DLP.
  
Na przykład w przypadku zasad numer paszportu Stanów **Zjednoczonych/Zjednoczonego** Królestwa skonfigurowanych z poziomem ufności 75% następujące zasady są sprawdzane i należy je wykrywać, aby reguła uruchamiała
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dziewięć cyfr

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Dziewięć kolejnych cyfr

- **[Sumy kontrolne:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zasady DLP mają 75% pewności, że wykrywane są tego typu informacje poufne, jeśli w odległości 300 znaków:

  - Funkcja Func_usa_uk_passport znajdzie zawartość, która odpowiada wzorcowi.

  - Zostanie znalezione słowo kluczowe Keyword_passport.

    Przykładem może być zasady numer paszportu Stanów **Zjednoczonych/Zjednoczonego** Królestwa: Numer paszportu Stanów Zjednoczonych 123456789

Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia numeru paszportu Stanów Zjednoczonych/Zjednoczonego Królestwa dla Twojej zawartości, zobacz następującą sekcję w tym artykule: Jakie informacje poufne mają na przykład typy danych [US/UK Passport](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Informacje wymagane dla innych typów można znaleźć w następującym artykule, w którym podano informacje o innych [typach:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) Typy informacji poufnych
  