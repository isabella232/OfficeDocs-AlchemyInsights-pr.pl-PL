---
title: Reguła DLP dla numeru paszportu USA/Wielkiej Brytanii nie działa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507308"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemy z DLP - numery paszportów USA/Wielkiej Brytanii

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy z DLP z numerami paszportów USA/Wielkiej Brytanii**

Czy masz problemy z **zapobieganiem utracie danych (DLP)** nie działa dla treści zawierających **numer paszportu USA / Wielkiej Brytanii** podczas korzystania z DLP typu poufnych informacji w O365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, czego szukają zasady DLP podczas oceny.
  
Na przykład w przypadku zasad **dotyczących numerów paszportów w STANACH Zjednoczonych/Wielkiej Brytanii** skonfigurowanych z poziomem ufności równym 75%, następujące zasady są oceniane i muszą zostać wykryte, aby reguła
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dziewięć cyfr

- **[Wzór:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Dziewięć kolejnych cyfr

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zasady DLP są w 75% pewne, że wykryto tego typu poufne informacje, jeśli w pobliżu 300 znaków:

  - Funkcja Func_usa_uk_passport znajduje zawartość, która pasuje do wzorca.

  - Zostanie znalezione słowo kluczowe z Keyword_passport.

    Na przykład następująca próbka spowoduje uruchomienie dla zasad **dotyczących numerów paszportów USA/Wielkiej Brytanii:** numer paszportu USA 123456789

Aby uzyskać więcej informacji na temat tego, co jest wymagane do wykrycia numeru paszportu USA/WIELKIEJ BRYTANII dla twojej zawartości, zobacz następującą sekcję w tym artykule: [Jakie typy poufnych informacji szukają numeru paszportu USA/Wielkiej Brytanii](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Przy użyciu innego wbudowanego typu poufnych informacji, zobacz następujący artykuł, aby uzyskać informacje na temat tego, co jest wymagane dla innych typów: [Czego szukają typy poufnych informacji](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  