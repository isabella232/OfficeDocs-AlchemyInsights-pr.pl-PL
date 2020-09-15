---
title: Reguła DLP dla numeru paszportu my/UK nie działa
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: pl-PL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679234"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemy z numerami paszportów DLP-USA/UK

**Ważne**: w tych niespotykanych czasach podejmujemy kroki zapewniające stałą wysoką dostępność usług SharePoint Online i OneDrive. Aby uzyskać więcej informacji, zapoznaj się z [tymczasowymi zmianami funkcji usługi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemy ze współdziałaniem z numerami Passport w USA/Wielkiej Brytanii**

Czy występują problemy z **zapobieganiem utracie danych (DLP)** nie działają w przypadku zawartości zawierającej **numer paszportu USA/Wielkiej Brytanii** w przypadku korzystania z typu informacji poufnych dla DLP w usłudze O365? Jeśli tak, upewnij się, że zawartość zawiera potrzebne informacje dotyczące tego, co mają zasady DLP podczas szacowania.
  
Na przykład w przypadku zasad **numeru paszportów amerykańskich/brytyjskich** skonfigurowanych z poziomem ufności równą 75% zostaną obliczone następujące obliczenia i trzeba je wykryć, aby reguła była wyzwalana.
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Dziewięć cyfr

- **[Wzorzec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Dziewięć kolejnych cyfr

- **[Suma kontrolna:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie ma żadnej sumy kontrolnej

- **[Definicja:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Zasady DLP to 75% pewności, że wykryto ten typ poufnych informacji, jeśli w pobliżu 300 znaków:

  - Funkcja Func_usa_uk_passport umożliwia Znajdowanie zawartości zgodnej ze wzorcem.

  - Znaleziono słowo kluczowe from Keyword_passport.

    Na przykład Poniższa przykładowa zasada **numeru paszportu US/UK** jest wyzwalana: numer paszportu amerykańskiego 123456789

Aby uzyskać więcej informacji na temat tego, co jest wymagane w przypadku wykrycia dla zawartości numeru paszportu USA/Wielkiej Brytanii, zobacz poniższą sekcję w tym artykule: [co to są typy informacji wrażliwych na numer paszportu my/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .
  
Korzystając z innego wbudowanego typu informacji poufnych, zobacz następujący artykuł, aby uzyskać informacje o tym, co jest wymagane dla innych typów: [czego szukają typy informacji wrażliwych](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) .
  